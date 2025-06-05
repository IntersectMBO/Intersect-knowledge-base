# Cardano's treasury governance

#### The treasury and safeguards

Cardano’s budgeting process is about managing the outflow of funds from its treasury. The treasury can currently only hold ada. The inputs and outputs of the Cardano treasury include:

<figure><img src="../../../.gitbook/assets/Edu Materials_Cardano Budget Process (1).jpg" alt=""><figcaption><p>Cardano treasury inflows and outflows.</p></figcaption></figure>

To manage the treasury outflows, the Cardano Constitution establishes this hierarchy of controls:

<figure><img src="../../../.gitbook/assets/Edu Materials_Cardano Budget Process (1) (1).jpg" alt=""><figcaption><p>Controls surrounding the Cardano treasury.</p></figcaption></figure>

Each layer in this hierarchy is driven by community consensus. The product roadmap was proposed for community review as [an info action](https://gov.tools/governance_actions/56f39054758f1a3cedc1de9225d66bf270b62dfdbfbc5399f1d6d43aceffc636#0). Votes on the product roadmap show DRep alignment to technical development, and presumably funding, of those items. The NCL, budgets, and treasury withdrawals require approval by the DReps and Constitutional Committee. Community consensus through DReps and oversight of the Constitutional Committee protects the treasury from being drained unexpectedly.&#x20;

#### About the NCL

DReps must approve an NCL, protecting against excessive treasury withdrawals.

> Withdrawals from the Cardano blockchain treasury that would cause the Cardano Blockchain treasury balance to violate the then applicable net change limit shall not be permitted.
>
> Cardano Constitution, Article IV, Section 3

Only _one_ NCL can be in effect at one time. The active NCL sets the maximum amount of treasury withdrawals per period of time. Based on the below language, if an NCL for period x is 100, withdrawals during period x _cannot_ exceed 100.

> Withdrawals from the Cardano Blockchain treasury made pursuant to an approved Cardano Blockchain ecosystem budget must not exceed the net change limit for the Cardano Treasury's balance per period of time” Cardano Constitution, Guardrail TREASURY-02a (x).
>
> Cardano Constitution, Guardrails Appendix

The Constitution does leave some flexibility in defining the applicable period for the NCL. The NCL is ultimately enforced by the Constitutional Committee and not by a protocol parameter. This leaves room for the community to propose, define, and approve sensible time periods. This is illustrated with examples below.

{% hint style="info" %}
Example NCL scenarios: &#x20;



The NCL is applied from its point of approval onward and until changed:

* Jan 2030 (epoch 900), an NCL of 500m per year (73 epochs) is approved and slated to start at epoch 901.&#x20;
* Between epochs 901-974, no more than 500m ada can be withdrawn from the treasury.
* Between epochs 975-1048, no more than 500m ada can be withdrawn from the treasury.
* And so on until a new NCL is approved.



It is possible for the community to subsequently approve a smaller NCL. If treasury withdrawals have not yet been made against the previous NCL, they may no longer be possible.

* Jan 2030 (epoch 900), an NCL of 500m ada per year (73 epochs) and a budget of 400m ada are both approved.
* Feb 2030 (epoch 905), treasury withdrawals totaling 50m ada are approved.
* Mar 2030 (epoch 910), an new NCL of 200m ada per year (73 epochs), starting on epoch 915 is approved.
*   Apr 2030 (epoch 915), a treasury withdrawal for 300m ada is proposed and subsequently rejected by the Constitutional Committee because it violates the then applicable NCL.

    <figure><img src="../../../.gitbook/assets/Edu Materials_Cardano Budget Process (2).jpg" alt=""><figcaption><p>Scenario with an NCL that is smaller than the previous one, and conflicts with the existing NCL and treasury withdrawals.</p></figcaption></figure>


*   The above example’s conflict between the new NCL and treasury withdrawal could be avoided by drafting the new NCL info action so that it starts at epoch 974, after the previous NCL period is completed:

    <figure><img src="../../../.gitbook/assets/Edu Materials_Cardano Budget Process (3).jpg" alt=""><figcaption><p>Scenario with a NCL that is smaller than the previous one, but avoids conflict with the existing NCL and treasury withdrawals.</p></figcaption></figure>


{% endhint %}

#### About the budget

Once the NCL is approved, budgets can also be approved. Treasury withdrawals cannot be passed until a budget is approved. It is possible for the NCL and budget to be discussed and voted on concurrently, as long as the NCL info action expires _before_ the budget info action. The voting bodies for the budget are the DReps and the Constitutional Committee.&#x20;

The constitution requires any budget to:

* Be designated in ada.
* Specify a process to oversee the use of funds.
* Specify one or more administrators responsible for the oversight of funds.

Because any budget has a 30-day voting window, regardless of any off-chain processes, there is time for discussion, consensus building, and for ada owners to delegate to DReps who will vote according to their preferences. DReps will also be asked to approve who will receive the funds associated with the 2025 budget.&#x20;

Intersect is gathering proposals from anyone wishing to receive treasury funds, and DReps will review those proposals to help finalize the budget amount, work items, and vendors within. Each budget must specify an administrator, whose role is to oversee and orchestrate the appropriate use of the funds once disbursed from the treasury.

#### About treasury withdrawals

Treasury withdrawals, which require approval of the DReps and Constitutional Committee, are the last step and move funds from the treasury. Withdrawals specify the amount of ada and where it will be sent. In most cases, a withdrawal request will be sent to the administrator specified within the budget. Treasury withdrawals must be pursuant to an approved budget and must not exceed the current NCL.

* _To learn more about the treasury system on Cardano, see_ [_here._](https://docs.intersectmbo.org/cardano/cardano-economy/cardano-treasury)
* _To read the constitution:_ [_https://constitution.gov.tools/en/constitution_](https://constitution.gov.tools/en/constitution)
* _To better understand the on-chain governance actions, the role of DReps, and Constitutional Committee, see_[ _CIP-1694_](https://github.com/cardano-foundation/CIPs/tree/master/CIP-1694)_. The roadmap, budget, and NCL are approved via info actions. Withdrawals are approved via treasury withdrawal governance actions._

#### Treasury management philosophies

For 2025, the budget process is aligned to conservatively spending treasury funds, similar to a sovereign wealth fund that does not draw down on the principal. This is based on several community indicators that conservative treasury spend is preferred. Read more about it[ here](https://intersectmbo.org/news/understanding-committees-in-intersect-0-0).
