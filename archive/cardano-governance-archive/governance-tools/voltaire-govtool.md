---
description: Overview of the Voltaire Govtool
---

# Voltaire GovTool

{% include "../../../.gitbook/includes/this-page-has-been-archived.md" %}

The Voltaire Govtool is a community tool that supports the key steps of Cardano's Governance process described in CIP1694. Govtool is part of the core governance tools.

Intersect has facilitated the bootstrapping of GovTool and supported the process to fully open source it, allowing community ownership for improvement and maintenance.

The Voltaire Govtool, together with the other core tools such as the Constitutional Committee Portal, is currently managed by the Intersect [Governance tools WG](https://intersect.gitbook.io/intersect-committees-groups/groups-overview/working-groups/governance-tools-working-group), the three existing pillars that make Govtool (Proposal Discussion, Delegation, and Voting) are developed and maintained by the WeDeliver Team, the Byron team and tested by the DQuadrand team.

## The four pillars of Govtool

The Voltaire Govtool architecture is divided into pillars, allowing the different maintainers to work with minimal dependencies on their respective applications while giving the end user one cohesive experience. This structure also allows for easier individual contribution and for easier expansion of these tools. Furthermore, because Govtool is fully open source, anyone can create their own version of Govtool, either the whole Govtool or just a pillar, making it better and then providing value back to the core tool.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-08-08 at 20.34.02.png" alt=""><figcaption></figcaption></figure>

## SanchoNet Govtool

In its first implementation, Govtool has been connected to the SanchoNet testnet allowing ADA holders to test the full governance features. The community can participate in testing on [sanchogov.tools](https://sanchogov.tools/), keep track of participation in the [participation dashboard](https://participation.sanchogov.tools/en), and track of development and feedback in the [github project](https://github.com/orgs/IntersectMBO/projects/30/views/14).

In its current implementation, SanchoNet Govtool has the following features:

* Proposal discussion
* DRep registration
* DRep delegation
  * Including delegation to Abstain and No-confidence
* Reviewing and Voting on active Governance Actions

Overall guides about the SanchoNet GovTool can be found [here](https://docs.sanchogov.tools/).
