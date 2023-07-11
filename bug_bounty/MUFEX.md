# ParaSpace Bug Bounty

## Bounty Guideline
- Active Since: July 11st, 2023
- Accept Threat Level: **Critical**, **High**, **Medium**, **Low**
- PoC required: **Yes**
- Minimum Reward: `500` USD
- Maximum Reward Cap: `500,000` USD
- KYC Required for Reward: No
- Submit Bug -> [Submit](https://forms.gle/wZ1Pdh7TeEGfwVGY6)

## Project Overview
Most User-Friendly EXchange, please visit https://www.mufex.finance.
MUFEX is a Decentralized Perpetual Exchange deployed across multiple chains.
By combining the strengths of centralized exchanges (CEX) and decentralized exchanges (DEX) while mitigating their respective weaknesses, MUFEX aims to revolutionize the landscape of decentralized trading.
Launched in 2023, users can enjoy secure and seamless trading on MUFEX with leverage of up to 150X. With a wide selection of contract trading assets, a comprehensive range of trading services, and a robust ecosystem, MUFEX enables users worldwide to experience secure, transparent, and fair trading services. 


## Reward by Threat Level

Critical
   up to USD $500,000
High
   USD $10,000
Medium
   USD $5,000
Low
   USD $500
Information
   None

**This reward plan is only applicable to Smart Contracts.**

## Impacts in Scope

### Critical 
- Any governance voting result manipulation
- Direct theft of any user funds, whether at-rest or in-motion, other than unclaimed yield
- Permanent freezing of funds
- Miner-extractable value (MEV)
- Protocol insolvency


### High  
- Theft of unclaimed yield
- Theft of unclaimed royalties
- Permanent freezing of unclaimed yield
- Permanent freezing of unclaimed royalties
- Temporary freezing of funds


### Medium   
- Smart contract unable to operate due to lack of token funds
- Block stuffing for profit
- Griefing (e.g. no profit motive for an attacker, but damage to the users or the protocol)
- Theft of gas
- Unbounded gas consumption


### Low   
- Contract fails to deliver promised returns, but doesn't lose value


### Information  
- Best practices


## KYC Requirement
N/A

## Asset In Scope
- https://arbiscan.io/address/0x763ecd00eEA0CDAECBDF97d88c3e0fd5457eE5A0 HotTreasury
- https://polygonscan.com/address/0x763ecd00eEA0CDAECBDF97d88c3e0fd5457eE5A0 HotTreasury
- https://arbiscan.io/address/0x16bedb2ab2aef9023ff2cbf0c78135ca120c03c6 MainTreasury
- https://arbiscan.io/address/0xc8a3a6d43e8aa43187d7b7a1faef21e65acba43b DepositWalletFactory



## Out of Scope & Rules

- Incorrect data supplied by third party oracles
- Not to exclude oracle manipulation/flash loan attacks
- Basic economic governance attacks (e.g. 51% attack)
- Lack of liquidity
- Best practice critiques
- Sybil attacks
- Vulnerabilities already reported and/or discovered in contracts built by third parties on MUFEX
- Bugs in any third party contract or platform that interacts with MUFEX





