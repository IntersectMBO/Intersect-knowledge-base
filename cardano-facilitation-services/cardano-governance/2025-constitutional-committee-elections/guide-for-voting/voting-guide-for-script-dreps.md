---
description: This voting guide is for any script base DReps
---

# Voting Guide for Script DReps

{% hint style="info" %}
**Rules to keep in mind**

* Voting will close on the 2nd of July at 12PM UTC
* Votes can't be changed, so if more than one vote is submitted only the first one will be counted
{% endhint %}

{% stepper %}
{% step %}
#### Review all candidates

Review all candidates on [election.constitution.gov.tools](https://elections.constitution.gov.tools/)
{% endstep %}

{% step %}
#### Select the candidates you want to vote for

Select up to 7 candidates to vote for and take note of the related id

| Candidate Name                                                                                          | Candidate id |
| ------------------------------------------------------------------------------------------------------- | ------------ |
| [Emurgone](https://elections.constitution.gov.tools/candidateDetails/2)                                 | 2            |
| [Waldo](https://elections.constitution.gov.tools/candidateDetails/3)                                    | 3            |
| [Kevin G Mohr](https://elections.constitution.gov.tools/candidateDetails/4)                             | 4            |
| [Tingvard](https://elections.constitution.gov.tools/candidateDetails/5)                                 | 5            |
| [Cardano Constitutional Consortium](https://elections.constitution.gov.tools/candidateDetails/6)        | 6            |
| [Quality of Life World Foundation](https://elections.constitution.gov.tools/candidateDetails/9)         | 9            |
| [Cardano Lover](https://elections.constitution.gov.tools/candidateDetails/11)                           | 11           |
| [FutureProduct LLC dba Futurism Products](https://elections.constitution.gov.tools/candidateDetails/12) | 12           |
| [Cardano Atlantic Council](https://elections.constitution.gov.tools/candidateDetails/13)                | 13           |
| [Cardano Ethical Oversight (CEO)](https://elections.constitution.gov.tools/candidateDetails/14)         | 14           |
| [KtorZ](https://elections.constitution.gov.tools/candidateDetails/15)                                   | 15           |
| [phil\_uplc](https://elections.constitution.gov.tools/candidateDetails/16)                              | 16           |
| [Eastern Cardano Council](https://elections.constitution.gov.tools/candidateDetails/17)                 | 17           |
| [Adara Consortium](https://elections.constitution.gov.tools/candidateDetails/18)                        | 18           |
| [Cardano Japan Council](https://elections.constitution.gov.tools/candidateDetails/19)                   | 19           |
| [Wanchain](https://elections.constitution.gov.tools/candidateDetails/20)                                | 20           |
| [STORM Partners](https://elections.constitution.gov.tools/candidateDetails/21)                          | 21           |
| [SIDAN Lab](https://elections.constitution.gov.tools/candidateDetails/22)                               | 22           |
| [Ace Alliance](https://elections.constitution.gov.tools/candidateDetails/23)                            | 23           |
{% endstep %}

{% step %}
#### Add your selected candidates code in the metadata format (using metadatum label `11113`)

```json
{
    "11113" : {
        "action": "cast_vote",
        "data": {
            "event": "CC-Elections-2025",
            "category": "CATEGORY_E794",
            "proposal": "0ae97786-d17b-4f96-84af-979ff9c0b276",
            "id": "2a9b76c3-9e84-4c4b-92bb-0184d4407f82",
            "walletType": "CARDANO",
            "network": "MAIN",
            "votes": [candidate ids]
        }
    }
}
```

example

```json
{
    "11113" : {
        "action": "cast_vote",
        "data": {
            "event": "CC-Elections-2025",
            "category": "CATEGORY_E794",
            "proposal": "0ae97786-d17b-4f96-84af-979ff9c0b276",
            "id": "2a9b76c3-9e84-4c4b-92bb-0184d4407f82",
            "walletType": "CARDANO",
            "network": "MAIN",
            "votes": [2,14,22]
        }
    }
}
```
{% endstep %}

{% step %}
#### Build a transaction that'll be witnessed by your script and contains the metadata

Now we have our metadata, we will need to construct a transaction that contains the metadata and will satisfy our script to trigger.

We recommend constructing a transaction which contains a DRep Update certificate. For continuity you can supply this certificate with the same metadata as you use now.

This certificate will trigger your script to witness the transaction.

You can use a configuration like this:

```sh
cardano-cli conway governance drep update-certificate \
 --drep-script-hash $(cat my-drep-script.id) \
 --drep-metadata-url https://my-metadata.jsonld  \
 --drep-metadata-hash "0000000000000000000000000000000000000000000000000000000000000000" 
 --out-file my-update-cert-that-doesnt-change-anything.cert

cardano_cli conway transaction build \
 --tx-in $(cardano_cli conway query utxo --address $(cat my-payment.addr) --out-file  /dev/stdout | jq -r 'keys[0]') \
 --change-address $(cat my-payment.addr) \
 --certificate-file my-update-cert-that-doesnt-change-anything.cert \
 --certificate-script-file my-drep-script.json \
 --metadata-json-file my-cc-election-vote-metadata.json \
 --out-file my-cc-election-vote.unsigned
```
{% endstep %}

{% step %}
#### Sign and submit the transaction to Mainnet

See example transaction (on Preview)

* [3193ca54a934253895d61aea6cf7521e4e0a07d81883107af24a18615f279dd0](https://preview.cardanoscan.io/transaction/3193ca54a934253895d61aea6cf7521e4e0a07d81883107af24a18615f279dd0?tab=metadata)
{% endstep %}
{% endstepper %}
