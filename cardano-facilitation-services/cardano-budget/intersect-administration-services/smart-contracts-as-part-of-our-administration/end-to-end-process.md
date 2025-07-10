# End-to-end process

## Proposed Intersect end-to-end process

Within the context of the budget process to date, the following flowchart illustrates an indicative, high-level end-to-end process for smart contracting, administration, and the oversight committee.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcnyO-fsOayAJ9AoI5ubAQGXXQNSwUq-anLgtBJqIiOXPVdrvUAQ6rDI3q-sL_bve5PctpaLkgMwjyBZ9LpjX_PBScfcCsDPxcYLhFq4MYa7wk7p_VBFZJ05pW_sMYTfwQU49uv?key=5CTbYNvoouuip-dWreQBqg" alt=""><figcaption><p>Figure 5. Process overview</p></figcaption></figure>

### Bulleted explanation

1. Treasury Withdrawal governance action outlines several proposals to receive funding. Treasury Contracts and oversight committee(s) are created with permissions to control them.
2. Funds are distributed into these holding Treasury Contracts based on the success of the Treasury Withdrawal governance action.
3. Written legal contracts are pursued and agreed upon with prospective vendors off-chain (constitutionally, these are required)&#x20;
4. On-chain Vendor Contracts are created once the governance action passes, and a written legal contract is signed.&#x20;
5. Vendor commences delivery as per the schedule in the contract
6. As per the schedule, the vendor provides attestation of milestone completion to Intersect and on-chain.&#x20;
7. Intersect undertakes its role as the administrator of the oversight committee, and as permissioned, provides necessary checks and balances on the administrator.&#x20;
8. Once a milestone matures and reaches its due date, the vendor can withdraw the funds associated with that milestone. They may specify where the funds go.

### Narrative explanation

Following or during the on-chain Treasury Withdrawal governance action (1), a number of Treasury Contracts will be defined (2). These will outline the budgets or funding themes requested within the original on-chain action. This allows the partitioning of smart contract funds, assisting transparency on-chain.

Partitioning the Treasury Withdrawal has several benefits; it enhances community observability by breaking funds down into more manageable and meaningful groupings, allowing for different sets or granularities of oversight committee permissions between partitions, and improving security by not having all of the total budget in one transaction or account.&#x20;

The treasury funds stay here until Vendor Contracts are agreed upon. At this point, the funds are held in the smart contract and cannot be delegated or staked, which satisfies provisions within the constitution.&#x20;

Required by many vendors and to satisfy constitutional requirements, legal contracts (3) will be created between the CDH and the vendors whose proposals have been approved by DReps in the treasury withdrawal governance action.

Following the signing of the written legal contracts, Intersect, as the administrator, will create a back-to-back smart Vendor Contract for individual projects (4).&#x20;

At this stage, the vendor has a legally written contract that contains constitutional requirements, such as dispute resolution, and a tailored Vendor Contract for the specific project. The vendor now delivers according to the agreed-upon project schedule (5).

Defined by the milestones within a Vendor Contract, the vendor submits and attests milestone acceptance to the community and Intersect (6). Tooling will be configured to link these attestations to the on-chain milestone.

As per the permissions outlined in the Treasury Contract, which is associated with the Vendor Contract, the oversight committee will undertake oversight capabilities for Intersect, the previously described Fund, Modify, and Disperse (7). This assures that in these circumstances, Intersect cannot act unilaterally. As needed, once the ‘M-of-N’ permissions associated with these actions are met, they are enacted and recorded transparently on-chain.&#x20;

Once a milestone date has matured or reached its due date, the vendor can withdraw the specified milestone amount (8). The process ‘fails open’ to protect vendors should the oversight committee fail in any way. The vendor withdrawal is captured on-chain, so it becomes auditable.&#x20;

Timeouts are configured so that, at the end of a contract, any unclaimed or locked funds ultimately return to the Cardano Treasury, allowing on-chain governance to decide their use again.&#x20;

The Treasury Contract and permissions, the Vendor Contracts and permissions, milestones, and vendor payment withdrawals are all captured, transparent, visible, and auditable on the chain
