# On-chain voting

{% include "../../../../.gitbook/includes/this-page-has-been-archived.md" %}

On-Chain Voting is the process that allows the 3 voting bodies ([DReps](../../governance-roles/delegated-representatives-dreps.md), [SPOs](../../governance-roles/stake-pool-operators-spos.md), [Constitutional Committee](../../key-terms/constitutional-committee.md)) to submit their decision about On-Chain active Governance Actions, and so allows the Cardano Community and its ADA Holders to be represented in the Governance of Cardano.

In order for a Governance Action to get ratified through On-Chain voting it needs to meet voting thresholds from some or all of the voting bodies (depending on the Governance Action Type).

<mark style="color:green;">✓ Can Vote on that Governance Action Type</mark>

<mark style="color:red;">✕ Cannot Vote on that Governance Action Type</mark>

<table><thead><tr><th width="506">Governance action type</th><th width="74">CC</th><th width="84">DReps</th><th>SPOs</th></tr></thead><tbody><tr><td>Motion of no-confidence</td><td><mark style="color:red;">✕</mark></td><td><mark style="color:green;">✓</mark></td><td><mark style="color:green;">✓</mark></td></tr><tr><td>New constitutional committee or quorum size</td><td><mark style="color:red;">✕</mark></td><td><mark style="color:green;">✓</mark></td><td><mark style="color:green;">✓</mark></td></tr><tr><td>Update to the Constitution</td><td><mark style="color:green;">✓</mark></td><td><mark style="color:green;">✓</mark></td><td><mark style="color:red;">✕</mark></td></tr><tr><td>Hard-fork initiation</td><td><mark style="color:green;">✓</mark></td><td><mark style="color:green;">✓</mark></td><td><mark style="color:green;">✓</mark></td></tr><tr><td>Protocol parameter changes</td><td><mark style="color:green;">✓</mark></td><td><mark style="color:green;">✓</mark></td><td><mark style="color:red;">✕</mark></td></tr><tr><td>Treasury withdrawal</td><td><mark style="color:green;">✓</mark></td><td><mark style="color:green;">✓</mark></td><td><mark style="color:red;">✕</mark></td></tr><tr><td>Info</td><td><mark style="color:green;">✓</mark></td><td><mark style="color:green;">✓</mark></td><td><mark style="color:green;">✓</mark></td></tr></tbody></table>

{% hint style="info" %}
On-Chain Voting can be performed through the Cardano CLI and through the Voltaire GovTool.
{% endhint %}
