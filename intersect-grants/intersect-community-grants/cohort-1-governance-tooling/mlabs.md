# Mlabs

**Grant Value : 70,000 ADA**

## Scope:

* update Plutarch to take advantage of features in the Conway Ledger Era

## Deliverables:

* Document relevant changes required for Plutarch
* Document relevant ledger, specification and API changes for Plutarch libraries
* This is likely to include, but may not be limited to;
  1. BLS curve features;
  2. Untyped Plutus Core (UPLC) optimizations;
  3. Changes to the UTXO body
  4. Integration of governance credentials and certificates, delegation, governance action interactions, and voting features;
  5. Test the updated and new features above, on the Sancho network; seek user feedback from MLabs’s major clients and other key ecosystem players on the updated and new features above; where feasible, integrate and test requested changes from the user feedback; communicate and promote Plutarch changes to other Intersect members and the Cardano community at large to increase awareness of the tools available to support developers

## Updates:

* In progress - Completion due 31st May
*   Pull requests completed up-to PlutusLedger V3 implementation are as follows:

    633 - Fix PRationalData's POrd instance, add test cases&#x20;
* 638 - Add Subproject changelogs&#x20;
* 645 - Create plutarch-api, to separate ledger api from plutarch core&#x20;
* 648 - Append plutarch-extra utilities relating to ledger api to plutarch-api&#x20;
* 650 - Fix script compilation logic that prevents function application from and to error type&#x20;
* 651 - Relocate TermCont tools into plutarch for better accessibility&#x20;
* 659 - Prune all ledger api related modules from plutarch and plutarch-extra in favor of pluatrch-api

### Close-out Report :

* [https://drive.google.com/file/d/1PJlJZWDUVcWxYkmjg24XQw8rfl--Ng\_g/view?usp=drive\_link](https://drive.google.com/file/d/1PJlJZWDUVcWxYkmjg24XQw8rfl--Ng_g/view?usp=drive_link)
