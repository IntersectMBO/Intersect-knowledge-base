---
hidden: true
---

# Milestone report July 2024

## Continuity July Achievements

\
This report is a progress update which follows on from the previous Milestone report issued in June and provides a summary of achievements related to Cardano Continuity during the month of July.

More information on Continuity can be found in the [Cardano continuity | Intersect - Knowledge Base ](https://docs.intersectmbo.org/cardano/cardano-continuity) on the Intersect website.

### Byron

Byron continue to develop the GovTool WebApp by supporting the launch and running a beta testing period to discover and fix bugs and collect feedback and ideas.

#### During July they completed the following milestones:

#### Milestone 3 - GovTool - Beta Testing  - DRep Explorer & Governance Action Submission

“We are pleased to announce the conclusion of the beta testing phase for our project, GovTool. We are incredibly grateful to all participants for their engagement, valuable feedback, and constructive criticism. Your contributions have significantly helped us improve the functionality and stability of the tool.”

#### Milestone 4 - GovTool - DRep Explorer - Hard Fork Product Release

“We will release the latest stable version of the DRep Explorer section into the production environment once all external dependencies are resolved. This version will be crucial for the bootstrapping phase.”

#### Milestone 5 - GovTool - Governance Action Submission - Hard Fork Product Release

“We will release the latest stable version of the delegation section into the production environment once all external dependencies are resolved. This version will be crucial for the bootstrapping phase.”

#### GovTool - Support for Beta Testing - Deliverables 1 & 2 (Monthly)

“Over the past month, the GovTool team has been actively engaged in this process, ensuring a smooth and efficient maintenance.”

### DQuadrant

Dquadrant are focusing on developing a comprehensive testing strategy for dApps (decentralized applications). The key deliverables included the “Intersect dApps testing strategy document” and a reference document to support its implementation. These documents were designed to ensure the functionality and security of dApps through detailed testing protocol and strategic documentation.\
\
DQuadrant are also helping with the Chang Hard Fork by carrying out thorough testing, including checking old and new features in Plutus v3. The contract involves important tasks like verifying transaction costs, making sure older versions still work, and comparing the performance of Plutus v2 and v3. The testing also includes checking governance actions, wallet functions, and how the system handles different network conditions. The goal is to ensure the blockchain remains strong and effective after the upgrade, with clear documentation to back up these efforts.

#### During July they completed the following milestones:

#### Milestone 2 - Governance Actions Load Testing

“The overall purpose of our project is to test the Cardano node readiness for the Chang hard fork. Milestone 2 focuses on load testing governance actions within the Cardano network.

For Milestone 2, we implemented and observed scenarios involving multiple votes on various governance action proposals. Three distinct scenarios were tested: a majority vote leading to the enactment of one proposal, an equal vote leading to the enactment of the first proposal, and insufficient votes leading to no enactment. These tests confirmed the system's ability to accurately process and enact governance decisions based on the voting outcomes.

This milestone validates the Cardano network's stability and governance capabilities. By validating the voting and proposal mechanisms under different conditions, we ensure that the network can efficiently handle governance actions. This contributes to improved network security, stability, and the overall reliability of the Cardano community's decision-making processes.”

#### Milestone 3 - Drep, Votes, Delegation Negative testing

“The overall purpose of our project is to test the Cardano node readiness for the Chang hard fork. Milestone 3 is centered on testing various scenarios related to DReps, voting, and delegation processes.

In Milestone 3, we implemented and validated scenarios involving DReps and vote delegation. The tests included generating DRep IDs, enforcing single delegation, verifying stake registration requirements for delegation, preventing multiple DRep registrations, and testing the retirement process for DReps. Each test confirmed the correct behavior of the network's governance mechanisms, such as ensuring an ADA holder cannot delegate to multiple DReps and that only registered DReps can retire.

\
This milestone contributes significantly to the Cardano network by ensuring the accuracy and security of its governance and delegation processes. By validating these critical functions, we ensure the network's ability to manage decentralized voting and delegation efficiently, thereby improving overall network security, stability, and trust within the Cardano community.”

#### Milestone 4 - DApp Testing (use case: NFT Marketplace)

“The overall purpose of our project is to test the Cardano node readiness for the Chang hard fork. Milestone 4 focuses on DApp testing with use-case DApp as Cardano Marketplace. It focuses on the integration of PlutusV3 with existing marketplace decentralized applications (DApps) initially developed using PlutusV2. This milestone is crucial for the broader testing of Cardano, as it ensures that upgrades to the smart contract platform do not disrupt existing applications and that new features are utilized effectively.&#x20;

In Milestone 4, we conducted extensive tests to assess the compatibility and performance of PlutusV3 in the context of marketplace DApps. This included verifying the functionality of buy, sell, and mint operations using updated reference scripts and documenting computational costs and associated fees. Benchmark tests were performed to evaluate the performance improvements of PlutusV3, and compliance with CIP-69 standards was also confirmed.&#x20;

This milestone contributes to the Cardano network by ensuring that the transition to PlutusV3 is smooth and beneficial for DApp developers and users. By validating the integration and performance of new smart contract features, we validate the overall functionality, efficiency, and scalability of the Cardano ecosystem, contributing to a more robust platform for future developments and innovations.”

#### Milestone 5 - Mass delegate-to-abstain testing

“The overall purpose of our project is to test the Cardano node readiness for the Chang hard fork. Milestone 5 focuses on testing the Cardano network's ability to handle mass delegation to abstain from voting. This milestone is important in the broader development of Cardano as it ensures that the network can manage large-scale voting behaviors and still function smoothly.&#x20;

For Milestone 5, we tested a scenario where a large majority of ADA holders delegated their voting power to abstain. We conducted tests with 1,000 and 10,000 wallets, where 99% of ADA holders chose to abstain. Despite this, the governance action to update the constitutional committee was successfully ratified by the remaining DReps and SPOs. These tests confirmed that the network could handle extensive abstention while still processing governance actions accurately.&#x20;

This milestone validates the Cardano network by proving its capacity to manage large-scale delegation behaviors without compromising functionality. Ensuring that the network can handle mass abstention improves its stability and reliability, contributing to a more secure and efficient governance process for the Cardano community.”\


### EMURGO

EMURGO produces Educational Materials which will cover every aspect of CIP 1694, testing and support of the Cardano Serialisation library, Yoroi Extension & Mobile Wallet.

#### During July they completed the following milestones:

#### Cardano Serialization Library: Deliverable 1: -Update Cardano Serialization Library to support Conway and Deliverable 2: Test and release CSL

“EMURGO has completed all the development and testing required to upgrade the CSL to support the changes introduced in Cardano's Conway era, including the distributed governance model described within CIP-1694. Further incremental beta releases will also enable user-based testing via the SanchoNet governance test network.”

#### Yoroi Extension Wallet: Milestone 1: Upgrade Yoroi extension wallet to support the Conway ledger era and  Milestone 2: Upgrade Yoroi extension wallet to support CIP95 with nightly release

“EMURGO has upgraded Yoroi Extension Wallet (Desktop) to support Cardano's Conway era, enabling users a smooth transition to the post-Chang hard fork. This deliverable also includes a beta release via Yoroi Nightly to allow connectivity to the SanchoNet governance test network, and the extension of Yoroi to support the CIP-95 standard.”

#### Yoroi Mobile Wallet -  Milestone 1: Upgrade Yoroi mobile wallet to support The Conway ledger era and Milestone 2: Upgrade Yoroi mobile wallet to support CIP-95

“EMURGO has upgraded Yoroi Mobile Wallet to support Cardano's Conway era, enabling users a smooth transition to the post-Chang hard fork. This deliverable includes a beta release, to allow connectivity to the SanchoNet governance test network, and the extension of Yoroi to support the CIP-95 standard.”

### Input Output Infrastructure&#x20;

Input Output’s Infrastructure group is developing and testing the Cardano governance node in readiness for [CIP-1694](https://www.1694.io/) and continuity maintenance.

#### During July they completed the following milestones:

#### Delivery of Identity Management for ICC

“This release contains the latest governance changes for Identity Management to allow ICC key build for Constitution. This version of the node also adds support for reference scripts in the Conway era.”

#### Delivery of Sanchonet 8.11

“This release contains the latest governance changes for SanchoNet. It has support for a new cost model for Plutus v3, plus new Plutus byte string primitives. The Constitution Committee quorum has been renamed to threshold in the CLI and a new economic parameter minFeeRefScriptCostPerByte has been added for reference scripts. This version of the node also adds support for reference scripts in the Conway era.”

### WellTyped

Welltyped are developing new Log Structured Merge Tree implementations (LSM). These will store the ledger's UTxO set on disk rather than in memory, substantially increasing the number of UTxOs—supporting many more users—while also allowing nodes to run on cheaper, lower-spec machines.

#### During July they completed the following milestone:

#### Milestone 5 - Minimal Working Version

“Well-Typed are developing an on-disk storage component intended to be used in Cardano to help Cardano scale to much larger numbers of accounts and UTxO sizes, while preserving good system performance.&#x20;

In previous milestones we have delivered various pieces of internal functionality. In this milestone we have connected that internal functionality to the component’s public API for the first time. In particular we have filled in the part of the public API that covers basic key/value operations: lookup, insert and delete.

In addition for this milestone we have created a benchmark that simulates the UTxO workload (using the new public APIs for lookup, insert and delete) and measures the throughput. This benchmark will be used during the project to guide our work to improve performance, and at the end of the project to demonstrate whether the performance targets have been met.”
