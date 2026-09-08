# 2025 CC Election - Results

## Results

| ID | Name                                    | Num Votes | Voting Power (Lovelace) | Voting Power (Ada) |
| -- | --------------------------------------- | --------- | ----------------------- | ------------------ |
| 13 | Cardano Atlantic Council                | 85        | 2.43709E+15             | 2,437,091,844      |
| 5  | Tingvard                                | 53        | 2.0381E+15              | 2,038,104,314      |
| 17 | Eastern Cardano Council                 | 68        | 1.79064E+15             | 1,790,636,843      |
| 15 | KtorZ                                   | 56        | 1.70629E+15             | 1,706,293,942      |
| 23 | Ace Alliance                            | 75        | 1.63353E+15             | 1,633,525,358      |
| 19 | Cardano Japan Council                   | 61        | 1.62553E+15             | 1,625,533,719      |
| 16 | phil\_uplc                              | 65        | 1.61688E+15             | 1,616,883,528      |
| 18 | Adara Consortium                        | 38        | 1.47497E+15             | 1,474,973,215      |
| 6  | Cardano Constitutional Consortium       | 45        | 969126575839273         | 969,126,576        |
| 20 | Wanchain                                | 20        | 836685545388075         | 836,685,545        |
| 22 | SIDAN Lab                               | 24        | 303866948728127         | 303,866,949        |
| 21 | STORM Partners                          | 17        | 237044646097433         | 237,044,646        |
| 14 | Cardano Ethical Oversight (CEO)         | 5         | 70337853320572          | 70,337,853         |
| 11 | Cardano Lover                           | 2         | 63659592527165          | 63,659,593         |
| 9  | Quality of Life World Foundation        | 3         | 42920172594650          | 42,920,173         |
| 4  | Kevin G Mohr                            | 3         | 1359714504097           | 1,359,715          |
| 2  | Emurgone                                | 1         | 239223502597            | 239,224            |
| 3  | Waldo                                   | 1         | 131117804227            | 131,118            |
| 12 | FutureProduct LLC dba Futurism Products | 0         | 0                       | 0                  |
|    | Total                                   | 622       | 1.68484E+16             | 16,848,414,154     |

## Audit

### Audit results

{% file src="../../../.gitbook/assets/CC Elections 2025 _ Audit _ Dquadrant.xlsx" %}

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
