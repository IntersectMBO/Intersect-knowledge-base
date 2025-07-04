# 2025 CC Election - Results

## Results

{% hint style="info" %}
Currently **results are pending audit**.\
\
You can use the files and criteria below to audit the results yourself.
{% endhint %}

## Audit

### Audit files

{% file src="../../../.gitbook/assets/allVotes.json" %}

{% file src="../../../.gitbook/assets/candidateResults.json" %}

{% file src="../../../.gitbook/assets/blockchainTransactionsWithScript-basedDRepVotes.json" %}

### Constitutional Elections 2025 - Audit Criteria

1. Candidate Verification
   1. The number and identity of candidates on the ballot match the official candidate list.
   2. Candidate information (name, ID) is consistent and unaltered across all records.
2. Voter Eligibility&#x20;
   1. DRep status for each voter is verified at both the time of voting and at the end of the voting period.&#x20;
   2. Each DRep votes only up to the allowed maximum number of candidates.&#x20;
   3. The list of eligible voters is transparent and can be independently verified on-chain.
3. Vote Integrity&#x20;
   1. Every vote is cryptographically signed and signatures are validated.&#x20;
   2. Vote data—including timestamp and hash—matches the corresponding vote proofs.&#x20;
   3. Votes cast outside the permitted timeframe are excluded. i. June 12, 2025 12:00 PM (UTC) - July 2, 2025 12:00 PM (UTC)&#x20;
   4. Duplicate or replayed votes are disqualified.
4. Tally Verification&#x20;
   1. The tally for each candidate accurately reflects the count of valid, eligible votes.&#x20;
   2. The tallying process and algorithm are transparent and subject to audit.
