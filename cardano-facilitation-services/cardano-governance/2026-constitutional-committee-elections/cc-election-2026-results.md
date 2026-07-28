# CC Election 2026 - Results

The Constitutional Committee election results have completed an independent audit and are **verified against the on-chain record**.

The four highest-ranked candidates will proceed to the on-chain Constitutional Committee update action.

## Final Results

<table><thead><tr><th width="85" align="right">Rank</th><th width="166">Candidate</th><th align="right">DRep votes</th><th width="182" align="right">Voting power</th><th align="right">Support</th></tr></thead><tbody><tr><td align="right"><strong>1</strong></td><td><strong>Philip DiSarro</strong></td><td align="right">24</td><td align="right">₳1,979,047,586.427</td><td align="right">84.86%</td></tr><tr><td align="right"><strong>2</strong></td><td><strong>Leandros BSP</strong></td><td align="right">23</td><td align="right">₳1,964,850,507.458</td><td align="right">84.26%</td></tr><tr><td align="right"><strong>3</strong></td><td><strong>Marek Mahut (deliberative.cc)</strong></td><td align="right">28</td><td align="right">₳1,370,113,895.267</td><td align="right">58.75%</td></tr><tr><td align="right"><strong>4</strong></td><td><strong>Cardano Curia</strong></td><td align="right">27</td><td align="right">₳1,288,633,576.302</td><td align="right">55.26%</td></tr><tr><td align="right">5</td><td>Asia Africa Cardano Coalition (AACC)</td><td align="right">16</td><td align="right">₳1,142,561,765.138</td><td align="right">48.99%</td></tr><tr><td align="right">6</td><td>Bosco Ribeiro</td><td align="right">10</td><td align="right">₳197,409,335.579</td><td align="right">8.47%</td></tr><tr><td align="right">7</td><td>Gbiri Oluwaseun (Olokoji)</td><td align="right">3</td><td align="right">₳121,192,048.252</td><td align="right">5.20%</td></tr><tr><td align="right">8</td><td>NexTrium Global Innovations Ltd</td><td align="right">4</td><td align="right">₳34,298,868.077</td><td align="right">1.47%</td></tr><tr><td align="right">9</td><td>Ian Njuguna</td><td align="right">2</td><td align="right">₳1,324,683.789</td><td align="right">0.06%</td></tr><tr><td align="right">10</td><td>Meek Owen</td><td align="right">0</td><td align="right">₳0</td><td align="right">0.00%</td></tr></tbody></table>

Support percentages are calculated against the total participating DRep voting power. As each DRep could select up to four candidates, voting-power totals across candidates must not be added together.

## Election Highlights

* **38 valid DRep voters**
* **0 invalid voters**
* **1 explicit abstention**
* **₳2,332,021,661.623 participating voting power**
* Voting power was calculated using the Cardano mainnet snapshot for **epoch 645**
* All submitted selections complied with the maximum of four candidates per voter

## Audit Approach

The audit independently reconstructed the election result using the finalized voting records and the epoch 645 DRep voting-power snapshot.

The process included:

1. Verifying the ballot, proposal and candidate identifiers.
2. Confirming that the published candidate set matched the committed ballot data.
3. Validating every finalized voter and submitted selection.
4. Confirming that no voter selected more than four candidates.
5. Matching each valid voter with their epoch 645 DRep voting power.
6. Independently recalculating the voting-power total and support percentage for every candidate.
7. Verifying the integrity of the source files using SHA-256 hashes and recorded file sizes.
8. Validating the Hydra close and fanout transactions and reproducing the committed on-chain result hashes.

All audit checks passed. The final status is:

> **VERIFIED: on-chain validated**

## Audit Data and On-Chain Record

* [Download the complete raw audit data](ipfs://bafybeigc77zeko6rhfgc5nzp4q474m5d4i7vt522ykhdjypv5odqplvl7m) (IPFS)
* [View the on-chain transaction containing the election results](https://cexplorer.io/address/addr1vy0ugap77dvmxuys4m7gleht74qx3e60x55zam2rqg8dddqasd8s3?tab=utxos)

The raw audit package contains the finalized vote records, voting-power snapshot, independently calculated results, source manifests, integrity hashes and on-chain validation evidence. :::
