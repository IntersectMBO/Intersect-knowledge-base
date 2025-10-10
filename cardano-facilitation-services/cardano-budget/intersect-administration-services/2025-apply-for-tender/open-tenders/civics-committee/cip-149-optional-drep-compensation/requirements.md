# Requirements

### Project Scope - Technical Requirements

Each grantee will implement [CIP-149 | Optional DRep Compensation](https://github.com/cardano-foundation/CIPs/blob/master/CIP-0149/README.md) functionality tailored to their platform:

**a) Wallets**

* Implement CIP-149 Optional DRep Compensation during staking reward withdrawal.
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

### Eligibility

All applicants must successfully complete[ KYB (Know Your Business)](https://docs.intersectmbo.org/legal/policies-and-conditions/intersect-administration-policies/due-diligence-policy) verification as a condition of funding, as well as meeting the standards below tailored to the individual platforms.

* **Wallets:** Must be CIP-95 compliant, listed as mainnet-compatible on[ gov.tools](https://docs.gov.tools/cardano-govtool/using-govtool/getting-started/compatible-wallets), actively maintained, and commit to open documentation.
* **Governance Tools:** Publicly accessible, actively maintained, and already integrated with at least one governance process (delegation, voting, or proposal tracking). Must commit to open documentation.
* **SDKs/Libraries:** Open source, actively maintained, and used by at least one mainnet application. Must provide test coverage and documentation for CIP-149 functions.
