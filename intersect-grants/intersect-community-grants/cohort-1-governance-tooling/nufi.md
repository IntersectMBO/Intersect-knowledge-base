# NuFi

**Grant Value : 70,000 ADA**

## Scope:

* Implement CIP-95 and SanchoNet functionality into NuFi

## Deliverables:

* Updated NuFi wallet software: so users are able to connect the wallet to SanchoNet users are able to connect and interact with CIP95 governance dApps
* Includes but is not limited to:
  1. Display the new governance transaction types (vote delegation, DRep registration, DRep retirement, vote, submit a governance action)
  2. Provide information for users that explains why reward accounts with stake credentials not delegated to a DRep will be blocked from withdrawing any rewards

## Updates:

* In progress - Completion due 31st May
* Milestone 1 delivered in the "sanchonet" version of our extension published here: [https://github.com/nufi-official/nufi?tab=readme-ov-file#cardano-sanchonet-build](https://github.com/nufi-official/nufi?tab=readme-ov-file#cardano-sanchonet-build)
* Official documentation : [https://nufi.gitbook.io/developer-docs/nufi-wallet/testnet](https://nufi.gitbook.io/developer-docs/nufi-wallet/testnet)
* Download extension: [https://assets.nu.fi/extension/sanchonet/nufi-cwe-sanchonet-latest.zip](https://assets.nu.fi/extension/sanchonet/nufi-cwe-sanchonet-latest.zip)

## Close-out Report:

{% embed url="https://docs.google.com/document/d/1jjYXXelbDBwc5DuTkY2Zyd0-E68a3fGP/edit?usp=drive_link&ouid=102295201310683679603&rtpof=true&sd=true" %}

## Takeaways:

*   The governance functionality integration into NuFi went rather smoothly. We only faced minor issues regarding the Sanchonet node/db-sync stability and schema changes.

    We also consider the on-chain requirement to delegate to a DRep before withdrawing staked funds as a possible UX and maybe even legal challenge (institutional delegators, centralized exchanges, ...) for other wallets/(d)apps in the Cardano ecosystem which may deserve further discussion at community level.
