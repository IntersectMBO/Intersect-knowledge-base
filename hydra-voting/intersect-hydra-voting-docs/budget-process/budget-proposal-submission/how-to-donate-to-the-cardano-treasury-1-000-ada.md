---
description: This page shows a guide on how to submit a donation to the Cardano treasury.
---

# How to Donate to the Cardano Treasury (1,000 ada)

{% hint style="danger" %}
## Disclaimer

This guide is provided by Intersect strictly for informational purposes and does not constitute financial, legal, or technical advice, nor does it create any obligation or responsibility on the part of Intersect.

By using this guide and proceeding with any transaction to the Cardano treasury, **you acknowledge and agree that you do so entirely at your own risk**. You are solely responsible for verifying all transaction details, including but not limited to the recipient address, the amount of ADA to be transferred (e.g., 1000 ADA), network conditions, fees, and any other relevant parameters prior to submission.

Intersect does not facilitate, process, validate, or monitor any transactions and has no control over blockchain operations. As such, Intersect is unable to reverse, recover, amend, or otherwise intervene in any transaction once it has been initiated.

To the fullest extent permitted by applicable law, Intersect expressly disclaims all liability for any loss, damage, or claim arising out of or in connection with the use of this guide or any transaction undertaken, including but not limited to errors, omissions, incorrect transfers, failed transactions, or loss of funds.
{% endhint %}

## Guide

{% hint style="info" %}
## Prerequisites

The steps below assumes you have:&#x20;

* Access to a Cardano node socket and know how to set it as a variable in the shell i.e. CARDANO\_NODE\_SOCKET\_PATH
* Have sufficient Ada balance
{% endhint %}

{% stepper %}
{% step %}
### Query your wallet address and select the utxo(s) you would like to use to fund the donation to the treasury (inputs must be greater than 1000 ada)

```
cardano-cli conway query utxo \
--address <WALLET_ADDRESS> \
--mainnet
```
{% endstep %}

{% step %}
### Build the unsigned transaction &#x20;

```
cardano-cli conway transaction build \
--tx-in <TX_HASH#TX_IX> \
--treasury-donation <AMOUNT IN LOVELACE (i.e. 1 ada = 1000000 lovelace) > \
--change-address <WALLET_ADDRESS> \
--mainnet \
--out-file tx.raw
```
{% endstep %}

{% step %}
### Sign and submit via cli or

```
cardano-cli conway transaction sign \
--tx-file tx.raw \
--signing-key-file <SIGNING_KEY.skey> \
--mainnet \
--out-file tx.signed

cardano-cli conway transaction submit \
--tx-file tx.signed \
--mainnet
```
{% endstep %}

{% step %}
### Alternatively Sign and Submit via Lite Wallet

```
Copy cborHex from tx.raw 
e.g.
{
    "type": "Tx ConwayEra",
    "description": "Ledger Cddl Format",
    "cborHex": "fe5443bd1dd1fe20ea489884f2132916b41b0000004b10fce1e2021a00029a41151b001766c0df5a3a70161a02faf080a0f5f6"
}

Import to Lite Wallet 

Sign and Submit 
```
{% endstep %}
{% endstepper %}

{% hint style="info" %}
### Note

As the treasury value updates on the epoch boundary any transaction built should be submitted within the same epoch as it may fail due to the values being updated and the transaction will have to be rebuilt
{% endhint %}



## Community tools

<details>

<summary><strong>Typhon wallet</strong></summary>

This wallet offers a donation feature. Below is a simple guide<br>

1. Go in the 'Advanced' tab in your Typhon wallet and click 'donate'

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

2. Add the donation amount

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

3. Confirm the transaction

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>



</details>

