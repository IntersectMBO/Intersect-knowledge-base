# Requirements

### Project Scope - Technical Requirements

Each grantee will implement [CIP-149 | Optional DRep Compensation](https://github.com/cardano-foundation/CIPs/blob/master/CIP-0149/README.md) functionality tailored to their platform:

**a) Wallets**

* Implement CIP-149 Optional DRep Compensation during staking reward withdrawal.
  * See example transaction: [38641cd70b0ab300e4fb850e7a0c747bac54d894bdc9deb07e934c0c0e4c6223](https://preview.cardanoscan.io/transaction/38641cd70b0ab300e4fb850e7a0c747bac54d894bdc9deb07e934c0c0e4c6223?tab=summary)
* Provide supporting UI to inform users about donating to their DRep.
* (Optional) Enable creation of DRep delegations containing CIP-149 metadata.

**b) Governance Tools**

* Enable creation of DRep delegations with CIP-149 metadata.
  * See example transaction: [8c86970a2431a9f43a0363b116b4c60471a29cc35d253c0ed8c18c1dff3dcf10](https://preview.cardanoscan.io/transaction/8c86970a2431a9f43a0363b116b4c60471a29cc35d253c0ed8c18c1dff3dcf10?tab=metadata)
* (Optional) Display compensation amounts received by DReps and a wallet's donation history.

**c) SDKs/Libraries**

Due to variance within SDK/Library design and functionality, there is flexibility with proposed implementations, suggested functions:

*   Add functions for creating CIP-149 DRep delegation transactions.

    * The motivation for this is to governance tool makers a straight forward way to build DRep delegation transactions, containing CIP-149 compliant metadata.
    * i.e. As a part of transaction building, give users methods to add CIP149 compliant metadata `transaction.addCIP149Delegation(stakeAddr, dRepID, donationBasisPoints)`

    ```typescript
    // Eample of what interfaces and functions could look like
    // SDKs and libraries are free to interpret and implement as suits their implementation

    // values based on (preview): 8c86970a2431a9f43a0363b116b4c60471a29cc35d253c0ed8c18c1dff3dcf10

    const stakeAddr = "stake1u8sa8kegf22wcjqqlc0230rtlemck5lhqycd3u8lattqh2cdjuzs4"
    const dRepID = "drep1yfhx2j5j7q989gfvj6cg04htakpqn32a3yuhtytjxt9m80qt5ekm3"
    const donationBasisPoints = 150 // 15% donation

    /** 
    * Where transaction is an existing object from library (something else can be used)
    * addCIP149Metadata adds a VoteDelegation certificate and CIP149 compliant metadata
    */
    transaction.addCIP149Delegation(stakeAddr, dRepID, donationBasisPoints)

    console.log(transaction.toJson())
    /**
    ...
    "certs":[
        0:{
          "VoteDelegation":{
            "stake_credential":{
              "Key":"e1d3db284a94ec4800fe1ea8bc6bfe778b53f70130d8f0ffea…"
            }
            "drep":{
              "KeyHash":"6e654a92f00a72a12c96b087d6ebed8209c55d893975917232…"
            }
          }
        }
      ]
    ...
    "auxiliary_data":{
      "metadata":{ 
        "3692": {
          donationBasisPoints: 150
        }
      }
    }
    ...
    */
    ```
*   Add functions for indexing CIP-149 delegation transactions.

    * The motivation for this is to wallets and governance tool makers an example implementation of how to index chain to find a given stake credential's CIP-149 delegations.
    * i.e. When a wallet is building a staking reward withdrawal transaction `getLastestCIP149Delegation()`

    ```typescript
    // Example of what interfaces and functions could look like
    // SDKs and libraries are free to interpret and implement as suits their implementation

    interface CIP149Delegation {
      txId: string;
      drepId: string;
      drepPaymentAddr: string;
      basisPoints: number;
    }

    /**
     * NoCIP149Delegation: The stakeKey has not delegated to a DRep using CIP149 correctly
     * NoDRepPaymentAddr: The DRep has not included payment address in their metadata
     */
    interface CIP149DelegationError {
      type: "NoCIP149Delegation" | "NoDRepPaymentAddr" ; // some more error cases
      message: string;
    }

    /**
     * getLastestCIP149Delegation triggers a chain query (using a given provider)
     * to find the most recent valid CIP149 delegation.
     * Indexing will invovle indexing the stakeKey's most recent vote delegation transacion
     * its transaction metadata and the DRep's latest metadata (to find DRep's payment address)
     */
    const cip149Delegation: CIP149Delegation | CIP149DelegationError = getLastestCIP149Delegation("stake1u8sa8kegf22wcjqqlc0230rtlemck5lhqycd3u8lattqh2cdjuzs4")

    const rewardsAvaliable = 100 // 100 ada avaliable in rewards account

    /**
     * Where withdrawalTransaction is an existing object from library (something else can be used)
     * The wallet can then use this information, to build the withdrawal transaction
     * using drepPaymentAddr and basisPoints to donate to the DRep
     */
    withdarawalTransaction.addRewardsWithdrawal(rewardsAvaliable)
    withdrawalTransaction.addOutput(cip149Delegation.drepPaymentAddr, (rewardsAvaliable/100 * cip149Delegation.basisPoints/10))

    ```

### Example Transactions

Staking Address: [stake\_test1ursa8kegf22wcjqqlc0230rtlemck5lhqycd3u8lattqh2c2ckq5g](https://preview.cardanoscan.io/stakeKey/stake_test1ursa8kegf22wcjqqlc0230rtlemck5lhqycd3u8lattqh2c2ckq5g)\
DRep ID: [drep1yfhx2j5j7q989gfvj6cg04htakpqn32a3yuhtytjxt9m80qt5ekm3](https://preview.cardanoscan.io/dRep/drep1yfhx2j5j7q989gfvj6cg04htakpqn32a3yuhtytjxt9m80qt5ekm3)\
DRep's most recent registration/update transaction: [337a2dc8ef4f2e139fae3c1f8a5eb25d7441d29db653417d6fe5883ea3e49227](https://preview.cardanoscan.io/transaction/337a2dc8ef4f2e139fae3c1f8a5eb25d7441d29db653417d6fe5883ea3e49227?tab=dRepCertificates)\
DRep's most recent metadata: [https://ipfs.io/ipfs/bafkreiaebdt43kqssaajkcpbg7wab5vq4g6e5kzwf4pals74lqk744wjrq](https://ipfs.io/ipfs/bafkreiaebdt43kqssaajkcpbg7wab5vq4g6e5kzwf4pals74lqk744wjrq)\
DRep's payment address (from metadata): `addr_test1vp8vlxck6kvndekp0fudqvlhc0lj5jvuk4a57ma7sqh0ucsmny9t3`

#### CIP-149 DRep Delegation

Transaction: [8c86970a2431a9f43a0363b116b4c60471a29cc35d253c0ed8c18c1dff3dcf10](https://preview.cardanoscan.io/transaction/8c86970a2431a9f43a0363b116b4c60471a29cc35d253c0ed8c18c1dff3dcf10?tab=metadata)

This transaction contains, both a Vote Delegation certificate and CIP-149 transaction metadata.&#x20;

* Vote Delegation certificate: This delegates the voting rights of [stake\_test1ursa...kq5g](https://preview.cardanoscan.io/stakeKey/stake_test1ursa8kegf22wcjqqlc0230rtlemck5lhqycd3u8lattqh2c2ckq5g) to [drep1yfh...ekm3](https://preview.cardanoscan.io/dRep/drep1yfhx2j5j7q989gfvj6cg04htakpqn32a3yuhtytjxt9m80qt5ekm3).
* CIP-149 Metadata: using the `3692` metadatum label the transaction metadata specifies `donationBasisPoints: 150` which is a donation of 15%.   &#x20;

#### CIP-149 Staking Rewards withdrawal

Transaction: [38641cd70b0ab300e4fb850e7a0c747bac54d894bdc9deb07e934c0c0e4c6223](https://preview.cardanoscan.io/transaction/38641cd70b0ab300e4fb850e7a0c747bac54d894bdc9deb07e934c0c0e4c6223?tab=summary)

This transaction contains, a staking rewards withdrawal (of `700,000 ada`) and two outputs, one to [stake\_test1ursa...kq5g](https://preview.cardanoscan.io/stakeKey/stake_test1ursa8kegf22wcjqqlc0230rtlemck5lhqycd3u8lattqh2c2ckq5g)'s chosen DRep ([drep1yfh...ekm3](https://preview.cardanoscan.io/dRep/drep1yfhx2j5j7q989gfvj6cg04htakpqn32a3yuhtytjxt9m80qt5ekm3)) and the second output was the change back to [stake\_test1ursa...kq5g](https://preview.cardanoscan.io/stakeKey/stake_test1ursa8kegf22wcjqqlc0230rtlemck5lhqycd3u8lattqh2c2ckq5g)'s wallet.

* The chosen DRep's payment address was found via their metadata
* The chosen compenation amount was found via the prior CIP149 delegation [transaction's metadata](https://preview.cardanoscan.io/transaction/8c86970a2431a9f43a0363b116b4c60471a29cc35d253c0ed8c18c1dff3dcf10?tab=metadata).
* The DRep compensation amount was `15%` of the withdrawn `700,000 ada`, equalling `105,000 ada`.

#### More example transactions

* **CIP-149 DRep Delegation**\
  Transaction: [09e735369a1782d190dab39c9f7a94bcc9b4faf40f0148c623f96fa4686f063f](https://preview.cardanoscan.io/transaction/09e735369a1782d190dab39c9f7a94bcc9b4faf40f0148c623f96fa4686f063f)
  * Delegates voting rights of [stake\_test1uqgykl...w7lk](https://preview.cardanoscan.io/stakeKey/stake_test1uqgykl0j0tdn689syxuasmg35hfjaqnd06t2fav38r7fyqcc0w7lk) to [drep1yf460x3...48je](https://preview.cardanoscan.io/dRep/drep1yf460x38f2elz52ua932m5pljtr750gn7vu6rsa6ewxlzug7r48je)
  * Donation: 15%
* **CIP-149 Staking Rewards Withdrawal**\
  Transaction: [c4a39ee99e1ba777c1151afd76356868d473271a76a8c252848af31db387c6d1](https://preview.cardanoscan.io/transaction/c4a39ee99e1ba777c1151afd76356868d473271a76a8c252848af31db387c6d1)
  * Withdraws 3,382.884997 ada
  * Sends 500.432749 (15%) to chosen DRep [drep1yf460x3...48je](https://preview.cardanoscan.io/dRep/drep1yf460x38f2elz52ua932m5pljtr750gn7vu6rsa6ewxlzug7r48je) on payment address [addr\_test1vqwq...9ftk](https://preview.cardanoscan.io/address/601c07a4478f0da1b99bd0d49de50b15c73fd5767befeadee373a59d14) as stated on DRep's [metadata](https://preview.cardanoscan.io/dRep/drep1yf460x38f2elz52ua932m5pljtr750gn7vu6rsa6ewxlzug7r48je?tab=meta).&#x20;
  * Remaining rewards sent back to wallet

### Eligibility

All applicants must successfully complete[ KYB (Know Your Business)](https://docs.intersectmbo.org/legal/policies-and-conditions/intersect-administration-policies/due-diligence-policy) verification as a condition of funding, as well as meeting the standards below tailored to the individual platforms.

* **Wallets:** Must be CIP-95 compliant, listed as mainnet-compatible on[ gov.tools](https://docs.gov.tools/cardano-govtool/using-govtool/getting-started/compatible-wallets), actively maintained, and commit to open documentation.
* **Governance Tools:** Publicly accessible, actively maintained, and already integrated with at least one governance process (delegation, voting, or proposal tracking). Must commit to open documentation.
* **SDKs/Libraries:** Open source, actively maintained, and used by at least one mainnet application. Must provide test coverage and documentation for CIP-149 functions.
