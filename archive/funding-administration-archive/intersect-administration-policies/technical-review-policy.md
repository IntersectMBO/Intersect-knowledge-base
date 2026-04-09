# Technical Review Policy

**1. Policy title:** Technical Review Policy

**2. Version:** 1.1

**3. Effective date:** 15th June 2025

**4. Review date:** Annually, next applicable June 2026

**5. Policy owner:** Head of Operations

**6. Policy sponsor:** Intersect Executive Director&#x20;

_Updated on 15th July 2025_

***

**7. Purpose:**

* This Technical Review Policy outlines requirements, guidance where necessary, for review and technical audit of milestones (documents, designs, code, or other technical project artefacts) to ensure that the deliverables do not endanger the security, functionality, performance or long-term sustainability of the Cardano Blockchain.

**8. Scope:**

* This policy applies to any deliverable which has the potential to affect the core code responsibilities under Intersect's administration.
* Specifically, any deliverable which affects crypto primitives, ledger, or consensus rules must abide by this policy and any artefacts referenced.&#x20;
* This policy does not replace any requirements set out by the Cardano Constitution. Where applicable, this must be completed in addition to anything set out in this policy
* Where a deliverable does not affect any core code, this policy should be undertaken as best practice, where practically possible.

**9. Principles:**

* To provide support to any constitutional requirements regarding technical audit, and, where necessary, further definition.
* To ensure that deliverables do not endanger the security, functionality, performance, or long-term sustainability of the Cardano Blockchain.&#x20;
* Where deliverables do not potentially affect the security, functionality, performance, or long-term sustainability of the Cardano Blockchain; vendors should consider undertaking the practices defined to demonstrate trust and promote adoption of deliverables within the ecosystem.&#x20;

**10. Definitions:**

* **Beneficiary:** Individual and/or Company who will be receiving funds and/or entering into contractual relationships with Intersect or with CDH where Intersect is acting as its Administrator
* **Compliance:** Adhering to the terms and conditions in the DRep approved funding allocated contract.
* **Ecosystem Risk:** Where the security, functionality, performance, or long-term sustainability of the Cardano Blockchain may be affected.
* **Intersect:** Intersect serves as an Administrator within Cardano’s funding ecosystem, helping to operationalize community-approved proposals by coordinating due diligence, contracting, and on-chain disbursements. This role is grounded in the principles of transparency, decentralization, and adherence to the Cardano Constitution.
* **Technical Audit:** A Technical Audit is an independent verifiable examination of technical information undertaken by a designated capable third party, separate to the Beneficiary, ensuring full alignment with contract milestones approved by DReps.
* **Technical Review:** A Technical Review is a systematic check of technical work undertaken as part of consistent delivery assurance, ensuring full alignment with contract milestones approved by DReps.

**11. Policy statements:**

* Where applicable, all deliverables must adhere to the rules within the Cardano Engineering Handbook, including any testing or reasonable disclosure requirements.
* Where applicable, all deliverables must adhere to any policy contained within the code repositories under Intersect’s administration.&#x20;
* Prior to any mainnet integration, the following artefacts, or others reasonably requested, are expected to have been agreed in advance with Intersect or a chosen third party of Intersect, produced where practically possible and reviewed by Intersect as the administrator.
  * Functionality Tests&#x20;
  * Security Reviews
  * Code Audits
  * Performance Tests
  * Integration Functionality Tests
  * Performance Tests&#x20;
* Any deliverable which affects crypto primitives, ledger, or consensus rules must seek prior agreement on technical audit and testing prior to commencement of any deliverable.&#x20;
* Because requirements for new features may not be able to be defined in this policy in advance, any other reasonable requirement for technical testing, auditing, or security review must be met.&#x20;

_Examples_

<table><thead><tr><th width="378" valign="top">Acceptable</th><th width="379" valign="top">Unacceptable</th></tr></thead><tbody><tr><td valign="top"><p><strong>Minor Update/Merge to Core Code Repository:</strong></p><p><br></p><p>Full adherence to any repository specific documentation (example here: <a href="https://github.com/IntersectMBO/cardano-node">https://github.com/IntersectMBO/cardano-node</a>) </p><p></p><p>Full adherence to repository review and merge process</p><p></p><p>Sign off from Repository Maintainers/Owners.</p></td><td valign="top"><p><strong>Minor Update/Merge to Core Code Repository:</strong></p><p><br></p><p>Uncommented code, or code which does not adhere to the policies or practices defined within the repository in question</p><p></p><p>Non-adherence or violation of any release or releasing markdown(md) requirements or similar. <br></p><p>Vague or ambiguous statements or testing which cannot be understood, verified or easily replicated.</p></td></tr><tr><td valign="top"><p><strong>Ledger Feature Release:</strong><br></p><p>Full Node Release Testing (here: <a href="https://tests.cardano.intersectmbo.org/readme.html">https://tests.cardano.intersectmbo.org/readme.html</a>) </p><p></p><p>Full adherence to any repository specific documentation (example here: <a href="https://github.com/IntersectMBO/cardano-node">https://github.com/IntersectMBO/cardano-node</a>)<br></p><p>CICD Sign off from:</p><ul><li>Test Engineer</li></ul><ul><li>Performance Engineer<br>Site Reliability Engineer</li><li>Release Engineer</li></ul></td><td valign="top"><p><strong>Ledger Feature Release:</strong></p><p></p><p>Uncommented code, or code which does not adhere to the policies or practices defined within the repository in question</p><p></p><p>Non-adherence or violation of any release or releasing markdown(md) requirements or similar. <br></p><p>Vague or ambiguous statements or testing which cannot be understood, verified or easily replicated.</p></td></tr><tr><td valign="top"><p><strong>Full Node Version Release:</strong><br></p><p>Full Node Release Testing (here: <a href="https://tests.cardano.intersectmbo.org/readme.html">https://tests.cardano.intersectmbo.org/readme.html</a>) </p><p></p><p>Full adherence to any repository specific documentation (example here: <a href="https://github.com/IntersectMBO/cardano-node">https://github.com/IntersectMBO/cardano-node</a>)<br></p><p>CICD Sign off from:</p><ul><li>Test Engineer</li><li>Performance Engineer<br>Site Reliability Engineer</li><li>Release Engineer</li></ul></td><td valign="top"><p><strong>Full Node Version Release:</strong><br></p><p>Uncommented code, or code which does not adhere to the policies or practices defined within the repository in question</p><p></p><p>Non-adherence or violation of any release or releasing markdown(md) requirements or similar. </p><p></p><p>Non-adherence, or evidence of completion, of cardano-node-test. Or public release of results.</p><p><br></p></td></tr><tr><td valign="top"><p><strong>DApp Feature or Release:</strong></p><p></p><p>Advised to follow provided delivery assurance best practice for required technical review and or audits where required.<br></p><p>Ultimately the vendor should want to demonstrate safe, secure applications and code as this is likely to increase utilization and ultimately delivery better benefit to the community. </p><p></p><p>Vendors are encouraged to demonstrate progress and incorporate community throughout development lifecycles, through prototyping, AMAs/Q&#x26;A as well as other live sessions.<br></p></td><td valign="top"><p><strong>DApp Feature or Release:</strong></p><p></p><p>Features or applications released with no prior community engagement. </p><p></p><p>Features or applications where no feedback loops are present or available for the community. <br></p><p>Features or applications where no testing or development can be seen on testnets or through prototyping. </p><p></p><p>Ultimately Intersect cannot force a vendor to undertake certain actions, but as an Administrator we can make it clear where developers and vendors have taken all due diligence and care to develop safe, secure applications for the betterment of the ecosystem.</p></td></tr></tbody></table>

**12. Roles and responsibilities:**

**Intersect (administrator)**&#x20;

* Intersect serves as an administrator, offering guidance. Intersect can advise but not enforce or amend constitutional requirements.&#x20;
* Where possible, offer audit coordination services and guidance, ensuring the initiation of necessary technical audits and reviews for each proposal under its administration.&#x20;
* Put in place reporting mechanisms to ensure clear and timely communication, including conducting Delivery Assurance checks and promptly escalating any identified issues, discrepancies, or risks.

**Vendor**

* Responsibility for conducting any technical reviews or audits prior to commencement of deliverables, as deemed reasonable by the administrator.
* Responsible for any remediation or retesting required, as reasonably requested by Intersect, until such time as the deliverable does not endanger the security, functionality, performance, or long-term sustainability of the Cardano Blockchain.
* Responsible for reasonable disclosure to Intersect or the Security Council or community as appropriate; where practically possible, reducing the likelihood of duplicating effort, and reducing the likelihood of the risk to other deliverables. &#x20;

**13. Procedures (or referenced procedures):**

* Vendors should seek clarity and requirements prior to any proposal submissions (at the earliest opportunity).
* Proposal vendors must agree to required technical audits and reviews in advance, ahead of any contractual agreements.
* Any cost associated with a proposal's technical review or audit is the responsibility of the vendor
* Where practically possible, all test results should be shared with the administrator and, as appropriate, logged by the Security Council.&#x20;
* Where practically possible, the outcomes of testing shall be shared with the community to build evidence of quality and encourage adoption.&#x20;

**14. Monitoring and compliance:**

* **Monitoring:** Intersect, as the administrator, will monitor the completion of milestones and documentation throughout the contract lifecycle, ensuring that the appropriate technical audits and reviews are undertaken.
* **Compliance:** Compliance will be monitored by delivery assurance on a per-milestone basis. Non-compliance to a required technical audit or review risks a delay in the approval of milestones.

**15. Review and amendment:**

* To ensure the policy remains current and effective, it will be reviewed at least annually. In response to significant organizational changes or regulatory updates, the policy will be updated by the Intersect Operational Services team and approved via the Intersect Executive team as required.&#x20;

**16. Related documents/references:**

This policy should be read in conjunction with the following documents, guidelines and regulatory frameworks:

* Cardano governance and policy documents
  * [Intersect Constitution - Hard Fork & Parameters](https://docs.intersectmbo.org/cardano/cardano-governance/cardano-constitution/read-the-cardano-constitution#article-viii.-amendment-process)
  * [Security Policy](https://docs.google.com/document/d/1lQPhyTOW2yV-DM22pXXQtwXM8UXW7fLSRRWjfECUpAw/edit?tab=t.0)
  * [Intersect as an Administrator](https://docs.intersectmbo.org/cardano/cardano-budget-submission/intersect-as-an-administrator)
  * [Cardano Engineering Handbook](https://input-output-hk.github.io/cardano-engineering-handbook/)
  * [Intersect: Project Deliverable Quality Assurance](https://docs.google.com/document/u/0/d/1t9n5VtipFB0OW7E9Imze1F_H8wy8Q7661qiooyZjkjA/edit)
  * [Delivery Assurance Policy and Best Practice](delivery-assurance-process-and-best-practice-policy.md)
  * [Administration Financial Audit Policy](administration-financial-audit-policy.md)
  * Transparency Policy

\
