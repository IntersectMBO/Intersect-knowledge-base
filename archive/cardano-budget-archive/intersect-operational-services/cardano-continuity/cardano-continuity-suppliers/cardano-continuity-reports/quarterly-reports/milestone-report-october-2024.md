---
hidden: true
---

# Milestone report October 2024

## Delivery Assurance Completed Milestone Report - October 2024

### Continuity October Achievements

This report is a progress update which follows on from the previous Quarterly Milestone report issued in September and provides a summary of achievements related to Cardano Continuity during the month of October.

All reports will be stored and accessible on the Intersect website, under [Cardano continuity | Intersect - Knowledge Base](https://docs.intersectmbo.org/cardano/cardano-continuity).  This will allow you to easily refer back to previous reports and stay updated on all developments.

### Byron: GovTool Development & Testing

Byron have completed the remaining work on the GovTool WebApp, finalizing the beta testing phase and Hard Fork Product Releases. They are also continuing their work on the Cardano GovTool, which supports vital governance processes for Cardano. This contract includes; refactoring the front and back ends of the Delegation and Voting pillars, and maintaining and supporting these pillars through testing networks and mainnet phases, with an emphasis on fixing bugs and gathering feedback.

#### Govtool Pillar maintainer activities - August Support

_“I am pleased to announce that we have successfully achieved several significant milestones over the past month. Here’s a summary of our key accomplishments:_&#x20;

1. _Hard Fork Preparation and Execution: The team efficiently prepared for and executed a hard fork, demonstrating our strong commitment to technical excellence._&#x20;
2. _Initialization of Pilars: We initiated work on the Pilars project by setting up the necessary repositories, creating projects, and copying over some of the existing code._&#x20;
3. _Rebranding of GovTool: We have successfully rebranded Sanchonet GovTool to Cardano GovTool, aligning our tools with our broader strategic vision._&#x20;
4. _Pre-release of Design System: We launched the pre-release of the Design System to support Pilars, ensuring a uniform styling framework across our projects.”_

### DQuadrant: Testing Strategies & Chang Hard Fork Support&#x20;

#### Testing Strategies

DQuadrant have completed the final milestones in their contract and have made significant contributions to Cardano’s testing framework, specifically related to the governance tooling and readiness for the Chang hard fork. Their efforts to test Plutus v3 and ensure the continued functionality of decentralized applications (DApps) have been crucial.

DQuadrant are continuing to extend the testing frameworks for Cardano GovTool to accommodate new features. DQuadrant are maintaining the Cardano GovTool integrated testing and the Governance Action Loader.

#### During October they completed the following milestones:

#### Milestone 1 - Plutus Testing

_“The overall purpose of our project is to test the Cardano node readiness for the Chang hard fork. Milestone 1 focuses on testing Plutus v3 new builtins, regression tests, wallets (hardware/software) and performance measurements. This milestone is important in the broader development of Cardano as it ensures that the Plutus v3 and the migration to v3 is smooth._&#x20;

_For Milestone 1, we prepared the tests for Plutus v3, inheriting the base framework from Antaeus repository. We also prepared a separate tests dashboard to show all the Plutus v3 tests. Ledger Nano S hardware wallet and several software wallet were also tested with several testing scenarios ranging from normal transactions to governance functions. To support DApps for smooth migration to Plutus v3, we also prepared a comprehensive migration guide, which was widely shared in the communications. During testing, some bugs were found which were promptly reported to the respective development teams._

_Under the scope of the milestone, we were able to successfully cover the expected tests defined on the scope of work, and are proud of the work done.”_

#### Milestone 7 - Issues Management

_“The overall purpose of our project is to test the Cardano node readiness for the Chang hard fork. Milestone 7 focuses on monitoring the core repositories: cardano-node, cardano-api and cardano-cli for the user reported Github issues._

_This milestone is important from the perspective that no critical user reported bug is left un-triaged and the critical bugs are brought to the attention of the respective teams._\
\
_For Milestone 7, we monitored the new issue reports on the core repositories daily to triage to find out the reproducibility and severity of the bugs. In the process, we ourselves raised several additional bugs as well. During the scoped time, there were several issues reported but no critical labeled issues were found that would impact the Conway era functionalities.”_

### Galois

Galois continued their critical work on the Midnight Halo 2 project, focusing on enhancing the capabilities of Zero Knowledge Proofs (ZKPs) within the Cardano ecosystem.&#x20;

#### During October they completed their final milestone:

Milestone 5: Recursion

_“Galois has achieved full IVC recursion of ZK proofs over two cycles of curves within the Halo2 codebase: 1) The Pasta curves with the IPA commitment scheme 2) The  Pluto / Eris curves with the IPA and KZG commitment schemes This milestone completes the project of providing ZK-proof roll-up capability in the Halo2 framework. Integration of the results of all previous milestones was necessary, the culmination of a year’s worth of work.”_

### Input Output Engineering

Input Output Engineering is continuing to develop and test the Cardano governance node in readiness for [CIP-1694](https://www.1694.io/) and continuity maintenance.

### Tweag

Tweag are developing the Ouroboros Genesis mechanism (Genesis), which enables new nodes to join the Cardano blockchain and bootstrap themselves without relying on a trusted service. It also allows nodes to become disconnected and rejoin the network similarly. Earlier this year Tweag completed Limit on Patience, Genesis State Machine & Lightweight Checkpointing.&#x20;

#### During October they completed the following milestone:

#### Guardrails Script Audit - Technical Review of Constitution script

_“Tweag analyzed the validator scripts comprising Constitution script, contained in the repositoryas of commit ccebcc0. As this is a security audit we are inclined not to reveal to many details.”_

### WellTyped: On-Disk Storage for UTxOs&#x20;

WellTyped achieved another key milestone with the Minimal Working Version of the on-disk storage component for UTxOs. This solution will allow for higher UTxO scalability and improved performance, benefiting the broader Cardano ecosystem.

#### During October they completed the following milestone:

#### Milestone 7 - BLOBs and range lookups

_“Well-Typed are developing an on-disk data storage component intended to be used in Cardano to help Cardano scale to much larger numbers of accounts and UTxO sizes, while preserving good system performance. In previous milestones we have implemented the component’s public API, covering basic key/value operations like lookups, inserts and deletes._&#x20;

_In this milestone, we extended the public API to support “BLOB” storage and retrieval, range lookups and cursors. BLOBs allow storing large values efficiently, such as scripts in the UTxO. Range lookups and cursors allow efficient iteration through the contents of a table. This will be used in Cardano (once the stake-related tables are stored on disk) to implement incremental bulk queries such as aggregating the stake distribution.”_

\
