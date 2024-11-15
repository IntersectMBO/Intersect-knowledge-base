# Milestone report May 2024

## **Continuity May Achievements**

This report is a progress update which follows on from the previous Milestone report issued in April and provides a summary of achievements related to Cardano Continuity during May.

More information on Continuity can be found in the [Cardano Continuity Blogspot](https://www.intersectmbo.org/news/cardano-continuity).

### Byron

Byron Byron continue to develop the GovTool WebApp by supporting the launch and running a beta testing period to discover and fix bugs and collect feedback and ideas.

**During May they completed the following milestones:**

**DRep Explorer - Milestone 2 & GovTool - Support for Beta Testing Milestone 1 & 2**

“In the past month, the GovTool DevOps team focused on enhancing their infrastructure and deployment processes. Efforts were concentrated on speeding up container builds through the preparation of a base backend image, addressing and resolving Sentry errors reported in the console log, and refining the deployment workflow by overhauling the Makefile. Furthermore, the team implemented docker image versioning to improve version control and developed a Nix configuration for the frontend, aiming to streamline development and deployment activities. These tasks, pivotal for infrastructure management and DevOps, are meticulously documented and can be reviewed in detail through their respective issue links on GitHub.”

**Governance Action Submission - Milestone 2**

“We have successfully completed the development phase of the Governance Action Submission tool for both desktop and mobile platforms. This milestone was achieved through the full implementation of all features as outlined in our evolving Figma plan. This includes both the functionalities we initially planned and those we added as we gained new insights during the development process. Initial work for integrating with the Proposal Discussion Forum has been started.”

### DQuadrant

Dquadrant are focusing on developing a comprehensive testing strategy for dApps (decentralized applications). The key deliverables included the “Intersect dApps testing strategy document” and a reference document to support its implementation. These documents were designed to ensure the functionality and security of dApps through detailed testing protocol and strategic documentation. \


**During May they completed the following milestones:**

**Milestone 2 - Develop testing boilerplate frameworks**

“For Milestone 2, the Dquadrant team has updated the web-app-boilerplate repo with three PRs to set up the test boilerplate and integration with the reporting dashboard. This boilerplate enables current and future teams to add tests for govtool pillars and render the test results in the reporting dashboard.

The reporting dashboard is available here: [https://intersectmbo.github.io/govtool-test-reports/](https://intersectmbo.github.io/govtool-test-reports/)

This milestone enables current and future teams to add tests for govtool pillars and render the test results in the reporting dashboard.”

\
**Milestone 1 - Design test cases**

“For workstream 2 Milestone 1, the Dquadrant team has updated the cardano-test-plans repository with the users stories for govtool application. The user stories are available here: https://github.com/IntersectMBO/cardano-test-plans/blob/main/userStoryInventoryChangHF.md

The users stories added to this document are implemented with tests on the actual govtool repo. These tests can be seen on the reporting dashboard here:

https://intersectmbo.github.io/govtool-test-reports/govtool-frontend/”

\
**Milestones 2 - Refactor testing infrastructure**

“For workstream 2 Milestone 2, the Dquadrant team refactored the testing infrastructure to be inline with the testing strategy. This involves having all cypress tests migrated to Playwright tests and replacing Cypress test dashboard with Allure dashboard. The deployed test dashboard is made available here: https://intersectmbo.github.io/govtool-test-reports/govtool-frontend/

The tests are triggered on commits made to the test branch. This happens after the deployment of the test branch on the test infrastructure. After the deployment, the tests on frontend and the backend are triggered.

The dashboard shows the test results of all executions of the tests which represent the user stories defined on workstream 2, milestone 1. This milestones enables the team to see the regression of the tests with each new commit pushed to the repository and helps to detect and debug the bugs early.”

### Input Output Infrastructure

Input Output’s Infrastructure group is developing and testing the Cardano governance node in readiness for [CIP-1694](https://www.1694.io/) and continuity maintenance.

**Milestone 1 - Delivery of node version 8.8, 8.9 & 8.10 to Sanchonet**

&#x20;“8.8.0 - Release of the Cardano node, bring the ability to use Plutus V3 in Conway-era transactions. Plutus V3 brings several new capabilities such as a new Voting script purpose for writing voting scripts, access to governance actions in the ScriptContext, new cryptographic (BLS, Keccak256 and Blake2b-224) Plutus primitives, and more.”

“8.9 - Cardano Node 8.9.0 is a release that introduces genesis lite a.k.a bootstrap peers. This version fixes a small bug on the dynamic block forging logic and also includes some overall improvements."

“8.10 - This release contains the latest governance changes for SanchoNet. It has support for a new cost model for Plutus v3, plus new Plutus byte string primitives. The Constitution Committee quorum has been renamed to threshold in the CLI and a new economic parameter minFeeRefScriptCostPerByte has been added for reference scripts. This version of the node also adds support for reference scripts in the Conway era.”

### WellTyped

Welltyped are developing new Log Structured Merge Tree implementations (LSM). These will store the ledger's UTxO set on disk rather than in memory, substantially increasing the number of UTxOs—supporting many more users—while also allowing nodes to run on cheaper, lower-spec machines.

**During May they completed the following milestone:**

**Milestone 4  - Core I/O paths**

“Well-Typed are developing an on-disk storage component intended to be used in Cardano to help Cardano scale to much larger numbers of accounts and UTxO sizes, while preserving good system performance.&#x20;

We have recently completed an intermediate technical milestone covering several key I/O code paths within the component. Benchmarks of these code paths indicate that we are on-track to meet the overall performance targets for the component. Meeting these component performance targets will be important in the broader project that aims to enable Cardano to scale to much larger ledger states while preserving good overall system performance.”

\
