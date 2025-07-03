# Milestone report Q1 2024

## Intro

Since the foundation of Intersect at the start of 2024, the Delivery Assurance team has been coordinating with a multitude of suppliers who are working to develop and maintain core Cardano. Throughout Q1 a number of important milestones have been completed, which are outlined in this summary.

Delivery Assurance forms part of Technical Operations team and coordinates continuity delivery partners to ensure the timely and reliable delivery of products, services, or projects - meeting specified requirements and expectations. You can read more about it here.&#x20;

{% hint style="info" %}
Cardano “**continuity**” is defined or referred to as any approved technical service needed to build or fix current and future areas of the Cardano blockchain. Continuity in this definition can include new developments, such as the CIP-1694 governance software, component upgrades, or testing improvements, to name a few.
{% endhint %}

***

## Summary of Q1 milestones completed

Below is a summary of the Q1 milestones completed by companies within the Continuity workstream:

### **Byron Network**

The Byron team continue to develop the GovTool WebApp by supporting the launch and running a beta testing period to discover and fix bugs and collect feedback and ideas. In Q1 the following milestone was reported complete and described by the Bryron team below:

#### Milestone 1 - Design Phase&#x20;

* Explore the new horizon of digital engagement with our latest design suite optimized for every screen:
  * Experience our homepage and dashboard designs, perfected for every device size from mobile (375px) to desktop (2560px), ensuring a responsive and seamless experience no matter where you are.&#x20;
* Innovation Unleashed:&#x20;
  * Explore the future with our governance action submission and delegation flow designs, featuring wireframes and experiments that redefine the boundaries of user experience. First milestone in the path of Governance Actions delivery.”

### **Galois**

As part of the Halo 2 project, Galois are leading the development of Zero-Knowledge Proofs (ZKPs) for future interoperability of the Cardano economy.

#### Milestone 3 - Recursive Proof Verifier

“Galois has successfully delivered Milestone 3, implementing ZK circuits that verify Plonk proofs and adding ECC Chip support for multiple curves including Pluto/Eris. These are key building blocks to fully recursive ZK proofs, enabling benefits including zk-rollups and the ability to trade between blockchains.”

### **Input Output Infrastructure**&#x20;

Input Output’s Infrastructure group is developing and testing the Cardano governance node in readiness for [CIP-1694](https://www.1694.io/) and continuity maintenance.

* CIP 1694 second fixes - this work included a large number of acceptance criteria including: the addition of bootstrap era support for Cardano node, execution of quality plan, finalizing Plutus v3 (cost model, testing), fixing of issues found interesting, updating of DB Sync & the deployment of all updates into SanchoNet. &#x20;
* Governance support - development of a prototype guardrail script as well as a prototype constitutional committee credential management script
* Repository migration - assisted with the migration of a second wave of repositories from IOG to Intersect
* Network enhancements - developments of both a Genesis Lite & Peer Sharing Solution  as well as various P2P upgrades & enhancements

### **Tweag**

Tweag are developing the Ouroboros Genesis mechanism (Genesis), which enables new nodes to join the Cardano blockchain and bootstrap themselves without relying on a trusted service. It also allows nodes to become disconnected and rejoin the network similarly. During Q1 they completed phase 3 of this work which consisted of the following Milestones:

#### Milestones 7, 9 & 10 - Limit on Patience, Genesis State Machine & Lightweight Checkpointing.

“As part of the ongoing effort towards full Cardano decentralisation, the Genesis team has delivered a number of milestones towards the implementation of Ouroboros Genesis. Tweag have now implemented the Genesis State Machine, which concerns the determination whether a node is caught up with the network or still syncing, as well as the limits on eagerness and patience”

### **WellTyped**

Welltyped are developing new Log Structured Merge Tree implementations (LSM). These will store the ledger's UTxO set on disk rather than in memory, substantially increasing the number of UTxOs—supporting many more users—while also allowing nodes to run on cheaper, lower-spec machines.

#### Milestone 3 - Core Data Structures & Algorithms

“An intermediate milestone has been completed for the Cardano LSM on-disk storage component. This milestone covers the development of the core in-memory data structures and algorithms. Progress on this component is progress towards the goal of enabling Cardano to scale to much larger ledger state sizes (e.g. comparable to Bitcoin’s \~100M UTxOs), enabling higher transaction throughput, while keeping memory (RAM) requirements acceptable.”

### **VacLabs**

VacLabs are working on ensuring the continued practical use of the Ledger and Trezor hardware wallets for the Cardano community and enhancements to support the Conway era. During Q1 they completed the following milestones:

#### Milestone 1 - Trezor Implementation

"Completed development of Trezor hardware wallet firmware and supporting libraries to support the Conway ledger era and its governance model as described within CIP-1694. Specifically, this upgrade allows smooth transition of users to the new era, as well as the ability to participate in governance by delegating to DReps. The code was tested internally, externally and pre-reviewed by Trezor, now just pending final review and release process.”

#### Milestone 2 - Ledger Implementation

“Completed development of Leder hardware wallet firmware app (and supporting libraries) to support the Conway ledger era and its governance model as described within CIP-1694. Specifically, this upgrade allows smooth transition of users to the new era for all devices, with the smaller memory devices allowing users to participate in governance by delegating to DReps. The larger memory devices (Nano X, Stax), support all actions of DReps and Constitutional Committee members. The code was tested internally, externally and has been reviewed by an external auditor appointed by Ledger. It is expected that these functionalities will be released by Ledger shortly.”

#### Milestone 3 - Supporting Tooling

“This is a highly technical milestone, to support a tweak in the ledger design. This supports some sets of data within transactions being tagged with the CBOR tag 258.

Updating this ensures a smooth transition for users from Babbage to Conway ledger era.”

***

{% hint style="info" %}
It is anticipated that a full report, like the above, will be published at the end of each quarter, as well as smaller updates through our other channels and development updates.&#x20;
{% endhint %}
