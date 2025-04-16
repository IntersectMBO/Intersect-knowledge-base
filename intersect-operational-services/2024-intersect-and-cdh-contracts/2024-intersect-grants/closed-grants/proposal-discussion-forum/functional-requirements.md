# Functional requirements

## Minimum functional requirements

Must have (in no particular proirity order)

* Community members log-in via email address and/or wallet connect
* Proposal submission form - (details below)
* Proposal comments form - (details below)
* Single choice opinion Poll (Yes/No) to test consensus on a proposal
* The author of proposals should be able to edit and update their proposal
* Generates an anchor - URL that points to an off-chain JSON file containing all the information generated for a specified proposal within the Proposal Discussion Forum
* Open APIs allow other services to query proposal information alongside public endpoint with JSON structured data containing all information generated for a specified proposal&#x20;
* Proposal search and filtering
* Moderator role, to keep the forum clean (neutralizing spam and spambots, profanity check and ability to remove, hide, delete, or flag inappropriate content)&#x20;

### Minimum required fields for the Proposal Submission Form:

The list below should align with what is decided in the [governance metadata CIP. ](https://github.com/cardano-foundation/CIPs/pull/556)\


<table data-header-hidden><thead><tr><th width="205"></th><th></th></tr></thead><tbody><tr><td><strong>Form fields</strong></td><td><strong>Description</strong></td></tr><tr><td>Author ID</td><td><p>ID of author: </p><ul><li>A way for the users to identify the author of the proposal</li><li>A way to allow the platform to identify which proposal belongs to who - permissions control</li><li>Nice to have: Possibly a way to allow this platform to connect the off-chain and the on-chain author</li></ul></td></tr><tr><td>Proposal ID</td><td>Auto generated unique identifier for the proposal</td></tr><tr><td>GA Type</td><td>Indicate which type of GA this proposal represents</td></tr><tr><td>Title</td><td>The proposal name should give an indication of the Governance action that community members are trying to achieve. Keep it simple and informative.</td></tr><tr><td>Abstract</td><td>A concise summary of your proposal that provides the essential information such as the problems, implications (200-character limit including spaces)</td></tr><tr><td>Motivation/problem</td><td>Detailed description of the motivation/problem</td></tr><tr><td>Solution</td><td>The proposed solution. Explain how it is aligned with the motivation/problem.</td></tr><tr><td>Supporting links</td><td>Allows proposer to share links to different resources (e.g. PDFs, images, website/ GitHub and additional URLs).</td></tr><tr><td>Tags</td><td>Nice to have: Tags with keywords related to the proposal</td></tr></tbody></table>

### Minimum required fields for the Proposal Comment Form:

<table data-header-hidden><thead><tr><th width="211"></th><th></th></tr></thead><tbody><tr><td><strong>Form fields</strong></td><td><strong>Description</strong></td></tr><tr><td>Author ID</td><td>ID of the comment’s author</td></tr><tr><td>Comment</td><td>Once a proposal is submitted the discussion starts by users adding comments</td></tr><tr><td>Supporting links</td><td>Allow users to share additional information. e.g. PDFs, images, Website/ GitHub and additional URLs</td></tr></tbody></table>
