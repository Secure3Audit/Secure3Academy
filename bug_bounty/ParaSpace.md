# ParaSpace Bug Bounty

## Bounty Guideline
- Active Since: Apr 4th, 2023
- Accept Threat Level: **Critical**, **High**, **Medium**
- PoC required: **Yes**
- Minimum Reward: `3,000` USD
- Maximum Reward Cap: `200,000` USD
- KYC Required for Reward: No
- Submit Bug -> [Submit](https://forms.gle/iCVyupRVtCbV61zG8)

## Project Overview
Para Space is a decentralized protocol with a foundation of providing lending and borrowing services for various assets on the Ethereum blockchain. Users can lend their NFTs and ERC-20 tokens to earn income in the form of interest, as well as use their lended assets as collateral for borrowing assets. One of the main entry bars for retail users into the NFT market is the high price of NFT items, especially blue-chip NFTs, therefore, ParaSpace introduces its Marketplace, allowing users to access NFTs through leveraged buy and leveraged bid, using the purchased item as collateral for the outstanding loan.

The Para Space protocol aims to provide users access to cash and profits without selling their assets. Para Space uses a pool-based money market model whereby users supply their assets to a pool to earn interest and instantly borrow from the pool when collateralizing their asset.

For more information about Para Space, please visit https://para.space/.

## Reward by Threat Level

Rewards are distributed according to the impact of the vulnerability based on the [Secure3 Security Vulnerability Severity Definition](../IssueSeverityDefinition.md). This is a simplified 4-level scale, with separate scales for websites/apps, smart contracts, and blockchains/DLTs, focusing on the impact of the vulnerability reported.

All bug reports must come with a PoC with an end-effect impacting an asset-in-scope in order to be considered for a reward. Explanations and statements are not accepted as PoC and code is required. In addition, all bug reports must come with a suggestion for a fix in order to be considered for a reward.

Known issues highlighted in the following audit reports are considered out of scope:
- [Certik Audit](https://625248360-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FSkcQFPKbtOmfoFkTbdbO%2Fuploads%2FTrzK55XEvu2r3uBZANDN%2FREP-final-20221025T060830Z.pdf?alt=media&token=0a582b33-f05c-4e6e-b66e-f3da32b0cb4c)
- [Secure3](https://github.com/Secure3Audit/Secure3Academy/tree/main/audit_reports/ParaSpace)
- [Trail of Bits](https://github.com/trailofbits/publications/blob/master/reviews/ParallelFinance2FixReview.pdf)
- [Trail of Bits](https://github.com/trailofbits/publications/blob/master/reviews/ParallelFinance3.pdf)
- [0xQuit](https://625248360-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FSkcQFPKbtOmfoFkTbdbO%2Fuploads%2F68ZQDO2ooO08WQzgSfwi%2FParaSpace%20Contract%20Audit.pdf?alt=media&token=24b5b3c3-ae8e-4c5a-92c3-17b5dd3edd92)
- [Veridise](https://625248360-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FSkcQFPKbtOmfoFkTbdbO%2Fuploads%2FfF8ZVrmygSWIz8tY6n0x%2FVAR_Parallel2.pdf?alt=media&token=72e49c1e-2c00-408e-8a89-437543e404ad)
- [0xQuit](https://625248360-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FSkcQFPKbtOmfoFkTbdbO%2Fuploads%2FJBp3r0NvwTBshjgbZSDr%2FParaSpace%20Autocompounding%20Ape%20Review.pdf?alt=media&token=c9bd379d-880b-4c96-a818-3e1cd878ca1b)
- [Secure3](https://625248360-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FSkcQFPKbtOmfoFkTbdbO%2Fuploads%2FZLVihMsHpqmJFhnm0kZi%2FParaSpaceApeYield_final_Secure3_Audit_Report.pdf?alt=media&token=937eba50-b975-4753-b034-90c175b42073)
- [Secure3](https://625248360-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FSkcQFPKbtOmfoFkTbdbO%2Fuploads%2FcmfaiYVL3O1Qq4KyVIJJ%2FParaSpaceV1.4P1_final_Secure3_Audit_Report.pdf?alt=media&token=4b74a271-c549-41e7-b3ee-4d065ce87d8d)
- [Secure3](https://625248360-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FSkcQFPKbtOmfoFkTbdbO%2Fuploads%2FLimRSLp0Erz0egxrW2fS%2FParaSpaceV1.4P2_final_Secure3_Audit_Report.pdf?alt=media&token=20115def-6481-496f-8fed-78264c4ed073)
- [Secure3](https://docs.google.com/document/d/14rBCh8Iofg1UrpAUinycj-uAdATCR5CcmWgtmcw_lUg/edit)

To be eligible for a reward under this Program, you must:
- Discover a previously unreported, non-public vulnerability within the scope of this Program. Vulnerabilities must be distinct from the issues covered in the previously conducted publicly available audits.
- Be the first to disclose the unique vulnerability to the Team by the disclosure requirements below. If similar vulnerabilities are reported, the first submission shall be rewarded (if determined valid and otherwise in the scope of this Program).
- Possess sufficient technical knowledge and provide sufficient information necessary to reproduce and fix the vulnerability.
- Not engage in any unlawful conduct when disclosing the bug, including through threats, demands, or any other coercive tactics.
- Not exploit the vulnerability in any way, including by making it public or obtaining a profit (other than a reward under this Program). Any publicity in any way, whether direct or indirect, relating to any bug or vulnerability will automatically disqualify it and you from the Program.
- Make a good faith effort to avoid privacy violations, data destruction, interruption or degradation of ParaSpace.
- Submit only one vulnerability per submission unless you need to chain vulnerabilities to impact any vulnerabilities. If you want to add more information to a provided issue, create a new submission referencing the initial one.
- Not submit a separate vulnerability caused by an underlying issue that is the same as an issue on which a reward has been paid under this Program. However, if a vulnerability is found that bypasses a previous fix that was deployed, it will still be considered within the scope of this program.

Payouts are handled by the Para Space team directly and are denominated in USD. However, payouts are conducted in USDC. Future payouts may be done in our own protocol token, at the discretion of the team.

## Impacts in Scope

Critical:
- Direct theft of any user funds, whether at-rest or in-motion, other than unclaimed yield
- Direct theft of any user NFTs, whether at-rest or in-motion, other than unclaimed royalties
- Permanent freezing of user funds
- Permanent freezing of user NFTs
- Unauthorized minting of NFTs
- Unintended alteration of what the NFT represents (e.g. token URI, payload, artistic content)
- Protocol insolvency

High: 
- Theft of unclaimed yield
- Theft of unclaimed royalties
- Permanent freezing of unclaimed yield
- Permanent freezing of unclaimed royalties
- Temporary freezing of funds for at least 24 hours
- Temporary freezing NFTs for at least 24 hours

## KYC Requirement
N/A

## Asset In Scope
- https://github.com/para-space/paraspace-core/blob/main/contracts/misc/flashclaim/AirdropFlashClaimReceiver.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/misc/flashclaim/UserFlashclaimRegistry.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/misc/marketplaces/LooksRareAdapter.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/misc/marketplaces/SeaportAdapter.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/misc/marketplaces/X2Y2Adapter.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/misc/ERC721OracleWrapper.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/misc/NFTFloorOracle.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/misc/ParaSpaceOracle.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/misc/ProtocolDataProvider.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/misc/UniswapV3OracleWrapper.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/configuration/ACLManager.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/configuration/PoolAddressesProvider.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/configuration/PoolAddressesProviderRegistry.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/libraries/configuration/ReserveConfiguration.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/libraries/configuration/UserConfiguration.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/libraries/logic/AuctionLogic.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/libraries/logic/BorrowLogic.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/libraries/logic/ConfiguratorLogic.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/libraries/logic/FlashClaimLogic.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/libraries/logic/GenericLogic.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/libraries/logic/LiquidationLogic.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/libraries/logic/MarketplaceLogic.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/libraries/logic/PoolLogic.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/libraries/logic/ReserveLogic.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/libraries/logic/SupplyLogic.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/libraries/logic/ValidationLogic.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/pool/DefaultReserveAuctionStrategy.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/pool/DefaultReserveInterestRateStrategy.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/pool/PoolApeStaking.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/pool/PoolConfigurator.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/pool/PoolCore.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/pool/PoolMarketplace.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/pool/PoolParameters.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/pool/PoolStorage.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/tokenization/base/MintableIncentivizedERC721.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/tokenization/NToken.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/tokenization/NTokenApeStaking.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/tokenization/NTokenBAYC.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/tokenization/NTokenMAYC.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/tokenization/NTokenMoonBirds.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/tokenization/libraries/MintableERC721Logic.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/protocol/tokenization/libraries/ApeStakingLogic.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/ui/WETHGateway.sol 
- https://github.com/para-space/paraspace-core/blob/main/contracts/ui/WPunkGateway.sol 


## Out of Scope & Rules
The following vulnerabilities are excluded from the rewards for this bug bounty program:

Vulnerabilities related to domains, DNS or servers of websites
- Any already-reported bugs
- Attacks that the reporter has already exploited themselves, leading to damage
- Attacks requiring access to leaked keys/credentials
- Attacks requiring access to privileged addresses (governance, strategist)

Smart Contracts and Blockchain
- Vulnerabilities already reported and/or discovered in contracts built by third parties on ParaSpace
- Bugs in any third party contract or platform that interacts with ParaSpace
- Incorrect data supplied by third party oracles
- Not to exclude oracle manipulation/flash loan attacks
- Basic economic governance attacks (e.g. 51% attack)
- Lack of liquidity
- Best practice critiques
- Sybil attacks
- Centralization risks

The following activities are prohibited by this bug bounty program:
- Any testing with mainnet or public testnet contracts; all testing should be done on private testnets
- Any testing with pricing oracles or third party smart contracts
- Attempting phishing or other social engineering attacks against our employees and/or customers
- Any testing with third party systems and applications (e.g. browser extensions) as well as websites (e.g. SSO providers, advertising networks)
- Any denial of service attacks
- Automated testing of services that generates significant amounts of traffic
- Public disclosure of an unpatched vulnerability in an embargoed bounty





