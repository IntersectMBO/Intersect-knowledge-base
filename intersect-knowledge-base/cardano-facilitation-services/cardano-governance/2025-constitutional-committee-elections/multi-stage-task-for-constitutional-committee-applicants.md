# Multi-Stage Task for Constitutional Committee Applicants

**Introduction**

This document outlines an optional three-step task for applicants to the Constitutional Committee (CC). Completing this task allows applicants to demonstrate key skills relevant to the CC role: technical proficiency in credential management (Steps 1 & 2) and the analytical ability to evaluate governance actions within Cardano's framework (Step 3), all performed in the SanchoNet environment.

**Overall Objective**

To successfully generate cold credentials, get enrolled in the SanchoNet CC, authorize hot credentials using your cold credentials, and then use the hot credentials to evaluate, vote on, and justify a position on a governance action on SanchoNet, submitting your vote rationale in the application form.



**Step 1:** Generate Cold Credentials

Purpose: To demonstrate the fundamental technical capability required to create secure cold credentials necessary for participating in Cardano governance.

Task: Generate a set of cold credentials on the SanchoNet environment. <mark style="color:orange;">As an initial part of this step, you must contact</mark> [<mark style="color:purple;">Mike Hornan</mark>](https://t.me/Hornan7) <mark style="color:orange;">to request a transfer of tAda to your wallet to cover transaction fees and necessary deposits on SanchoNet.</mark>

Method: You are free to use any method or toolset you prefer (e.g., cardano-cli, hardware wallets, or other available tools).

Outcome: Successfully created cold credentials, which will be used in Step 2.

Submission Deliverable (from this step): Prepare the required output demonstrating successful cold credential generation in preparation for Step 2.



**Step 2**: Enroll in SanchoNet CC and Authorize Hot Credentials

Purpose: To first get enrolled in the SanchoNet CC using your cold credentials, and then to demonstrate the ability to use these existing cold credentials to securely authorize hot credentials, enabling active participation like voting within the governance system.

Task:

1. <mark style="color:orange;">Using the cold credentials generated in Step 1, you must first contact</mark> [<mark style="color:purple;">Mike Hornan</mark>](https://t.me/Hornan7) <mark style="color:orange;">to request enrollment into the SanchoNet CC.</mark>
2. Once enrolled, use the cold credentials generated in Step 1 to authorize a corresponding set of hot credentials on SanchoNet. These hot credentials should be suitable for submitting votes.

Method: Utilize appropriate tools compatible with your chosen cold credential method from Step 1 for authorizing hot credentials.

Outcome: Successfully enrolled in the SanchoNet CC and subsequently authorized hot credentials linked to your cold credentials, ready for use in Step 3.



**Step 3**: Evaluate, Justify and Vote on Governance Action

Purpose: To demonstrate understanding of Cardano's governance framework, constitutional principles, and the ability to apply them by evaluating a proposal, casting a vote, and articulating the reasoning.

Context & Prerequisites for Evaluation:

A Net Change Limit (NCL) is established at 350 Million Ada and we are within the time period set by the NCL.

114 Million Ada has already been withdrawn under this NCL.

A budget corresponding to the proposal is approved.

Reference the current Cardano Blockchain Ecosystem Constitution.

Governance Action to Evaluate: "Project Nova Funding Proposal”\
`.cardano-cli conway query gov-state --testnet-magic 4 | jq '.proposals[] | select(.actionId.txId == "931a13c62bd2645feaff143302170b41a49dd3bc9527bee00b3e646fbd50ca41" and .actionId.govActionIx == 0)'`

Task:

Evaluate: Assess if the "Project Nova Funding Proposal" is constitutional or unconstitutional, based solely on the provided prerequisites.

Vote: Use the hot credentials authorized in Step 2 to cast your vote (Constitutional/Unconstitutional/Abstain) for this proposal on the SanchoNet environment.

Justify: Write a clear rationale explaining your constitutionality decision.

**Submission Deliverable (from this step)**: Submit a copy of your vote rationale in the application form. Use CIP-136 Governance Metadata standard.

***

Resources

* [CC Credential Manager instructions](https://credential-manager.readthedocs.io/en/latest/)
* [Cardano Governance: Credential Manager & Constitutional Committee Workshops](https://youtube.com/playlist?list=PLWYf5eQbRdbUPdt9UT-Vjhi6b840WSIWg\&si=HjJp19azfk1x_jR1)
* [SanchoNet tutorials](https://github.com/Hornan7/SanchoNet-Tutorials)
* [Cardano Blockchain Ecosystem Constitution](https://constitution.gov.tools/en/constitution)
* [CIP-136 Governance Metadata Standard](https://cips.cardano.org/cip/CIP-0136)

Disclaimer

The "Project Nova Funding Proposal" is purely hypothetical, designed for this task. It does not reflect any actual Cardano proposal or plan.

\
