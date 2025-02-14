# Milestone report August 2024

## Delivery Assurance Completed Milestone Report - August 2024

This report is a progress update which follows on from the previous Milestone report issued in July and provides a summary of achievements related to Cardano Continuity during the month of August.

Going forward, these reports will be included in the Development Report, so please keep an eye out for those updates. Additionally, all reports will be stored and accessible on the Intersect website, under [Cardano continuity | Intersect - Knowledge Base](https://docs.intersectmbo.org/cardano/cardano-continuity).  This will allow you to easily refer back to previous reports and stay updated on all developments.

### DQuadrant

Dquadrant are focusing on developing a comprehensive testing strategy for dApps (decentralized applications). The key deliverables included the “Intersect dApps testing strategy document” and a reference document to support its implementation. These documents were designed to ensure the functionality and security of dApps through detailed testing protocol and strategic documentation.\
\
DQuadrant are also helping with the Chang Hard Fork by carrying out thorough testing, including checking old and new features in Plutus v3. The contract involves important tasks like verifying transaction costs, making sure older versions still work, and comparing the performance of Plutus v2 and v3. The testing also includes checking governance actions, wallet functions, and how the system handles different network conditions. The goal is to ensure the blockchain remains strong and effective after the upgrade, with clear documentation to back up these efforts.

#### During August they completed the following milestones:

#### Milestone 3 - Extend coverage for Proposal Discussion Forum

_“The overall purpose of our project is to test the GovTool functionalities for decentralized governance as indicated in CIP-1694. Milestone 3 focuses on testing the Proposal submission and discussion forum._&#x20;

_For Milestone 3, we created user stories for proposal submission and discussion forum and had them reviewed by the respective team manager. A total of 38 tests were written for covering the user stories covering the cases for use cases like wallet connected/disconnected states, proposal submission, proposal validation, listing, searching, accessing, filtering, searching etc. These tests confirm the system's ability of GovTool to enable users to successfully submit a draft proposal for discussion and later submit as governance action._

_This milestone validates the GovTool’s proposal submission and discussion forum’s capabilities. By validating the proposal submission and discussion mechanisms under different conditions, we ensure that the GovTool can correctly handle governance actions. This contributes to the overall effort to make decentralized governance possible for the Cardano community.”_

#### Milestone 1 - Maintenance and hosting of Governance Actions Loader

_“The overall purpose of our project is to test the GovTool functionalities for decentralized governance as indicated in CIP-1694. Milestone 1 focuses on maintaining and hosting the governance actions loader used for loading governance actions in bulk._

_For Milestone 1, we had been maintaining and hosting the governance actions loader since the beginning. It had been operational until early July. At the moment, it is not fully operational because of the dependency bug_ [_https://github.com/IntersectMBO/cardano-api/issues/594_](https://github.com/IntersectMBO/cardano-api/issues/594)  _Issue is created and fix is being prepared by the cardano-api. Once the bug is fixed on the dependency, the loader can be made operational again._

_The Governance Actions Loader is useful in loading multiple governance actions in bulk which helps in (stress) testing the GovTool. The loader internally handles the constraints of linking the correct previous governance actions and preparing valid governance actions to submit on chain. This contributes to the overall testing effort to make decentralized governance possible for the Cardano community.”_

#### Milestone 6 - Guardrails Testing

_"The overall purpose of our project is to test the Cardano node readiness for the Chang hard fork. Milestone 6 focuses on testing the guard rails scripts and the governance actions with a gov-cli utility. This milestone is important in the broader development of Cardano as it ensures that the guard rails are properly enforced._

_For Milestone 6, we prepared the tests for the guard rails that are merged to cardano-node-tests so that it can be executed at any time. The tests dashboard also now includes the guard rails tests. Further, we prepare a Python utility called ‘gov-cli’ to easily compose and test the governance actions for the community. This utility is publicly accessible on the PyPi repository. Further, we have prepared the documentation for the utility with several recipes to get started."_

### Input Output Engineering

Input Output Engineering is developing and testing the Cardano governance node in readiness for [CIP-1694](https://www.1694.io/) and continuity maintenance.

#### During August they completed the following milestones:

Over the month of August IOE engineering teams have supported the final checks and balances required prior to initiating the community-driven Chang hard fork into the Conway era.\
\
This includes management and completion of User story testing – results of which can be found here CIP 1694 User Story Testing \[[https://tests.cardano.intersectmbo.org/test\_results/requirements/chang\_user\_stories\_system\_tests.html#cip1694-user-stories](https://tests.cardano.intersectmbo.org/test_results/requirements/chang_user_stories_system_tests.html#cip1694-user-stories)].\
\
Final amendments, peer review and external audit of key scripts for governance guardrails and credentials management required for hard fork.\
\
The wider IOE and Input Output Group communication and community teams have also supported community readiness. Contributing to communications, press releases, hosting Question and Answer sessions and during the lead up to hard fork offering, at times, 1-2-1 DApp and developer support. IOE also stood up an incident support team in the lead up to and over the hard fork boundary.\
\
Aside from Chang the IOE team have been supporting the set up and initial sessions of several Special Interest Groups at Intersect, details for these can be found on the Intersect Discord. These are designed to share technical details, gather feedback and community support on proposals currently being shaped. These proposals will ultimately be put forward to the Product and Budget committee for inclusion in future funding requests. This aimed at democratising some of the technical information which to date has only resided within the core development teams.

### WellTyped

Welltyped are developing new Log Structured Merge Tree implementations (LSM). These will store the ledger's UTxO set on disk rather than in memory, substantially increasing the number of UTxOs—supporting many more users—while also allowing nodes to run on cheaper, lower-spec machines.

#### During August they completed the following milestone:

#### Milestone 6 – Optimisation and monoidal updates

_“Well-Typed are developing an on-disk data storage component intended to be used in Cardano to help Cardano scale to much larger numbers of accounts and UTxO sizes, while preserving good system performance. In previous milestones we have implemented the component’s public API, covering basic key/value operations like lookups, inserts and deletes. In addition, we created a benchmark that simulates the UTxO workload and measures the throughput._&#x20;

_In this milestone, we extended the public API to support “monoidal updates”. A monoidal update can be used to update a value (e.g., increment a number) without requiring a separate operation to look up the value that already exists in the database. This is a more performant alternative to performing a lookup followed by an  insert. In addition, we implemented various optimisations to the basic key/value operations, and demonstrated benchmark results showing the project is on track to meet its performance goals.”_
