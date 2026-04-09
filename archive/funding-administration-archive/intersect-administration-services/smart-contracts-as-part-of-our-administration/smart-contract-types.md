# Smart contract types

## Smart Contract Types

There are two types of smart contracts initially designed for managing treasury funds: a Treasury Reserve Contract (formally referred to in specifications as a Treasury Reserve Smart Contract (TRSC)) and a Vendor Contract (officially referred to in specifications as a Project-Specific Smart Contract (PSSC)). For clarity and ease, we will refer to these as Treasury Contracts and Vendor Contracts from here on.

### Treasury Contract

One or more smart contract instances on-chain will hold funds from the Cardano Treasury in a reserve account. These funds will be allocated to projects that have been approved and budgeted by the community. Funds will be held in ada. Funds can only be transferred to another Treasury Contract instance, a Vendor Contract instance, swept back to the Cardano Treasury, or moved temporarily to an exchange for conversion purposes. Each Treasury Contract will be permissioned as to who can undertake the defined actions within the smart contract. The following permissions are available within a Treasury Contract:

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdRe9DMbA46BKRfTP93QNJAnf5LontLCgptjvOXGiut-U0IvhgYOD52XldvB5salPB-zAjtmY8-70p_1TAjE9DbLjoOVri5UL1gXoYYYXufVSkRDB5XTz6_NtO6XdAWMzMbnWR0oQ?key=5CTbYNvoouuip-dWreQBqg" alt=""><figcaption><p>Figure 1: Treasury fund permissions</p></figcaption></figure>

Actions defined:

* **Fund** - Treasury Reserve contract can be used to fund a new Vendor Contract
* **Disburse** - Funds can be disbursed to arbitrary destinations (should require a high many-of-a-number (MofN) signatory, metadata rationale should be provided if used)&#x20;
* **Reorganize** - UTXOs at the treasury address can be reorganized, such as splitting or merging them
* **SweepTreasury** - Funds can be swept back to the treasury before a mandatory expiration.

Prohibited actions:

* Participation in staking
* Participation in governance

### Vendor Contract&#x20;

A Vendor Contract is one or more smart contract instances on-chain with a descriptive project name, a project code, a specified vendor, a payment schedule, and a budget. A transfer from a Treasury Contract funds the budget for a Vendor Contract. The Vendor Contract is intrinsically linked to a Treasury Contract. The permissions of a Vendor Contract are inherited from the Treasury Contract to which it is associated. The following permissions are available within a Vendor Contract.\


<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXc5k7akfyLz0SEWGIzdUUgmt8zvqtEldqUz3dGSo4M3YY_VUiL9fSW0Kc8k77hEXZUr8_Eo7DaTztsVFQc3YdG3yor7woUxKdQBFM4xbcqzwJehqz4Yacpq9OvKlf-7g21MYZm6Lg?key=5CTbYNvoouuip-dWreQBqg" alt=""><figcaption><p>Figure 2. Vendor contract permissions</p></figcaption></figure>

Actions defined:

* **Pause** - The oversight committee can pause a payment milestone (milestones can be paused independently of each other)&#x20;
* **Resume** - The oversight committee can un-pause a specific milestone&#x20;
* **Modify** - The vendor and the oversight committee can agree to modify or cancel a project, such as extending the deadline for a milestone.

Two additional actions can be either inherited from the Treasury Contract or configured during the creation of the Vendor Contract.&#x20;

* **SweepVendor** - After an expiration, all paused, unmatured funds can be swept back to the Treasury Contract (and thus back to the Cardano treasury)
* **Malformed** - If a UTXO is malformed, such as when someone sends funds to the vendor contract directly without a Plutus datum, we don't want those to be locked. Therefore, we allow them to be swept back to the treasury contract.
