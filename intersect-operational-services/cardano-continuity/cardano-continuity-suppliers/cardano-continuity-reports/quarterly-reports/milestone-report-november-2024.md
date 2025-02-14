# Milestone report November 2024

### Continuity November Achievements

This report is a progress update which follows on from the previous Monthly Milestone report issued in October and provides a summary of achievements related to Cardano Continuity during the month of November.

We are excited to highlight the progress made, including milestones achieved within their target months. While reporting may sometimes be slightly delayed due to our thorough processes, this ensures that we bring you clear and accurate updates.&#x20;

All reports will be stored and accessible on the Intersect website, under [Cardano continuity | Intersect - Knowledge Base](https://docs.intersectmbo.org/cardano/cardano-continuity).  This will allow you to easily refer back to previous reports and stay updated on all developments.

### Byron: GovTool Development & Testing

Byron team are supporting the vital GovTool pillars, voting and delegation. They made significant progress in making GovTool full compliant with CIP-1694 which is currently being tested and will soon become available.

#### Govtool Pillar maintainer activities - September Support

_“In September, the GovTool project saw significant improvements focused on enhancing usability, refining governance processes, and improving system stability. The latest updates included randomizing the DRep list in the directory and improving UTxO management to prevent small, inefficient transactions. Additionally, a link to the mainnet instance was added to the testnet header for easier navigation._

_Voting features were improved by displaying ADA holder voting power and refining the descriptions and visibility of voter options. The system also addressed multiple bugs related to governance actions, modal content, and navigation issues. Test suites were enhanced with more comprehensive tests, including bootstrapping tests and guardrail script support. Infrastructure-wise, various dependencies were updated, including DBSync and CSL versions, to ensure compatibility and performance improvements. Overall, these changes contribute to an enhanced user experience, streamlined governance functionalities, and a more robust testing framework for the platform.”_

#### Govtool Pillar maintainer activities - October Support

1. _“We’re pleased to announce a series of updates across our latest releases, v1.0.20 through v1.0.23,  bringing key features and improvements to enhance your experience. Version v1.0.23, "The Protocol," focuses on refining user interface elements, with fixes for protocol parameters, voting power chip padding, and metadata management. It also introduces a 128-word limit on metadata anchors, adding efficiency to metadata validation and searches._
2. _With "The Script Power" in v1.0.22, we’ve concentrated on platform stability. This includes fixing governance action expiration dates, resolving page scroll  issues, and improving backend testing. In v1.0.21, "All That Counts," we’ve addressed important vote counting errors, ensuring accurate counting of SPO votes, ADA holder power, and governance action expirations._
3. _Finally, v1.0.20, "Language Barrier," introduces new features like the @language property in metadata to improve compatibility with dbSync, along with links to key resources on the Dashboard and Home pages. iOS users can now download metadata files seamlessly. Thank you for your ongoing feedback and support—your insights are invaluable as we continue to improve and refine the platform!”_

#### Deliverable 2 - Decouple delegation and voting to individual pillars

_“We’re excited to announce some key updates to the GovTool Pillars project, enhancing both our frontend and backend capabilities for a more seamless experience:_

1. _React Packages Development: We have developed a dedicated React packages: govtool-voting-pillar and govtool-delegation-pillar, that includes the pillar package and a set of reusable components. This will streamline frontend development and make it easier to implement and maintain a consistent UI across the project._
2. _Node.js Backend for Cardano DBSync Integration: A new backend in Node.js has been built to handle integrations with Cardano DBSync. This backend is essential for managing the voting pillar-related logic, ensuring reliable and efficient interactions with the Cardano blockchain._
3. _Comprehensive Documentation: We’ve created detailed documentation covering contribution guidelines and usage instructions. This will serve as a valuable resource for contributors and users alike, making it simpler to get started and stay aligned with the project’s standards._
4. _Voting & Delegation Pillar Integration: The voting pillar has been enhanced to better integrate with other system components, allowing for improved functionality and smoother operations within the ecosystem._&#x20;

_We believe these updates will significantly improve usability, accessibility, and developer experience. As always, your feedback is invaluable—please let us know your thoughts and suggestions as we continue to build and evolve together.”_

#### Deliverable 1 - Voting and delegation frontend refactoring

_“We are pleased to announce that significant updates have been made to our application to support the integration of the new design system. The application has been updated to meet the necessary technical requirements and includes a theme configuration to facilitate the seamless adoption of the new design system once it is approved by the customer._&#x20;

_Custom components have been replaced with standardized Material Design v2 components to enhance consistency and maintainability. Additionally, unused dependencies and components have been marked as deprecated, with plans for removal after the full transition._&#x20;

_These changes are key to aligning with modern design practices and improving the overall functionality of our application. Thank you for your continued support as we enhance our tools and systems.”_

### DQuadrant: Maintenance of GovTool&#x20;

DQuadrant team is empowering governance on the Cardano blockchain by making sure that the Governance Tools works through extensive testing. That includes expanding testing frameworks to accommodate new features, ensuring robust functionality. The latest set of features being validated includes support for all Governance Action types as defined in CIP-1694.

#### During November they completed the following milestones:

#### GovTool Maintenance - September Milestone

_“The overall purpose of our project is to test the GovTool functionalities for decentralized governance as indicated in CIP-1694. Milestone 2 focuses on maintenance of the tests by fixing the broken tests and adding new tests to address the new changes on the GovTool._

_For Milestone 2 for the month of September, over 10 PRs were created to fix the existing broken tests and to address the new features like default sort to random on DRep directory. The current state of the tests indicates 89% passing tests. The failing tests are reported and have Github issues associated with them. We’ll continue testing and adding/updating the tests as GovTool evolves._

_In Addition to GovTool testing, we also fixed the Governance action loader to use proper Guard rails script. Now with the governance action loader, all Governance actions can be loaded both as single load or bulk load.”_

#### Milestone 1 - Additional checks and refactoring

_“The overall purpose of our project is to test the GovTool functionalities for decentralized governance as indicated in CIP-1694. Milestone 1 focuses on addressing the changes required for supporting bootstrapping and full governance mode across different networks (sanchonet and preview)._

_For Milestone 1, we refactored the existing tests to include the conditional checks based on the protocol version so that appropriate GovTool interactions can be tested. Proposing Gov Actions and voting on the Gov Actions are tested and failing tests are reported as Github issues for fixes._

_This milestone validates the GovTool’s functions correctly across different networks which are on different protocol versions. This contributes to the overall effort to make decentralized governance ready post hard fork.”_

#### Milestone 2 - Maintainers role

“_The overall purpose of our project is to test the GovTool functionalities for decentralized governance as indicated in CIP-1694. Milestone 2 focuses on maintenance of the tests by fixing the broken tests and adding new tests to address the new changes on the GovTool._

_For Milestone 2 for the month of October, 9 PRs were created to fix the existing broken tests and to address the new fixes like expiry date correction of the governance actions. The current state of the tests indicates 86% passing tests. The failing tests are reported and have Github issues associated with them. This reduction from the last month is related to infrastructure related issues which are being addressed. We’ll continue testing and adding/updating the tests as GovTool evolves.”_

### Input Output Engineering

In the past month, IOE prepared for the Plomin Hard Fork (HF) by supporting the Hard Fork Working Group (HFWG) to meet requirements for safely initiating the mainnet hard fork governance action. The group has confirmed that all must-have requirements are fulfilled, and IOE has contributed to ensuring the overall readiness for this process. Plomin HF is now technically ready, pending the final governance action.

IOE also released version 10.1.3, which resolved a community-reported bug related to delegation. Following the release, IOE:

* Deployed a new version of DBSync.
* Updated nodes in Preview and PreProd environments.
* Conducted a replay of Preview and PreProd Nodes controlled by IOE to verify proper state.

#### Tweag

Tweag are developing the Ouroboros Genesis mechanism (Genesis), which enables new nodes to join the Cardano blockchain and bootstrap themselves without relying on a trusted service. It also allows nodes to become disconnected and rejoin the network similarly. Earlier this year Tweag completed Limit on Patience, Genesis State Machine & Lightweight Checkpointing.&#x20;

#### Performance Improvements

_“Performance improvements have been made to the consensus logic to ensure that Genesis logic does not impose a performance penalty on a syncing node.”_

#### Code re-audit of the Identity Management Script

_“Code re-audit of the Identity Management Script for Constitution Committee members. Tweag looks exclusively at the on-chain validation code provided by IntersectMBO. The identity management script is a set of 5 on-chain scripts. Their goal is to allow the delegation of hot and cold credential power to a set of peers instead of a unique credential. Those 5 scripts are as follows:_

* _A minting script, declined in two versions (one for hot, and one for cold credentials),_
* _producing NFTs to sit at the spending scripts addresses._
* _A certifying (cold credential) script, whose logics is delegated to its associated spending script._
* _A Cold NFT spending script, where the cold NFT sits, which dictates the full logics of the Cold credential side of the product._
* _A voting (hot credential) script, whose logics is delegated to its associated spending script._
* _A Hot NFT spending script, where the hot NFT sits, which dictates the full logics of the Hotcredential side of the product.”_

### WellTyped: On-Disk Storage for UTxOs&#x20;

WellTyped achieved another key milestone with the Minimal Working Version of the on-disk storage component for UTxOs. This solution will allow for higher UTxO scalability and improved performance, benefiting the broader Cardano ecosystem.

#### During November they completed the following milestone:

#### Milestone 8 – incremental merges and multiple writeable table handles

_“Well-Typed are developing an on-disk data storage component intended to be used in Cardano to help Cardano scale to much larger numbers of accounts and UTxO sizes, while preserving good system performance. In previous milestones we have implemented the component’s public API, covering basic key/value operations like lookups, inserts and deletes, and other features including cursors, range requests and “BLOB”s._

_In this milestone, we extended the public API to support duplicating multiple cheap copies of database tables that can be used and modified independently. We have also implemented a performance feature to dramatically reduce the worst-case latency of insert operations._

_Having support for cheap duplication will enable simplification of the Cardano consensus implementation, and also enable improved performance and reduced memory use. Limiting the worst case latency of table inserts is important for Cardano to make sure that the time to validate and forward Cardano blocks has good worst case latency. This is important because Cardano is a hard real-time system, and cannot easily tolerate high variance in the time to broadcast blocks, without loss of throughput, i.e. missing blocks.”_

### VacLabs

The team at VacLabs is upgrading Ledger and Trezor hardware wallet software to support the new functionalities of Cardano’s Conway ledger era.

#### VacLabs have completed the following milestones:

#### Milestone 3&#x20;

“_This project integrated new HW wallets functionalities in cardano-hw-cli tool which is used to connect HW wallets with cardano-cli and is also further used with Cardano SPO tooling which is important for SPOS.”_\


#### Milestone 6

“_This was the final milestone of HW wallets implementation project which enabled Conway Governance voting functionalities to Ledger & Trezor hardware wallets and cardano-hw-cli tool.”_

\
