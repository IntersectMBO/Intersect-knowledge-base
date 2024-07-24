# Chang timeline & dependencies

{% hint style="danger" %}
<mark style="color:red;">Any dates or windows provided in this Chang hard fork timeline are provided as</mark> <mark style="color:red;"></mark><mark style="color:red;">**estimates**</mark><mark style="color:red;">, and approved by the hard fork working group.</mark>&#x20;

<mark style="color:red;">These are based on factors such as velocity of development, testing outcomes, issues raised, and critical mass indicators.</mark>

<mark style="color:red;">Information on this page was last updated on</mark> <mark style="color:red;"></mark><mark style="color:red;">**19th July 2024**</mark>
{% endhint %}

Intersect plays the role of coordinator, as a functional servant-leader on behalf of the community and delivery teams working on hard fork activity. The functional teams within Intersect will work with the various committees, working groups, and delivery teams, relaying information here on the knowledge base. Ultimately the date for the hard fork is directly influenced by the community fulfilling the requirements detailed below.

***

## Chang Upgrades

The [Chang upgrade](https://docs.intersectmbo.org/cardano/cardano-upgrades/hard-forks/chang-upgrade) will stagger the release of governance functionality, easing adoption and onboarding for those with new or additional roles in governance.&#x20;

1. Chang Upgrade #1 Will deploy governance features to Cardano and enter the technical bootstrapping phase as described in [CIP-1694 Bootstrapping Phase](https://github.com/cardano-foundation/CIPs/blob/master/CIP-1694/README.md#bootstrapping-phase)
2. Chang Upgrade #2 Moves CIP-1694 out of technical bootstrapping phase and unlocks the final features of on-chain governance including DRep participation and all governance actions

Further information on [CIP-1694](https://www.1694.io/) and the interim bootstrapping period is available.

***

## Chang Upgrade #1

<figure><img src="../../../.gitbook/assets/image (4).png" alt=""><figcaption><p>Chang Upgrade #1 Sequence of Events</p></figcaption></figure>

In the lead-up to Change Upgrade #1 the following sequence of events will occur, driven by community participation and adoption.&#x20;

<table><thead><tr><th width="389">Step</th><th width="163">Environment</th><th>Owner</th></tr></thead><tbody><tr><td><p>Node version 8.12 will be released</p><p>(may only be a pre-release)</p></td><td>Preview + SanchoNet</td><td>Delivery Teams</td></tr><tr><td>Benchmarking and performance testing will be conducted on node version 8.12</td><td>Performance and tracing env't</td><td>Delivery Teams</td></tr><tr><td>Node passes benchmarking and performance testing (D1) </td><td>Performance and tracing env't</td><td>Delivery Teams</td></tr><tr><td>DB-Sync QA signoff</td><td>Preview</td><td>Delivery Teams</td></tr><tr><td>Node 9.0 is Released</td><td>Preview + SanchoNet</td><td>Delivery Teams</td></tr><tr><td>Preview upgraded to 9.0 and hardforked</td><td>Preview</td><td>Delivery Teams</td></tr><tr><td>Checkpoint - resolve any critical issues outstanding on Cardano-Node (D1) </td><td>Preview</td><td>Delivery Teams</td></tr><tr><td>Upgrade Pre Prod to Node 9.0.0</td><td>Pre Prod</td><td>Delivery Teams</td></tr><tr><td>SPOs and DApps will be asked to upgrade to 9.0.0 and test on Pre-Production and Mainnet in the Babbage era (D2)</td><td>Pre-Production &#x26; Mainnet</td><td>Community </td></tr><tr><td>Parameters &#x26; final genesis file will be prepared (required for 9.1.0)</td><td>Preview</td><td>Delivery Teams</td></tr><tr><td>SPOs, Exchanges and DApps will be asked to upgrade to 9.1.0 and test on Pre-Production and Mainnet in the Babbage era (D2)</td><td>Pre-Production &#x26; Mainnet</td><td>Community</td></tr><tr><td>With Critical mass indicators met, 70% SPOs and 80% Exchange liquidity hardfork to Conway era by bumping the protocol from 8.0 to 9.0 (D3)</td><td>Pre-Production &#x26; Mainnet</td><td>Community</td></tr></tbody></table>

Steps for Chang #2 upgrade will be released after completion of Chang #1 upgrade.

***

## Cardano Environments

**Preview**: Environment to test the latest functionality before release.

**Pre-Production**: Environment that matches mainnet configuration, long-term and stable environment for final-stage integration/upgrade testing.&#x20;

**Mainnet**: Our production environment – the actual network the Cardano community uses every day.

***

## Release Forecast

The following timeframes have been provided by the core Cardano development teams based on current velocity of development, scope changes and testing outcomes.

{% hint style="warning" %}
<mark style="color:red;">The following dates are purely engineering estimates provided by the delivery teams, approved by the hard fork working group for sharing. Hard fork dates will be known once dependencies are met and the community fulfils critical mass indicators</mark>
{% endhint %}

* 8.12 - mid June
* 9.0 - mid July
* 9.1 - August

Latest release information and notes can be found here at the [cardano-node releases github](https://github.com/IntersectMBO/cardano-node/releases) page.&#x20;

***

## Hard Fork Dependencies

The above timeline indicatively shows the high-level activities and dependencies required for the Chang hard fork. These are the dependencies, as agreed by the hard fork working group, which need to be completed or at a suitable point prior to initiating the hard for combinator event for the [Chang upgrades](https://docs.intersectmbo.org/cardano/cardano-upgrades/hard-forks/chang-upgrade).&#x20;

<table><thead><tr><th width="256">Item</th><th width="322">Acceptance Criteria </th><th>Current Status</th></tr></thead><tbody><tr><td>Node 9.0</td><td>Suitable candidate released in Preview environment, to be available for community testing and upgrade</td><td>Ready</td></tr><tr><td>Dquadrant Chang Testing </td><td>Completion of testing, no major issues outstanding </td><td>In Progress</td></tr><tr><td>Tweag Guardrails Script Audit</td><td>Completion of script audit, no major issues outstanding</td><td>Completed</td></tr><tr><td>Tweag Constitutional Committee Identity Script Audit</td><td>Completion of script audit, no major issues outstanding</td><td>In Progress</td></tr><tr><td>Core Governance Tooling (GovTool, CC Portal, etc.)</td><td>Governance tools finished developement, testing and deployed across environments</td><td>In Progress</td></tr><tr><td>Major Hardware Wallet Updates (Ledger and Trezor)</td><td>Conway era development completed, tested, audited and included in offical release</td><td>In Progress</td></tr><tr><td>DRep Pioneer Programme</td><td>No major programme issues reported. 15 initial DRep Workshops scheduled (<a href="https://intersect.gitbook.io/drep-pioneer-program/upcoming-dreps-workshops">upcoming workshops</a>)</td><td>In Progress</td></tr><tr><td>Constitutional Committee Genesis File</td><td>Completed and ready for inclusion in node 9.01</td><td>In Progress</td></tr></tbody></table>

### Technical Readiness

A ‘roll-call’ from the technical teams, performance & benchmarking and issue management that all teams have signed off on the release candidate and that no high-severity issues are outstanding

| Item                                | Acceptance Criteria                                                                                                       | Current Status              |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | --------------------------- |
| Technical team checklist/roll call  | Technical checklist, attestation of quality and readiness from core delivery teams                                        | In Progress                 |
| Performance and Benchmarking        | Suitable performance and benchmarking tests completed                                                                     | In Progress                 |
| High severity issues\*              | No high-level issues outstanding on [cardano-node](https://github.com/IntersectMBO/cardano-node/issues) related to Conway | Issue reported and resolved |

\*Issues are tracked here on the [Cardano-node Github](https://github.com/IntersectMBO/cardano-node/issues) repository. Issues are marked by severity by the delivery teams. A severity 1 or 2 issue may prevent hard fork until resolved. Most lower-level severity issues will not prevent a hard fork, this is reviewed on a case-by-case basis.&#x20;

### Community readiness

Qualitative feedback and sentiment from key committees, hubs, and working groups on their readiness for the hard fork.

As well as this feedback a number of critical mass indicators need to be met in order for the community to smoothly enact a hard fork. This is primarily driven by SPOs and exchanges, although other key dependent and supportive tooling will also be monitored.&#x20;

| Area                               | Acceptance Criteria                                                   | Current Status               |
| ---------------------------------- | --------------------------------------------------------------------- | ---------------------------- |
| Hard Fork Working Group            | Poll of working group members                                         | Not Started                  |
| Parameters Committee               | Poll of committee members                                             | Not Started                  |
| Open Source Committee              | Poll of committee members                                             | Not Started                  |
| Membership and Community Committee | Poll of committee members                                             | Not Started                  |
| Civics Committee                   | Poll of committee members                                             | Not Started                  |
| Intersect Hubs                     | Poll of each membership hub                                           | Poll sent and feedback given |
| Stake-Pool Operators (SPOs)        | 75% SPOs running Node 9.01 on mainnet                                 | Not Started                  |
| Exchanges                          | Majority of exchanges by liquidity (circa 80%) running hard fork node | Not Started                  |

Node 9.0 has been released, and an attestation page for community and ecosystem readiness has been launched to update progress on dependent tooling and critical mass indicators.

{% hint style="warning" %}
<mark style="color:red;">Any dates or windows provided in this Chang hard fork timeline are provided as estimates, and approved by the hard fork working group.</mark>&#x20;

<mark style="color:red;">These are based on factors such as velocity of development, testing outcomes, critical mass indicators, and issues raised.</mark>

<mark style="color:red;">Information on this page was last updated on</mark> <mark style="color:red;"></mark><mark style="color:red;">**19th July 2024**</mark>
{% endhint %}

***

More information on the [Major Release Process](https://docs.intersectmbo.org/cardano/cardano-upgrades/major-release-process) is also available. A [frequently asked questions](https://docs.intersectmbo.org/cardano/cardano-upgrades/hard-forks/hard-fork-frequently-asked-questions) page and [Ecosystem readiness](https://docs.intersectmbo.org/cardano/cardano-upgrades/hard-forks/chang-timeline-and-dependencies/chang-upgrade-1-readiness) page related to the Chang hard fork is also being updated on the knowledge base regularly.  &#x20;

To contribute to testing or provide feedback please visit the [SanchoNet](https://sancho.network/) website, as many features are already available for testing.&#x20;

