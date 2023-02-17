# Checklist For Popular EVM Protocols in Solidity

format
```
------
### Short Subject

#### Suggestions

#### Sample Bad Code

#### Suggestions

------

```

## Uniswap V2 (PancakeSwap, Sushi...)
------
### Get price
#### Descrption
When building DeFi contracts that need token prices from onchain contract, it may bring security problems in subtle ways.

The following functions are vulnerable.

Function `getPriceV0` uses the result of `balanceOf` as the number of tokens in the pair. However, the attacker can [flash swap](https://docs.uniswap.org/contracts/v2/guides/smart-contract-integration/using-flash-swaps) and borrow tokens from uniswap pair to affect the `balanceOf` result in the same block.

Function `getPriceV1` uses the result of `getReserves` as the number of tokens in the pair. However, the attacker can make a huge swap to affect token price before the attack.

#### Sample Bad Code

```solidity
/**
 * Vulnerable getPriceV0 function
 */
function getPriceV0(address pair) public view returns(uint256) {
    address token0 = UniswapV2Pair(pair).token0();
    address token1 = UniswapV2Pair(pair).token1();
    return 10**18 * IERC20(token0).balanceOf(pair) / IERC20(token1).balanceOf(pair);
}

/**
 * Vulnerable getPriceV1 function
 */
function getPriceV1(address pair) public view returns(uint256) {
    (uint112 reserve0, uint112 reserve1, ) = UniswapV2Pair(pair).getReserves();
    return 10**18 * uint256(reserve0) / uint256(reserve1);
}
```
#### Suggestions


It's suggested to use average price instead of spot price. UniSwap provides [official Oracle](https://docs.uniswap.org/contracts/v2/concepts/core-concepts/oracles) for external contracts to get on-chain TWAPs. Check out its [example implementation](https://github.com/Uniswap/v2-periphery/blob/master/contracts/examples/ExampleOracleSimple.sol).

------
### Pair tokens address order

[token0](https://docs.uniswap.org/contracts/v2/reference/smart-contracts/pair#token0) and [token1](https://docs.uniswap.org/contracts/v2/reference/smart-contracts/pair#token1) represent the address of the token pair. When user input is used, it is worth checking that `token0` must be strictly less than `token1` by sort order.
------
### Reasonable amountOutMin

[amountOutMin](https://docs.uniswap.org/contracts/v2/reference/smart-contracts/router-02#swapexacttokensfortokens) is an important parameter that represents the minimum amount of output tokens that must be received for the transaction not to revert. It needs to set a reasonable `amountOutMin` when swapping tokens, otherwise there may be a loss of funds.

------
## Chainlink VRF

Check out [security considerations](https://docs.chain.link/vrf/v2/security)

- The reliability of VRF depends on trusted miners/validators. This is because they can manipulate the order of transactions to affect possible random numbers. To avoid the possible harm caused by miners/validators, it should:
    - Use `requestId` to match randomness requests with their fulfillment in order.
    - Do not re-request randomness, even if you don’t get an answer right away.

- `fulfillRandomWords` must not revert because VRF service will not attempt to call it a second time.

## Chainlink Price Feeds

- Chainlink's data feeds are grouped into different categories based on the level of data quality and risk. Use [verified feeds](https://docs.chain.link/data-feeds/selecting-data-feeds#-verified-feeds) for greater reliability.

- Add a pause function or a backup price Oracle because chainlink may appear abnormal during extreme market events.

- [decimals](https://docs.chain.link/data-feeds/price-feeds/api-reference#decimals) represent the number of decimals present in the response value. Pay attention to different decimals for different pairs when converting prices.

## Aave

TBD

## Compound

- Reentrancy risk if tokens with hook function(e.g. ERC777) used as collateral
- TBD

## Curve

- Need to set a reasonable `_expected`, otherwise there may be a loss of funds
- TBD

## Aragon (DAO)

TBD
