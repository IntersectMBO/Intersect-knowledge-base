---
description: This voting guide is for any script base DReps
---

# Voting Guide for Script DReps

{% stepper %}
{% step %}
### Review all candidates

Review all candidates on [election.constitution.gov.tools](https://elections.constitution.gov.tools/)
{% endstep %}

{% step %}
### Select the candidates you want to vote for

Select up to 7 candidates to vote for and take note of the related code

| Candidate Name                                                                                          | Candidate Code |
| ------------------------------------------------------------------------------------------------------- | -------------- |
| [Emurgone](https://elections.constitution.gov.tools/candidateDetails/2)                                 | 2              |
| [Waldo](https://elections.constitution.gov.tools/candidateDetails/3)                                    | 3              |
| [Kevin G Mohr](https://elections.constitution.gov.tools/candidateDetails/4)                             | 4              |
| [Tingvard](https://elections.constitution.gov.tools/candidateDetails/5)                                 | 5              |
| [Cardano Constitutional Consortium](https://elections.constitution.gov.tools/candidateDetails/6)        | 6              |
| [Quality of Life World Foundation](https://elections.constitution.gov.tools/candidateDetails/9)         | 9              |
| [Cardano Lover](https://elections.constitution.gov.tools/candidateDetails/11)                           | 11             |
| [FutureProduct LLC dba Futurism Products](https://elections.constitution.gov.tools/candidateDetails/12) | 12             |
| [Cardano Atlantic Council](https://elections.constitution.gov.tools/candidateDetails/13)                | 13             |
| [Cardano Ethical Oversight (CEO)](https://elections.constitution.gov.tools/candidateDetails/14)         | 14             |
| [KtorZ](https://elections.constitution.gov.tools/candidateDetails/15)                                   | 15             |
| [phil\_uplc](https://elections.constitution.gov.tools/candidateDetails/16)                              | 16             |
| [Eastern Cardano Council](https://elections.constitution.gov.tools/candidateDetails/17)                 | 17             |
| [Adara Consortium](https://elections.constitution.gov.tools/candidateDetails/18)                        | 18             |
| [Cardano Japan Council](https://elections.constitution.gov.tools/candidateDetails/19)                   | 19             |
| [Wanchain](https://elections.constitution.gov.tools/candidateDetails/20)                                | 20             |
| [STORM Partners](https://elections.constitution.gov.tools/candidateDetails/21)                          | 21             |
| [SIDAN Lab](https://elections.constitution.gov.tools/candidateDetails/22)                               | 22             |
| [Ace Alliance](https://elections.constitution.gov.tools/candidateDetails/23)                            | 23             |
{% endstep %}

{% step %}
### Add your selected candidates code in the metadata format (using metadatum label `11113`)

<pre><code><strong>"11113" : {
</strong><strong>    "action": "cast_vote",
</strong>    "data": {
                "event": "CC-Elections-2025",
                "category": "CATEGORY_E794",
                "proposal": "0ae97786-d17b-4f96-84af-979ff9c0b276",
                "id": "2a9b76c3-9e84-4c4b-92bb-0184d4407f82",
                "walletType": "CARDANO",
                "network": "MAIN",
                "votes": [Candidates codes]
        }
}
</code></pre>

example

```
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
```
{% endstep %}

{% step %}
### Submit a transaction with the metadata file on-chain

Ensuring that your DRep script credenial witnesses the transaction

* [https://developers.cardano.org/docs/transaction-metadata/](https://developers.cardano.org/docs/transaction-metadata/)
* [https://www.youtube.com/watch?v=OPH8vCfjQrY](https://www.youtube.com/watch?v=OPH8vCfjQrY)
{% endstep %}
{% endstepper %}
