# Uniwhale Bounty

## Bounty Guidelines
- Active Since: Mar 1st, 2023
- Accept Threat Level: **High**, **Critical**
- PoC required: **Yes**
- Minimum Reward: `5,000` UNW
- Maximum Reward Cap: `500,000` UNW (i.e. `0.5%` of the total supply)
- KYC Required for Reward: **Yes**
- How to Submit a Bug:
    - Email: bug_bounty@secure3.io
    - Include `Uniwhale Bug Bounty` in the email title

## Project Overview
Uniwhale is an oracle-based decentralized on-chain perpetual trading exchange where
You can trade, with up to 200x leverage, BTC, ETH, and many mainstream crypto assets, directly from your wallet.
You can provide liquidity with stablecoins like BUSD, USDC, USDT, and more, to earn real yield from market-making and leverage trading.

For more information about Uniwhale, please visit https://www.uniwhale.co/.

This bug bounty program is focused on their smart contracts and is focused on preventing:
- Thefts and freezing of principal of any amount
- Thefts and freezing of unclaimed yield of any amount
- Theft of governance funds
- Governance activity disruption

## Reward by Threat Level

Rewards are distributed according to the impact of the vulnerability.

All **High** and **Critical** Smart Contract bug reports **require a PoC in order to be considered for a reward**. Explanations and statements are not accepted as PoC and code is required.

This bug bounty program has fixed rewards in UNW. The USD amounts reflected are only estimates. For an up-to-date price of the token, please visit https://www.uniwhale.co/.

Critical smart contract vulnerabilities are capped at `10%` of economic damage, primarily taking into consideration funds at risk, but also PR and branding aspects, at the discretion of the team. However, there is a minimum reward of UNW `5,000`. Additionally, the maximum reward is capped at `500,000` UNW (i.e. `0.5%` of the total supply), even if `10%` of the damage in USD equivalent is greater than the USD equivalent of `500,000` UNW.

**The following vulnerabilities are not eligible for a reward: `TODO: [security audit reports links].`**


Payouts are handled by the Uniwhale team directly and are denominated in UNW. Payouts are done in UNW.

## Impacts in Scope
Only the following impacts are accepted within this bug bounty program. All other impacts are not considered as in-scope, even if they affect something in the assets in scope table.

##### Critical
- Loss of user funds staked (principal) by freezing or theft
- Vote manipulation
- Miner-extractable value (MEV)
- Protocol Insolvency
- Permanent freezing of funds

#####  High
- Theft of unclaimed yield
- Freezing of unclaimed yield
- Temporary freezing of funds for a minimum period of 1 day


## KYC Requirement
Uniwhale requires KYC to be done for all bug bounty hunters submitting a report and wanting a reward. The information needed are:
1. Name
1. Email Address
1. Residential Address
1. Nationality
1. Stacks Wallet Address
1. Identity Proof (Passport / Driver License / National ID)
1. Address Proof (Utility Bill / Bank Statement)

**The collection of this information will be done by the Uniwhale team.**




## Asset In Scope
- [ ] TODO: github link with description


## Out of Scope & Rules


The following vulnerabilities are excluded from the rewards for this bug bounty program:
- Attacks that the reporter has already exploited themselves, leading to damage
- Attacks requiring access to leaked keys/credentials
- Attacks requiring access to privileged addresses (governance, strategist)
- Incorrect data supplied by third party oracles
- Not to exclude oracle manipulation/flash loan attacks
- Basic economic governance attacks (e.g. 51% attack)
- Lack of liquidity
- Best practice critiques
- Sybil attacks
- Centralization risks

The following activities are prohibited by this bug bounty program:
1. Any testing with mainnet or public testnet contracts; all testing should be done on private testnets
1. Any testing with pricing oracles or third party smart contracts
1. Attempting phishing or other social engineering attacks against our employees and/or customers
1. Any testing with third party systems and applications (e.g. browser extensions) as well as websites (e.g. SSO providers, advertising networks)
1. Any denial of service attacks
1. Automated testing of services that generates significant amounts of traffic
1. Public disclosure of an unpatched vulnerability in an embargoed bounty
