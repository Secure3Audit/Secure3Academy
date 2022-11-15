# Secure3 Security Vulnerability Severity Definition

Blockchain security vulnerabilities are security flaws and security risks that arise during the design, implementation, configuration, and operation of blockchain systems. These defects and risks exist in different forms in the system architecture, business logic, algorithm design, code implementation and other aspects of the blockchain system. Once exploited by attackers, the vulnerabilities will cause huge damage to the security of the funds, data, network, nodes, etc. of the blockchain system, thereby affecting the normal operation. To objectively and quantitatively assess the threat level of vulnerabilities in blockchain systems, Secure3 has formulated a set of detailed vulnerability grading rules based on CVSS 2.0 (Common Vulnerability Scoring System) and in combination with blockchain characteristics and application scenarios.
The methods described in these rules are applicable to the security vulnerability grading scenarios of blockchain **smart contracts**.

## Vulnerability rating system
Vulnerabilities are essentially unintended security flaws or risks, which can be classified into four threat levels: "Critical", "Medium", "Low" and "Informational". The rating is mainly based on the degree of harm and difficulty of exploiting the vulnerability, supplemented by other factors comprehensive judgment, including:

The degree of harm is mainly defined according to three dimensions: 
- confidentiality impact (C), 
- integrity impact (I), 
- availability impact (A);

The difficulty of exploitation is mainly defined according to the three dimensions of:
- attack vector (AV), 
- attack complexity (AC), 
- authentication (Au).

|                   | serious damage | high damage | medium damage | low damage    |
|-------------------|----------------|-------------|---------------|---------------|
| low difficulty    | Critical       | Critical    | Medium        | Low           |
| medium difficulty | Critical       | Medium      | Low           | Low           |
| high difficulty   | Medium         | Low         | Low           | Informational |
| very difficult    | Low            | Low         | Informational | Informational |


## The degree of harm and the difficulty of exploitation

### Degree of Damage
#### Serious Damage
Serious harm generally refers to the vulnerability that can have a bad impact on confidentiality, integrity, availability or its economic model of a smart contract, and can cause a lot of economic losses to the contract business features, large-scale data issue, privilege access compromise, failure of critical functions, and loss of credibility, or affecting the normal operation of other smart contracts interacting with it and cause a lot of losses and irreversible damage.
Including but not limited to:
- Large-scale additional issuance or overspending of assets.
- Large asset theft or unauthorized spending.
- The core business of smart contracts cannot operate normally, such as denial of service, etc.
- The core business logic of smart contracts is arbitrarily tampered with or bypassed, such as transfers, charges, accounting, etc.
- The key verification logic of smart contracts is bypassed, such as signature verification, proof verification, authentication, etc.

#### High Damage
High harm generally means that the vulnerability can have a bad impact on confidentiality, integrity, availability or its economic model of the smart contract, and can cause greater economic losses to the contract business system, partial function unavailability, and reduced credibility.
Including but not limited to:
- Great loss or freeze of other people's assets, or significant reduction in expected income.
- Unexpected sensitive information leakage that can directly cause economic loss or other obvious harm.
- The core fairness design of smart contracts is invalid, such as voting, lottery, auction etc
- The core economic model design of smart contracts is invalid. For example, the contract introduces mining incentives but there are serious problems with the mechanism.

#### Medium Damage
Medium damage generally refers to vulnerabilities that can have a slight impact on the confidentiality, integrity, availability or its economic model of smart contracts, and can cause a small amount of economic loss to the contract business system and the unavailability of individual services.
Including but not limited to:
- Small additional issuance or over issuance of assets.
- Small asset theft or unauthorized spending.
- Small loss or freeze of other people's assets, or small unexpected decrease in income.
- Some non-core businesses of smart contracts cannot operate normally.
- Unexpected leakage of sensitive information that will not directly cause economic loss or other obvious harm.
- Certain types of smart contracts use non-standard interfaces or implementations that can cause external system losses.

#### Low Damage
Low Damage generally refers to the risks and hazards that the vulnerability can have a slight impact on the smart contract, can pose a security threat to the contract business system, and need to be improved.
Including but not limited to:
- The operation stability of smart contracts is affected, such as abnormally high contract invocation failure rate, abnormally high resource consumption, etc.
- Certain types of smart contracts use non-standard interfaces or implementations, which affect safe calls or interface compatibility without causing losses.
- To a certain extent, it reduces the difficulty of exploiting other attacks.
- Smart contracts can be triggered by false or error events without causing losses.
- Other issues that clearly violate security development norms and may introduce potential risks.

### Difficulty to exploit
#### Low difficulty
Low difficulty generally means that the cost of exploiting a vulnerability is low, there is no special exploitation threshold, and the vulnerability can be triggered consistently.
Including but not limited to:
- The Attack requires a small or close to 0 capital cost.
- Need to hold a small amount of a certain asset.

#### Moderate difficulty
Moderate difficulty generally means that the vulnerability requires a certain cost, or there are certain exploitation conditions, and the vulnerability is not easily triggered consistently.
Including but not limited to:
- It requires a certain amount of capital cost that is less than the profit of the attack.
- It requires the attacker's own account assets or assets in the contract to reach a certain scale, such as close to the maximum attack profit.
- It requires the attacker to meet certain normal conditions, such as collaboration with a miner or block producing node, or the ability to package transactions and produce blocks to rearrange or filter transactions.
- It requires the victim to meet certain normal conditions, such as the asset amount being in a certain range.
- It needs to be combined with common attack methods in non-smart contracts, such as attacking off-chain data sources.
- It needs to be combined with known attack methods in smart contracts, such as attacking other Oracle contracts on the chain.
- It requires attackers to use higher transaction fees, such as higher gas for front-running.
- It needs to trigger within a certain time frame, such as a specific block height.
- It requires transactions to be executed in specific scenarios, such as specific transactions packaged in Uncle Block.
- It requires a certain time cost, such as several days.
- It requires a certain amount of network/computing resources.


#### High difficulty
High difficulty generally means that the vulnerability requires a higher cost, or the exploitation conditions are very strict, and the vulnerability is difficult to trigger.
Including but not limited to:
- It needs to pay a large capital cost not less than the attack profit.
- It requires the attacker's own account assets or assets in the contract to reach a high scale, such as significantly higher than the maximum attack profit.
- It requires the victim to meet certain low-frequency conditions, such as interacting with certain non-essential contracts.
- It requires attackers to be a small number of non-critical accounts that meet certain criteria.
- It requires significant time costs, such as several months and more.
- It requires extensive use of network/computing resources.

#### Very high difficulty
Extreme difficulty generally means that the vulnerability requires a very high cost, or the exploit conditions are extremely difficult to achieve.
Including but not limited to:
- Costs are normally unattainable.
- It needs to meet some special conditions that are not easy to occur under normal circumstances.
- Only a very small number of accounts are able to launch the attack.
- It needs to be able to control private keys of critical accounts, such as contract administrators.
