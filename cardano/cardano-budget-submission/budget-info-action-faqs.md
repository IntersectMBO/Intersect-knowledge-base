# Budget Info Action FAQs

{% hint style="warning" %}
**Important note:** Greater than 50% of active delegated DRep stake is required to pass a Budget Info Action. This does not result in the movement of any funds from the Cardano Treasury. If approved, it marks the next step toward funding, with Treasury Withdrawal governance actions required to be passed and enacted. \
\
These withdrawals require a higher threshold of over 67% DRep approval to release funds from the Cardano Treasury.
{% endhint %}

The Budget Info Action is a formal on-chain governance step that allows DReps and the Constitutional Committee to review and ratify an aggregate budget before any Treasury funds can be released. In Intersect’s case, our budget info action reflects the outcome of a community-driven process, where proposals were submitted, refined, and signaled on by DReps using the Ekklesia platform.

This action does not release funds - it authorizes the proposed allocation as a whole. Once approved, individual Treasury Withdrawal Actions must be submitted to release funds, subject to further approval and within the limits of the active Net Change Limit (NCL).



<details>

<summary>Why do we have an omnibus budget proposal instead of individual requests?</summary>

This Budget Info Action takes an omnibus approach, combining 39 proposals into a single submission for on-chain approval. It reflects the outcome of a coordinated, community-led budget process facilitated by Intersect and validated through DRep signaling on the Ekklesia platform, where over ₳3.8 billion in live stake participated.

This structure helped ensure strategic alignment with the Cardano Vision and Roadmap, reduced the risk of decision fatigue for DReps, and allowed for a clearer, more unified picture of the ecosystem’s priorities. Each included proposal was transparently published, timestamped, and stored via IPFS, and disbursements will still require individual governance actions and compliance with due diligence requirements.

That said, the omnibus format has trade-offs. It reduces voting granularity at the final approval stage, requiring DReps to accept or reject the entire bundle rather than each proposal individually. It also introduces greater coordination complexity, especially when managing different timelines and delivery models across the included proposals.

We recognize this may not be the ideal long-term model for Cardano. However, this proposal reflects verified DRep support and upholds the integrity of the signaling process. Not submitting it on-chain would mean acting on sentiment rather than signal - and would risk losing momentum at a pivotal time.

If DReps decide this format isn't suitable, we are ready to explore more modular approaches in future cycles. For now, this submission represents the most accurate and accountable expression of the community’s budget preferences.

</details>

<details>

<summary>Will this move all ₳275 million at once?</summary>

No. This Budget Info Action does not result in the immediate movement of any ADA. It represents the aggregate total of proposals that received over 50% support from participating DReps during the Ekklesia signaling process. Actual disbursement of funds will only occur through separate Treasury Withdrawal governance actions, each of which must be submitted and approved individually. These withdrawals must:

* Receive over 67% support from active voting DReps,
* Remain within the active Net Change Limit (NCL),
* Pass due diligence checks, including KYC/KYB and AML where required, and
* Be supported by a formal agreement between the delivery organization and either Intersect or Cardano Development Holdings.

Where applicable, funds will be distributed via smart contract-based escrow mechanisms, with multisig oversight involving Intersect, auditors, and other appointed parties. These contracts only become active if the corresponding Treasury Withdrawal is approved.

In short, this Budget Info Action enables a coordinated funding framework, but no funds move without a second round of on-chain approval.

</details>

{% include "../../.gitbook/includes/dropdowns.md" %}

<details>

<summary>Won’t withdrawing all this ada all at once have a negative effect on the price?</summary>

The Budget Info Action does not result in an immediate withdrawal of 275M ada from the Treasury. It simply authorizes an aggregate budget allocation.

Any actual withdrawal of funds happens gradually, through separate governance actions, and only after meeting agreed conditions such as delivery milestones and oversight checks. This process is designed to ensure responsible allocation over time - not sudden or uncontrolled releases.

</details>

<details>

<summary>How does Intersect manage funding and associated risks?</summary>

&#x20;Intersect’s role as an Administrator is to provide oversight, coordination, and accountability for the proposals that have requested it. Intersect does not manage or hold Treasury funds directly - those are released through approved governance actions and, where applicable, distributed via smart contracts or authorized accounts.

To help manage associated risks and ensure responsible use of Treasury funds, Intersect applies the following safeguards:

1. Due diligence before engagement:\
   Proposals must pass due diligence - including KYC/KYB and other verification checks - before Intersect will enter into any contractual agreement or support a Treasury Withdrawal.
2. Oversight of delivery, not custody of funds:\
   Once Treasury funds are released (following approval), Intersect’s role is to monitor progress, ensure contractual terms are being followed, and coordinate with auditors, vendors, and the community.
3. Escrow and control structures (where applicable):\
   Some proposals may use smart contracts or multisig escrows to hold and release funds. Intersect may be a signer or observer in these setups, but it does not control disbursements unilaterally.
4. Pause and recovery mechanisms:\
   If a funded proposal breaches terms, Intersect can recommend pausing disbursements or initiating recovery actions. Undisbursed funds may be returned to the Treasury if issues remain unresolved.
5. Public reporting and transparency:\
   Intersect will publish regular delivery updates and reporting for all proposals under its oversight, giving the community visibility into how funds are being used.

In short, Intersect acts as a facilitator and enabler of accountability, not a fund manager - ensuring that proposals live up to their commitments and that Treasury funding is responsibly tracked and governed.

</details>

<details>

<summary>Why did every proposal name Intersect as Administrator? Isn’t this centralizing control and increasing the risk of capture?</summary>

Intersect was named as Administrator by these proposals because it offered a structured pathway to participate in a coordinated, community-led budget process. This process included open submission, committee feedback, DRep signaling, and alignment with the Cardano roadmap, all made possible through Intersect’s support infrastructure. Participation was entirely optional, and proposers were free to submit standalone on-chain budget actions independently.

This is not about centralizing control. It is about enabling coordination in the absence of other fully operational budget facilitation alternatives. Intersect does not control funds, and its role as Administrator is limited to oversight, coordination, and transparency, not execution or decision-making authority.

Crucially:

* Intersect was requested by the proposers themselves, not assigned unilaterally
* Other entities are free to play this role in future budget cycles
* Intersect may refuse to act as Administrator if proposals do not meet due diligence or governance standards
* On-chain governance remains the final authority, with DReps and the Constitutional Committee approving all Treasury withdrawals

As the ecosystem matures, we expect to see multiple Administrators, diversifying responsibility and reducing any perceived concentration. This first round simply reflects the practical need for facilitation during a transitional governance phase.

</details>

<details>

<summary>Who checks if milestones are real or realistic? What prevents teams from gaming the system?</summary>

A multi-sig oversight body including Intersect, auditors, and independent ecosystem actors will have authority to pause payouts, demand arbitration, and ultimately return unused funds to the treasury. Intersect is currently talking a number of proven and responsible ecosystem players to fulfil this role and more news will be shared on this soon. Delivery is made public through a new dashboard, with milestone documentation and outcomes openly tracked.

</details>

<details>

<summary>What if a project goes bust or fails to deliver? What happens to the funds?</summary>

&#x20;If a funded project fails to meet its obligations or goes bust, several safeguards are in place to protect Treasury resources:

1. Pause or stop disbursements:\
   Intersect, working with oversight partners, can pause further payments if a project breaches its contract or misses key deliverables.
2. Claw-back mechanisms:\
   If funds remain undisbursed in a smart contract or designated account, they can be returned to the Treasury following a resolution process, including arbitration if needed.
3. Milestone-based or conditional payments:\
   Where applicable, funding is released in phases tied to verifiable progress. This limits exposure in the event of non-delivery.
4. Oversight and reporting:\
   Intersect and elected committees monitor delivery across proposals. Issues are flagged early to reduce risk and ensure transparency.\


In short, funds are not handed over in full at once. If a project fails, any unspent or unearned funds can be recovered or withheld, helping safeguard the Treasury and community interests.

</details>

<details>

<summary>This was all decided off-chain. Can’t that be manipulated? Why not do everything on-chain?</summary>

This budget process was an attempt to coordinate a community-driven approach using the tools and structures currently available. While we acknowledge it was imperfect and at times haphazard, it resulted in strong participation and clear signal from active DReps using live stake through the Ekklesia platform. The Ekklesia vote results were also recorded on-chain to create an immutable record.

As an ecosystem, we need to take the lessons learned from this process and work together to rebuild it - making it clearer, more inclusive, and more resilient. Moving forward, the community may well choose to make greater use of on-chain governance directly, with fewer off-chain coordination steps.

</details>

<details>

<summary> What assurance is there that Intersect won't misuse its role or become too powerful?</summary>

Intersect’s authority comes from the community. It does not control funds, cannot approve Treasury withdrawals on its own, and is accountable to both DReps and the Constitutional Committee.

Here are the key safeguards:

1. No unilateral power:\
   Intersect cannot spend Treasury funds. Every withdrawal requires a separate on-chain vote by DReps and must comply with constitutional guardrails.
2. Voluntary designation:\
   Proposers chose Intersect as Administrator for this process. They are free to select other Administrators in the future or submit proposals directly on-chain without Intersect’s involvement.
3. Transparent oversight, not control:\
   Intersect provides coordination, due diligence, and reporting. It does not act as a gatekeeper or hold exclusive rights to administer funding.
4. Subject to community checks:\
   Intersect’s actions can be scrutinized, challenged, or overridden through Cardano’s governance mechanisms. Its ongoing role depends entirely on the trust and support of the community.
5. Designed to be temporary and plural:\
   This process reflects a transitional phase. In future budget cycles, more Administrators are expected to emerge, reducing reliance on any single actor.

Intersect’s legitimacy is earned through transparency, delivery, and accountability, not through control.

</details>
