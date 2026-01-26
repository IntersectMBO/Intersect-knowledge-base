# Metadata

{% include "../../../.gitbook/includes/this-page-has-been-archived.md" %}

In the CIP-1694 Governance Metadata refers to any Off-Chain extra data submitted On-Chain to provide extra context.\
\
These include:

* **DRep Metadata:**\
  These are optionally submitted during DRep registration and should allow DRep to provide more context about themselves.
* **Governance Actions Metadata:**\
  These are optionally submitted during Governance Action submission and allow proposers to provide extra context about their Governance Action to the voters to allow them to make an informed decision.
* **Vote Metadata:**\
  These are optionally submitted when any of the voting bodies (DReps, SPOs, Constitutional Committee Members) submit their vote to provide extra context about their decision. For Constitutionally Committee Members is mandatory to submit a rationale about their vote and so to submit metadata with their vote.

Note: When submitted On-Chain, Metadata will be made of a URL where a .JSONLD file is stored and a Hash of that URL. (More info can be found here in CIP-1694)

***

Currently the structure of these metadata is in progress of being defined by the community in [CIP-100?](https://github.com/cardano-foundation/CIPs/pull/556)
