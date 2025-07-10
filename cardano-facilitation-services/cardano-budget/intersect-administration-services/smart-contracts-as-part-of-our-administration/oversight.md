# Oversight

## Oversight Committees

Each Treasury Reserve Contract can, as needed, be permissioned independently. Each action outlined above is subject to a required multi-signature to enact. These actions can also be permissioned individually or in groupings. As stated, the Vendor Contracts associated with a Treasury Contract inherit these permissions. Permissions can only be set when creating the Treasury Contract.\


<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdcKPNJf21VmzYsDYGC8FqMhi5jzFKhmxXsrBLuFyAb9QDYnxva-6VnOQVafCYZ8erR1rEzpKfTkgkB-sMnmvexIhmyNAeQbC0_wFhCftDofCNXBPjLXwwkuQFKLK1tuj9h_tJlPQ?key=5CTbYNvoouuip-dWreQBqg" alt=""><figcaption><p>Figure 4. Smart contracts and multi-signatures</p></figcaption></figure>

As the administrator, Intersect may legally require sole accountability for specific actions, such as Pause and Resume; however, Intersect, as practically possible and feasible, will continue to investigate the decentralization of additional controls for future implementations. Additional keys may be added for redundancy.&#x20;

As mentioned previously, the oversight is a check and balance on Intersect's administrative duties rather than a hands-on vendor of proposal management. All of the smart contract permissions require Intersect to initiate the action through its various key configurations, and then the oversight provides a check and balance. Actions initiated by oversight members fail the conditions of the permission, which means oversight members cannot unilaterally make changes to Intersect-administered contracts.

Ultimately, when designing oversight committee permissions, a balance must be struck between legal requirements, functionality, simplicity, and scalability.

## Smart Contract Permission Rationale

Initially, the smart contract permissions – Fund, Modify, Disperse, and Reorganize – will require additional signatures from the oversight committees before being used by Intersect. Effective oversight ensures that Intersect acts appropriately as an administrator, with checks and balances, rather than direct oversight of individual proposals.

This ensures that Intersect only creates smart contracts for vendors and proposals that  DReps have approved in the corresponding info and governance actions. Multi-signatories will be required to initially fund these smart contracts. Oversight also protects proposal benefits or outcomes from diminishing over time due to poor change control or modifications to vendor contracts. Modify controls also requires oversight.&#x20;

Secondly, should Intersect be required to use the Disperse or Reorganise action, multiple signatories will be needed to approve such an action. The process will ensure that appropriate reason and rationale are provided and that Intersect is not acting unilaterally.&#x20;

The remaining smart contract permissions currently need to reside with Intersect as the administrator to ensure that the liability of Intersect and the Oversight Committee is managed appropriately. Additional rationale and explanation are provided below.

* **Fund** - This permission allows the creation of a Vendor Contract. Oversight ensures that this Vendor Contract aligns with the original scope and value of the DRep-approved governance action. Intersect initiates the action as the administrator, which is then cross-checked and approved by oversight.&#x20;
* **Modify** - This permits a change to a Vendor Contract. Oversight ensures that any modified data is correct, consistent and that explanations have been attached as metadata . Intersect initiates a change request as the administrator, and then it is approved by oversight. The vendor must also sign a consent form to proceed with this action.&#x20;
* **Disburse** - This action allows funds to be removed from a smart contract. If required, this action is initiated by Intersect as the administrator but requires approval from oversight before it is enacted.&#x20;
* **Pause** and **Resume** - Following off-chain processes to verify the completeness of milestones and delivery, Intersect, at its discretion, may pause and resume vendor payments as necessary. Where applicable, rationale can be provided as metadata.
* **SweepTreasury** - This action is also enacted via a configurable timeout at an agreed-upon period after the treasury reserve contract has been completed. However, as the administrator, Intersect can undertake this action sooner should the need arise. It is permissioned at a higher level due to the potential effect it may have, effectively ensuring it is operated by two-person control to prevent erroneous actions.
* **Reorganize** - This administrative action is undertaken by Intersect and requires oversight to checks before enactment, administering back-end management of the UTXOs which underpin the smart contracts. This permission does not affect funds.&#x20;
