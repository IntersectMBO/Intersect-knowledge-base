---
description: >-
  This page provides guidance for vendors on their Smart Contracts and anything
  related to the Delivery Assurance processes.
---

# Smart Contract and Delivery Assurance F\&Q

## F\&Q

### Assets

1. **Can I receive payment in stablecoins or any other asset?**\
   Smart contracts are designed and can hold multiple types of digital asset. However for the most part, Intersects administration will be ada first. This means we will offer and work in ada as a first choice, with other digital assets or fiat payments only by exception.\
   \
   Currently most major stable coin providers require USD ($) to mint stable coins. In order for an administrator to offer this means that the administrator must temporarily custody treasury funds and convert to dollars before minting into stable coins. Following investigation and feasibility, future features may be developed for smart contracts for vendors to trade to a preferred asset whilst keeping approved value locked in smart contracts under a transparent delivery schedule.

### Delegating

1. **Can a Smart Contract be delegated to a DRep?**\
   No, smart contracts cannot delegate to a DRep. Smart Contracts are aligned with constitutional requirements for treasury funds, they can only be delegated to abstain. Which can be seen here:\
   [https://github.com/SundaeSwap-finance/treasury-contracts/blob/main/validators/treasury.ak#L97](https://github.com/SundaeSwap-finance/treasury-contracts/blob/main/validators/treasury.ak#L97)\
   And here;\
   [https://github.com/SundaeSwap-finance/treasury-contracts/blob/main/validators/vendor.ak#L69](https://github.com/SundaeSwap-finance/treasury-contracts/blob/main/validators/vendor.ak#L69)\

2. **Can a Smart Contract receive staking rewards?**\
   No, a smart contract cannot receive staking rewards. SPO delegation is excluded in the smart contract code, any attempt to delegate would fail. Which can be seen here:\
   [https://github.com/SundaeSwap-finance/treasury-contracts/blob/main/validators/treasury.ak#L108](https://github.com/SundaeSwap-finance/treasury-contracts/blob/main/validators/treasury.ak#L108)

### Third Party Assurance

1. **What happens if my Third Party Assurer is no longer able to review the milestones?**\
   Where practically possible Intersect asks that all vendors provide Third Party Assurance of the work. You may choose another Third Party Assurer throughout the duration of the contract, if aligned with the Delivery Assurance team. \

2. **Who is an appropriate Third Party Assurer?**\
   Considering the range of proposals under administration there is not a ‘_one size fits all_’ approach. The Third Party Assurer must be someone who is technically competent to properly review and attest that the work has been completed as per the acceptance criteria in the contract, this could be an individual or someone on behalf of an organisation. Whoever you decide to be youe Third Party Assurer must be informed and agree to do this.\
   \
   Technical or software based proposals must comply with Intersects [Technical Review Policy](https://docs.intersectmbo.org/legal/policies-and-conditions/intersect-administration-policies/technical-review-policy). Proposals which affect the core node must also consult the [Cardano constitution ](https://docs.intersectmbo.org/archive/cardano-governance-archive/cardano-constitution/read-the-cardano-constitution)for additional guardrails.\
   \
   Intersects Delivery Assurance team may look for community verified success for any project. Some of the things we will look for are:

* Are there open feedback loops with the community?
* Open issue and bug tracking, are these being acted upon in a timely manner?
* Are proposals being developed openly through test-nets or through prototyping, so progress can be verified?
* Have these prototypes and test-net versions had adoption and use?
* Does documentation exist?
* Has the community been used to help set or confirm direction (involvement in and use of Cardano Improvement Proposals, Cardano Problem Statements and other forums)?
* Are there open public communications between the vendors and community?

There are instances where Intersect will accept community based evidence, where a vendor can demonstrate that the community has been intrinsically involved in verifying the quality of the deliverables, such as the bullet points above.

### Wallets

1. **What wallet requirements do I need to be able to withdraw payments?**\
   The wallet and credentials used to withdraw funds from the PSSC vendor smart contracts will incur a standard transaction fee and need enough collateral to guarantee the withdrawal transaction. Attempting to withdraw a matured milestone payment using a wallet with 0 (zero) ada will fail.\

2. **Issue with Yoroi**\
   There is currently a known issue with Yoroi wallet and compatibility with these smart contracts. Yoroi wallet refuses to sign a transaction for which you are a required signer, but not a participant via the inputs; this means that any vendors using Yoroi will be unable to sign the transactions required for smart contracts until such time this is resolved. Vendors are asked to provide alternatives to Yoroi for the current smart contract deployments. The Yoroi team are aware of this issue and working on a fix.\

3. **I have an issue submitting a Transaction**\
   Please ensure your Ledger firmware is up to date, as outdated firmware may prevent you from submitting transactions. The Administration Portal is fully CIP-30 compliant.

_If you have any suggestions or feedback that you would like to provide to Intersect, please contact us at operational-services@intersectmbo.org._&#x20;
