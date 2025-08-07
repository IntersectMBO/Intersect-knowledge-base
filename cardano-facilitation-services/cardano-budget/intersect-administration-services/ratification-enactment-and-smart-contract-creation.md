# Ratification, Enactment, and Smart Contracts Creation

## Ratification and Enactment

Treasury withdrawal governance actions go through three stages before any funds get moved: proposal, ratification, and enactment. These treasury withdrawal actions are much like other on-chain governance actions, such as a hard fork. Action votes are only counted at an epoch boundary. Should they choose, this allows voters to change their vote before voting ends.

At each epoch boundary, the treasury withdrawal action is counted; should it meet the ratification threshold criteria of 67% and be found constitutional by the constitutional committee, it will change state to Ratified. At this stage, it has officially passed, and voting will cease on the governance action. However, another epoch still needs to pass before it moves into a state of Enactment; it is only on this boundary that any funds are transferred from the Treasury to the stake account specified within the governance action.&#x20;

Most explorers have features showing when epoch boundaries are and the status of any governance action.&#x20;

## Explorers and Differing Statistics

When looking at governance actions on Cardano, different tools show different percentages of support or voting power, all within a range of \~5%. This can be confusing, especially when actions like treasury withdrawals require 67% support to pass.

_Note: The source of truth for voting power calculations is Cardano nodes. All other tools displaying voting power are estimating._

There are two main reference points tools use when calculating voting power for DReps, and both are valid. They just serve different purposes:

* Live Stake (Dynamic)\
  This reflects ongoing, real-time changes in delegated stake. As wallets delegate or move funds, the total stake behind each DRep can shift, even during an ongoing vote. It is also harder to track accurately because of frequent changes.
* Epoch Boundary Stake (Stable)\
  This is the official snapshot taken at the end of each epoch. It’s the baseline used for the entire next epoch, and this is what actually counts in governance decisions.

Tools generally converge on the exact numbers once the epoch boundary is reached. Until then, they may differ based on what data they prioritize or how they handle confident choices (like abstaining and not voting).

**Summary**

* Different tools use either a live stake or an epoch boundary stake.
* The epoch boundary stake is the official reference used to determine vote outcomes.
* Percentages might look different mid-epoch, but they converge at the end of the epoch.
* Always be cautious when interpreting voting results in real time, especially for critical governance actions.

## KYC/KYB & Contract Signing&#x20;

Shortly after any treasury withdrawal action becomes ratified, the procurement team at Intersect will reach out to the proposal owner and begin formal proceedings to sign a traditional written legal contract. The procurement team will also ensure the required Know-Your-Customer (KYC) or Know-Your-Business (KYB) has been completed, following our [Due Diligence Policy](https://docs.intersectmbo.org/legal/policies-and-conditions/intersect-administration-policies/due-diligence-policy). These checks and contract signing are a necessity; failure to meet either of these due to legitimate concerns may, unfortunately, result in Intersect being unable to act as a proposals administrator.&#x20;

The nature of these steps means it is hard to articulate an exact timeframe for them to be completed by. Intersect has begun both of these steps well in advance over the last weeks and months with proposal vendors in order to expedite this as much as possible.&#x20;

Legally, at this point in tim, the delivery can begin.&#x20;

## Smart Contract Deployment

On completion of the above steps, Intersect will initiate the deployment of a vendor smart contract. This will detail the legal contract milestones and payments on-chain.

As per our previous blogs, smart contracts are required to be signed by Intersect, our independent oversight committee, and the vendor. Given the timing on Cardano, these must be initiated and signatures must be gathered within 36 hours, else the smart contract initiation process has to start again. As administrator, Intersect will coordinate this process and work diligently with all parties to ensure the prompt creation of vendor smart contracts.&#x20;

Smart contracts will transparently show all milestones, the deliverables, and payment dates associated with these. Look back at our previous blog series to see more details on this: [Smart Contract Tooling: What’s available and who's it for?](https://www.intersectmbo.org/news/smart-contract-tooling-whats-available-and-whos-it-for) And [Automating Accountability: Cardano’s Smart Contract Framework](https://www.intersectmbo.org/news/automating-accountability-cardanos-smart-contract-framework).

Only once these three steps have been completed do we say a proposal is now entirely in delivery and under Intersects' administration. It has passed the required on-chain threshold criteria, a legal contract is in place to satisfy constitutional needs, and a smart contract has been deployed for transparency to the community.&#x20;
