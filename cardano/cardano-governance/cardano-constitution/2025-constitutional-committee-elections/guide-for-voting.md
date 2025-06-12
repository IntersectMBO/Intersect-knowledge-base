---
description: Step-by-step guide for DReps to partake in the CC election.
---

# Guide for Voting

{% hint style="info" %}
<mark style="color:red;">**!IMPORTANT: Once your vote is submitted it can NOT be changed.**</mark>
{% endhint %}

{% stepper %}
{% step %}
[Review candidates.](https://elections.constitution.gov.tools/)
{% endstep %}

{% step %}
Select up to 7 candidates.
{% endstep %}

{% step %}
Click "Submit your vote".
{% endstep %}

{% step %}
#### Choose Connection Method

Select either browser wallet or CLI in the next steps.
{% endstep %}

{% step %}
{% tabs %}
{% tab title="Browser wallet" %}
Sign Vote Metadata:

* Connect hardware wallet to light wallet.
* Connect light wallet to voting app.
* Signal hardware wallet use in app.
* App prepares vote in transaction metadata.
* App asks light wallet to sign; light wallet asks hardware wallet to sign; confirm on device.
* Signature returned to app.

_Certain Hardware Wallets (e.g., Ledger Nano X/S+, Keystone via Light Wallet):_\
_Standard Light Wallets: Sign vote metadata in browser._
{% endtab %}

{% tab title="CLI" %}
#### Generate & Obtain Vote Metadata

App generates vote metadata; user downloads/copies it (JSON).

```
{
          "action": "cast_vote",
          "slot": "<insert Cardano slot number of the moment of your vote>",
		  "data": {
			  "event": "CANDIDATES_123",
			  "category": "MAIN_1",
			  "proposal": "36cfad40-29fc-4832-8d3f-ec4b795cb134",
			  "id": "d9cc067c-9f19-4bfa-86f1-d61bfce8c9e2",
			  "votedAt": "<insert Cardano slot number of the moment of your vote>",
			  "votingPower": "<insert your wallet voting power here>",
			  "timestamp": "<insert Unix timestamp of the moment of your vote, you can use: Math.floor(Date.now() / 1000)>",
			  "walletId": "<insert your wallet id>",
			  "walletType": "CARDANO",
			  "network": "MAIN",
			  "votes": [5,12,6,13,45]
		  }
        }
```

_(This path is typically for users of Trezor, older Ledger Nano S models, CLI wallets, Daedalus, or script-based methods.)_

**Reference Example:** [How to vote for Cardano ICC with the CLI](http://www.youtube.com/watch?v=OPH8vCfjQrY) by Mike Hornan.
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
{% tabs %}
{% tab title="Browser wallet" %}
Receive Vote Proof/Receipt

Receive vote proof/receipt on website.
{% endtab %}

{% tab title="CLI" %}
Create and sign transaction with metadata using wallet setup.
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
{% tabs %}
{% tab title="CLI" %}
Submit signed vote file via Ballot CLI API.
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
{% tabs %}
{% tab title="CLI" %}
Receive verifiable vote proof/receipt for on-chain verification.
{% endtab %}
{% endtabs %}
{% endstep %}
{% endstepper %}

## Supported Wallets

### Light wallets

* Eternl (latest version) ![:white\_tick:](https://a.slack-edge.com/production-standard-emoji-assets/14.0/apple-medium/2705.png)
* Lace (latest version) ![:white\_tick:](https://a.slack-edge.com/production-standard-emoji-assets/14.0/apple-medium/2705.png)
* Yoroi (latest version) ![:white\_tick:](https://a.slack-edge.com/production-standard-emoji-assets/14.0/apple-medium/2705.png)
* All other top Cardano light wallets should work too

### Hardware wallets

* Eternl + Ledger ![:white\_tick:](https://a.slack-edge.com/production-standard-emoji-assets/14.0/apple-medium/2705.png)&#x20;
* Eternl + Ledger Nano X ![:white\_tick:](https://a.slack-edge.com/production-standard-emoji-assets/14.0/apple-medium/2705.png)
* Eternl + Keystone ![:white\_tick:](https://a.slack-edge.com/production-standard-emoji-assets/14.0/apple-medium/2705.png)
* Trezor ![:x:](https://a.slack-edge.com/production-standard-emoji-assets/14.0/apple-medium/274c.png) (expected, DReps cant register with Trezor)

### Cli

* CLi ![:white\_tick:](https://a.slack-edge.com/production-standard-emoji-assets/14.0/apple-medium/2705.png)
