# Secure3Academy - How to prepapre yourself to become a smart contract auditor

## Learn programming and blockchain fundamentals 
The ability to code is one of the prerequisites of becoming a successful auditor.

If you are absolutely new to the blockchain, make sure you also understand how blockchain works. There are a lot of useful materials online.

**Bonus**

Understand some of the "advanced" blockchain concepts
- Cryptography
- Byzantine fault tolerance (BFT)
- Plasma, side chains, bridges
- Rollups (Optimistic and Zero-Knowledge ZK)


## Learn Solidity, EVM, and dev tools basics 
There are a lot of blockchain ecosystems and corresponding programming languages, among which, Ethereum and other EVM compatible chains are the most popular ones.

To become a smart contract auditor, Solidity is the most important programming language that auditors must understand thoroughly. Understand the EVM at least the high level will help you in the long run even if you do not have to understand all the low level technical details such as every single Opcode

- [Solidity](https://docs.soliditylang.org/) official document
- [EVM](https://ethereum.org/en/developers/docs/evm/) the Ethereum Virtual Machine
- [Remix IDE](https://remix-project.org/) allows developing, deploying and administering smart contracts for Ethereum like blockchains. 

**Bonus**

- [web3.js](https://github.com/web3/web3.js) a collection of JS libraries that lets you interact with an Ethereum node remotely or locally.
- [Foundry](https://github.com/foundry-rs/foundry) is a blazing fast, portable and modular toolkit for Ethereum application development written in Rust.
- [Hardhat](https://hardhat.org/) is an Ethereum development environment. Compile your contracts and run them on a development network. 
- [Truffle](https://trufflesuite.com/) is a development environment, testing framework and asset pipeline for Ethereum, aiming to make life as an Ethereum developer easier.


## Learn popular smart contracts and projects

**Token Contracts**

- [ERC-20](https://ethereum.org/en/developers/docs/standards/tokens/erc-20/) the standard for Fungible Tokens 
- [ERC-777](https://ethereum.org/en/developers/docs/standards/tokens/erc-777/) the ERC-20 backwards compatible standard with callback hook functions
- [ERC-721](https://ethereum.org/en/developers/docs/standards/tokens/erc-721/) the standard for Non-Fungible Token (NFT)
- [ERC-1155](https://ethereum.org/en/developers/docs/standards/tokens/erc-1155/) Multi-Token Standard that can represent and control any number of fungible and non-fungible token types in one smart contract at the same time. 


**Proxies and Upgradeable Contracts**

- [Proxy Upgrade Pattern](https://docs.openzeppelin.com/upgrades-plugins/1.x/proxies) uses data separation to keep business logic and data in separate contracts to allow developers to achieve the upgradeable mechanism
- [Upgradeable Contracts](https://docs.openzeppelin.com/upgrades-plugins/1.x/writing-upgradeable) allows users to change the contract code, while preserving the state, balance, and address. Let’s see it in action.


**Bonus**

Understand popular DeFi protocols is crucial to understand other projects builds on top of it. The fundamental concept of DEX, AMM, Oracle is something you cannot miss

- [SushiSwap](https://github.com/sushiswap/sushiswap) is a decentralized exchange (DEX) using the ethereum blockchain. It provides an alternative to liquidity provider (LP) tokens exchange. The Automated Market Maker (AMM) protocol allows users to buy and sell through Sushi DEX without the tranditional order books.
- [Compound](https://docs.compound.finance/) is a decentralized, blockchain-based protocol that allows users to lend and borrow crypto — and have a say in its governance with its native COMP token.
- [Uniswap](https://github.com/Uniswap/v3-core) is an automated liquidity protocol powered by a constant product formula and implemented in a system of non-upgradeable smart contracts on the Ethereum blockchain.
- [Chainlink VRF](https://docs.chain.link/docs/vrf/v2/introduction/) decentralized oracle networks provide tamper-proof inputs, outputs, and computations to support advanced smart contracts on any blockchain. The Verifiable Random Function (VRF) is a provably fair and verifiable random number generator (RNG) that enables smart contracts to access random values without compromising security or usability.


## Learn Security and Tools

**Knowledge Base**

- [SWC Registry](https://swcregistry.io/) is a Smart Contract Weakness Classification and Test Cases maintained by the community.

- [Ethereum Smart Contract Security Best Practices](https://consensys.github.io/smart-contract-best-practices/) provides a baseline knowledge of security considerations for intermediate Solidity programmers maintained by ConsenSys Diligence.


**Tools**

- [Surya](https://github.com/ConsenSys/surya) is an utility tool for smart contract systems. It provides a number of visual outputs and information about the contracts' structure.
- [Solidity Visual Developer](https://marketplace.visualstudio.com/items?itemName=tintinweb.solidity-visual-auditor) is a Ethereum Solidity Language plugin customized for developers and auditors using Visual Studio Code
- [solidity-coverage](https://github.com/sc-forks/solidity-coverage) is a code coverage tool for Solidity testing
- [solhint](https://github.com/protofire/solhint) is a Solidity linter provides both Security and Style Guide validations.
- [Slither](https://github.com/crytic/slither) is a Solidity static analysis framework. It runs a suite of vulnerability detectors, prints visual information about contract details, and provides an API to easily write custom analyses. Slither enables developers to find vulnerabilities, enhance their code comprehension, and quickly prototype custom analyses.
- [Mythril](https://github.com/ConsenSys/mythril) is a security analysis tool for EVM bytecode. It detects security vulnerabilities in smart contracts built for Ethereum, Hedera, Quorum, Vechain, Roostock, Tron and other EVM-compatible blockchains. It uses symbolic execution, SMT solving and taint analysis to detect a variety of security vulnerabilities. 
- [Echidna](https://github.com/crytic/echidna) is a fast Smart Contract Fuzzer. It uses sophisticated grammar-based fuzzing campaigns based on a contract ABI to falsify user-defined predicates or Solidity assertions. 
- [Manticore](https://github.com/trailofbits/manticore) is a symbolic execution tool for the analysis of smart contracts and binaries.



**Bonus**

CTFs (Capture The Flags) are programing challenges where pre-designed security vulnerable smart contract is given and user needs to write code or smart contract to exploit the vulnerability. Below are some good and popular ones for you to practice your hacking skills.

- [Ethernaut](https://ethernaut.openzeppelin.com/)
- [Paradigm CTF](https://github.com/paradigmxyz/paradigm-ctf-2021)
- [Capture the Ether](https://capturetheether.com/)


## Learn from Real Experience with Secure3
By now you should be quite familiar with the smart contract security best pratices, theory behind the exploits and commonly used tools, you should try finding issues in real project and code to pratice your skills.
[Secure3](https://secure3.io/) provides the project for you to audit and learn from other auditors. Signup and become an auditor today and pratice your skills on [Secure3](https://secure3.io/). Here are some sample audit reports from Secure3 for you to take a look on what real audit report looks like.

- https://github.com/Secure3Audit/ClearDAO_Audit/tree/main/audit_report
- https://github.com/Secure3Audit/P12_Competitive_Audit/tree/main/audit_report
- https://github.com/Secure3Audit/Shield_SSVault_CA/tree/main/audit_report

Secure3 aims to secure Web3 by empowering a transparent, collaborative and verifiable security ecosystem. 
