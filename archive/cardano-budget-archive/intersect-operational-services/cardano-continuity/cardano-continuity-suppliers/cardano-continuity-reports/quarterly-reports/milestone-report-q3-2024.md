# Milestone report Q3 2024

## Continuity Achievements for Q3 2024

Welcome to our Q3 2024 Delivery Assurance newsletter! This edition provides an update on the progress made across various Cardano Continuity contracts, highlighting the key achievements and milestones completed during the past few months.

### Key Achievements:

### Byron: GovTool Development & Testing

Byron have completed the remaining work on the GovTool WebApp, finalizing the beta testing phase and Hard Fork Product Releases. We have also successfully agreed a new statement of work to continue their work on the Cardano GovTool, which supports vital governance processes for Cardano. The contract includes; refactoring the front and back ends of the Delegation and Voting pillars, and maintaining and supporting these pillars through testing networks and mainnet phases, with an emphasis on fixing bugs and gathering feedback.

#### Milestone 3: GovTool Beta Testing - DRep Explorer & Governance Action Submission

“We are pleased to announce the conclusion of the beta testing phase for our project, GovTool. We are incredibly grateful to all participants for their engagement, valuable feedback, and constructive criticism. Your contributions have significantly helped us improve the functionality and stability of the tool.”

#### Milestone 4 & 5: Hard Fork Product Releases (DRep Explorer & Governance Action Submission)

“We will release the latest stable version of the DRep Explorer section into the production environment once all external dependencies are resolved. This version will be crucial for the bootstrapping phase.”

#### GovTool - Support for Beta Testing - Deliverables 1 & 2 (Monthly)

“Over the past month, the GovTool team has been actively engaged in this process, ensuring a smooth and efficient maintenance.”

#### August Monthly Deliverable - Govtool Pillar maintainer activities

“I am pleased to announce that we have successfully achieved several significant milestones over the past month. Here’s a summary of our key accomplishments:

1. Hard Fork Preparation and Execution: The team efficiently prepared for and executed a hard fork, demonstrating our strong commitment to technical excellence.
2. Initialization of Pilars: We initiated work on the Pilars project by setting up the necessary repositories, creating projects, and copying over some of the existing code.
3. Rebranding of GovTool: We have successfully rebranded Sanchonet GovTool to Cardano GovTool, aligning our tools with our broader strategic vision.
4. Pre-release of Design System: We launched the pre-release of the Design System to support Pilars, ensuring a uniform styling framework across our projects.”

### DQuadrant: Testing Strategies & Chang Hard Fork Support&#x20;

#### Testing Strategies

DQuadrant have completed the final milestones in their contract and have made significant contributions to Cardano’s testing framework, specifically related to the governance tooling and readiness for the Chang hard fork. Their efforts to test Plutus v3 and ensure the continued functionality of decentralized applications (DApps) have been crucial.

We have recently signed a new contract with DQuadrant to extend the testing frameworks for Cardano GovTool to accommodate new features. DQuadrant will maintain the Cardano GovTool integrated testing and the Governance Action Loader.

#### Milestone 3 - Extend coverage for Proposal Discussion Forum

“The overall purpose of our project is to test the GovTool functionalities for decentralized governance as indicated in CIP-1694. Milestone 3 focuses on testing the Proposal submission and discussion forum.&#x20;

For Milestone 3, we created user stories for proposal submission and discussion forum and had them reviewed by the respective team manager. A total of 38 tests were written for covering the user stories covering the cases for use cases like wallet connected/disconnected states, proposal submission, proposal validation, listing, searching, accessing, filtering, searching etc. These tests confirm the system's ability of GovTool to enable users to successfully submit a draft proposal for discussion and later submit as governance action.

This milestone validates the GovTool’s proposal submission and discussion forum’s capabilities. By validating the proposal submission and discussion mechanisms under different conditions, we ensure that the GovTool can correctly handle governance actions. This contributes to the overall effort to make decentralized governance possible for the Cardano community.”

#### Milestone 1 - Maintenance and hosting of Governance Actions Loader

“The overall purpose of our project is to test the GovTool functionalities for decentralized governance as indicated in CIP-1694. Milestone 1 focuses on maintaining and hosting the governance actions loader used for loading governance actions in bulk.

For Milestone 1, we had been maintaining and hosting the governance actions loader since the beginning. It had been operational until early July. At the moment, it is not fully operational because of the dependency bug [https://github.com/IntersectMBO/cardano-api/issues/594](https://github.com/IntersectMBO/cardano-api/issues/594)  Issue is created and fix is being prepared by the cardano-api. Once the bug is fixed on the dependency, the loader can be made operational again.

The Governance Actions Loader is useful in loading multiple governance actions in bulk which helps in (stress) testing the GovTool. The loader internally handles the constraints of linking the correct previous governance actions and preparing valid governance actions to submit on chain. This contributes to the overall testing effort to make decentralized governance possible for the Cardano community.”

### Chang Hard Fork Testing

#### Milestone 1 - Plutus testing

“The overall purpose of our project is to test the Cardano node readiness for the Chang hard fork. Milestone 1 focuses on testing Plutus v3 new builtins, regression tests, wallets (hardware/software) and performance measurements. This milestone is important in the broader development of Cardano as it ensures that the Plutus v3 and the migration to v3 is smooth. For Milestone 1, we prepared the tests for Plutus v3, inheriting the base framework from Antaeus repository. We also prepared a separate tests dashboard to show all the Plutus v3 tests. Ledger Nano S hardware wallet and several software wallet were also tested with several testing scenarios ranging from normal transactions to governance functions. To support DApps for smooth migration to Plutus v3, we also prepared a comprehensive migration guide, which was widely shared in the communications. During testing, some bugs were found which were promptly reported to the respective development teams. Under the scope of the milestone, we were able to successfully cover the expected tests defined on the scope of work, and are proud of the work done.”

#### Milestone 2: Governance Actions Load Testing

“The overall purpose of our project is to test the Cardano node readiness for the Chang hard fork. Milestone 2 focuses on load testing governance actions within the Cardano network.

For Milestone 2, we implemented and observed scenarios involving multiple votes on various governance action proposals. Three distinct scenarios were tested: a majority vote leading to the enactment of one proposal, an equal vote leading to the enactment of the first proposal, and insufficient votes leading to no enactment. These tests confirmed the system's ability to accurately process and enact governance decisions based on the voting outcomes.

This milestone validates the Cardano network's stability and governance capabilities. By validating the voting and proposal mechanisms under different conditions, we ensure that the network can efficiently handle governance actions. This contributes to improved network security, stability, and the overall reliability of the Cardano community's decision-making processes.”

#### Milestone 3 - Drep, Votes, Delegation Negative testing

“The overall purpose of our project is to test the Cardano node readiness for the Chang hard fork. Milestone 3 is centered on testing various scenarios related to DReps, voting, and delegation processes.

In Milestone 3, we implemented and validated scenarios involving DReps and vote delegation. The tests included generating DRep IDs, enforcing single delegation, verifying stake registration requirements for delegation, preventing multiple DRep registrations, and testing the retirement process for DReps. Each test confirmed the correct behavior of the network's governance mechanisms, such as ensuring an ADA holder cannot delegate to multiple DReps and that only registered DReps can retire.

This milestone contributes significantly to the Cardano network by ensuring the accuracy and security of its governance and delegation processes. By validating these critical functions, we ensure the network's ability to manage decentralized voting and delegation efficiently, thereby improving overall network security, stability, and trust within the Cardano community.”

#### Milestone 4 - DApp Testing (use case: NFT Marketplace)

“The overall purpose of our project is to test the Cardano node readiness for the Chang hard fork. Milestone 4 focuses on DApp testing with use-case DApp as Cardano Marketplace. It focuses on the integration of PlutusV3 with existing marketplace decentralized applications (DApps) initially developed using PlutusV2. This milestone is crucial for the broader testing of Cardano, as it ensures that upgrades to the smart contract platform do not disrupt existing applications and that new features are utilized effectively.

In Milestone 4, we conducted extensive tests to assess the compatibility and performance of PlutusV3 in the context of marketplace DApps. This included verifying the functionality of buy, sell, and mint operations using updated reference scripts and documenting computational costs and associated fees. Benchmark tests were performed to evaluate the performance improvements of PlutusV3, and compliance with CIP-69 standards was also confirmed.

This milestone contributes to the Cardano network by ensuring that the transition to PlutusV3 is smooth and beneficial for DApp developers and users. By validating the integration and performance of new smart contract features, we validate the overall functionality, efficiency, and scalability of the Cardano ecosystem, contributing to a more robust platform for future developments and innovations.”

#### Milestone 5: Mass Delegate-to-Abstain Testing

“The overall purpose of our project is to test the Cardano node readiness for the Chang hard fork. Milestone 5 focuses on testing the Cardano network's ability to handle mass delegation to abstain from voting. This milestone is important in the broader development of Cardano as it ensures that the network can manage large-scale voting behaviors and still function smoothly.&#x20;

For Milestone 5, we tested a scenario where a large majority of ADA holders delegated their voting power to abstain. We conducted tests with 1,000 and 10,000 wallets, where 99% of ADA holders chose to abstain. Despite this, the governance action to update the constitutional committee was successfully ratified by the remaining DReps and SPOs. These tests confirmed that the network could handle extensive abstention while still processing governance actions accurately.&#x20;

This milestone validates the Cardano network by proving its capacity to manage large-scale delegation behaviors without compromising functionality. Ensuring that the network can handle mass abstention improves its stability and reliability, contributing to a more secure and efficient governance process for the Cardano community.”

#### Milestone 6 - Guardrails Testing

“The overall purpose of our project is to test the Cardano node readiness for the Chang hard fork. Milestone 6 focuses on testing the guard rails scripts and the governance actions with a gov-cli utility. This milestone is important in the broader development of Cardano as it ensures that the guard rails are properly enforced.

For Milestone 6, we prepared the tests for the guard rails that are merged to cardano-node-tests so that it can be executed at any time. The tests dashboard also now includes the guard rails tests. Further, we prepare a Python utility called ‘gov-cli’ to easily compose and test the governance actions for the community. This utility is publicly accessible on the PyPi repository. Further, we have prepared the documentation for the utility with several recipes to get started.”

#### Milestone 7 - Issue Management

“The overall purpose of our project is to test the Cardano node readiness for the Chang hard fork. Milestone 7 focuses on monitoring the core repositories: cardano-node, cardano-api and cardano-cli for the user reported Github issues. This milestone is important from the perspective that no critical user reported bug is left un-triaged and the critical bugs are brought to the attention of the respective teams. For Milestone 7, we monitored the new issue reports on the core repositories daily to triage to find out the reproducibility and severity of the bugs. In the process, we ourselves raised several additional bugs as well. During the scoped time, there were several issues reported but no critical labeled issues were found that would impact the Conway era functionalities.”

### EMURGO: Education & Wallet Upgrades

EMURGO completed key milestones for the Yoroi Wallet and Cardano Serialization Library, enabling better user interaction in the Conway era and upgrading key functionalities to support CIP-1694.

#### Milestone 1 & 2: Cardano Serialization Library & Yoroi Extension Wallet

“EMURGO has completed all the development and testing required to upgrade the CSL to support the changes introduced in Cardano's Conway era, including the distributed governance model described within CIP-1694. Further incremental beta releases will also enable user-based testing via the SanchoNet governance test network.”

“EMURGO has upgraded Yoroi Extension Wallet (Desktop) to support Cardano's Conway era, enabling users a smooth transition to the post-Chang hard fork. This deliverable also includes a beta release via Yoroi Nightly to allow connectivity to the SanchoNet governance test network, and the extension of Yoroi to support the CIP-95 standard.”

#### Milestone 1 & 2: Yoroi Mobile Wallet Upgrades

“EMURGO has upgraded Yoroi Mobile Wallet to support Cardano's Conway era, enabling users a smooth transition to the post-Chang hard fork. This deliverable includes a beta release, to allow connectivity to the SanchoNet governance test network, and the extension of Yoroi to support the CIP-95 standard.”

### Input Output Engineering (IOE): Node Development & Governance

IOE engineering teams have supported the final checks and balances required prior to initiating the community-driven Chang hard fork into the Conway era.

This includes management and completion of User story testing – results of which can be found here CIP 1694 User Story Testing [\[https://tests.cardano.intersectmbo.org/test\_results/requirements/chang\_user\_stories\_system\_tests.html#cip1694-user-stories\]](https://tests.cardano.intersectmbo.org/test_results/requirements/chang_user_stories_system_tests.html#cip1694-user-stories)

Final amendments, peer review and external audit of key scripts for governance guardrails and credentials management required for hard fork.

The wider IOE and Input Output Group communication and community teams have also supported community readiness. Contributing to communications, press releases, hosting Question and Answer sessions and during the lead up to hard fork offering, at times, 1-2-1 DApp and developer support. IOE also stood up an incident support team in conjunction with Intersect in the lead up to and over the hard fork boundary.

Aside from Chang, the IOE team have been supporting the set up and initial sessions of several Special Interest Groups at Intersect, details for these can be found on the Intersect Discord. These are designed to share technical details, gather feedback and community support on proposals currently being shaped. These proposals will ultimately be put forward to the Product and Budget committee for inclusion in future funding requests. This is aimed to democratize some of the technical information which to date has only resided within the core development teams.

#### Delivery of Identity Management for ICC

“This release contains the latest governance changes for Identity Management to allow ICC key build for Constitution. This version of the node also adds support for reference scripts in the Conway era.”

#### Delivery of Sanchonet 8.11

“This release contains the latest governance changes for SanchoNet. It has support for a new cost model for Plutus v3, plus new Plutus byte string primitives. The Constitution Committee quorum has been renamed to threshold in the CLI and a new economic parameter minFeeRefScriptCostPerByte has been added for reference scripts. This version of the node also adds support for reference scripts in the Conway era.”

### WellTyped On-Disk Storage for UTxOs&#x20;

WellTyped achieved another key milestone with the Minimal Working Version of the on-disk storage component for UTxOs. This solution will allow for higher UTxO scalability and improved performance, benefiting the broader Cardano ecosystem.

#### Milestone 5 - Minimal Working Version

“Well-Typed are developing an on-disk storage component intended to be used in Cardano to help Cardano scale to much larger numbers of accounts and UTxO sizes, while preserving good system performance.

In previous milestones we have delivered various pieces of internal functionality. In this milestone we have connected that internal functionality to the component’s public API for the first time. In particular we have filled in the part of the public API that covers basic key/value operations: lookup, insert and delete.

In addition for this milestone we have created a benchmark that simulates the UTxO workload (using the new public APIs for lookup, insert and delete) and measures the throughput. This benchmark will be used during the project to guide our work to improve performance, and at the end of the project to demonstrate whether the performance targets have been met.”

#### Milestone 6 – Optimisation and monoidal updates

“Well-Typed are developing an on-disk data storage component intended to be used in Cardano to help Cardano scale to much larger numbers of accounts and UTxO sizes, while preserving good system performance. In previous milestones we have implemented the component’s public API, covering basic key/value operations like lookups, inserts and deletes. In addition, we created a benchmark that simulates the UTxO workload and measures the throughput.&#x20;

In this milestone, we extended the public API to support “monoidal updates”. A monoidal update can be used to update a value (e.g., increment a number) without requiring a separate operation to look up the value that already exists in the database. This is a more performant alternative to performing a lookup followed by an  insert. In addition, we implemented various optimisations to the basic key/value operations, and demonstrated benchmark results showing the project is on track to meet its performance goals.”

\
