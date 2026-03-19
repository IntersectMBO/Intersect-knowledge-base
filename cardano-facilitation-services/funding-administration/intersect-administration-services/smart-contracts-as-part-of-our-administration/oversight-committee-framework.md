# Oversight Committee Framework

## Role and responsibilities of the Oversight Committee

The role of the Oversight Committee (OC) is to provide a check and balance on Intersect as an Administrator. The Oversight Committee is narrowly responsible for specific data assurance tasks as described below. All other permissions regarding any smart contracts and their functions are and will continue to be held by Intersect at all times. The OC should consist of at least 5 and at most 7 members, balancing the potential for conflicts of interest versus operational cost. Any OC member may withdraw from the role at any time. Intersect, acting reasonably and in the best interest of the Cardano Community may also remove a member of the OC. In the instance a member of the OC is removed or leaves, Intersect will work expeditiously to replace the removed member.

Intersect retains all liability for the vendor proposals contracts, including the responsibility of pausing and resuming all milestone payments. Nothing in this framework or the actions it envisages will transfer any of Intersect’s responsibility or liability to the OC.&#x20;

The OC will record their decision/s as metadata as part of the smart contract framework with their own private key/s.

### New role of Oversight Committee Members

Intersect and the members of the OC acknowledge that the OC is a new role within Intersects’ treasury withdrawal administration processes. As a result, it is to be expected that changes will be required moving forward. Intersect and the OC members will act in utmost good faith to work together to ensure solutions to any change requests. The OC will be notified of any changes to this framework via email; and where necessary meetings shall be held to discuss the changes. Oversight Committee members term is that of the Expiry of the Treasury Reserve Contract associated.

### Oversight Committee Members’ Conflict of Interest

OC members should avoid any situations that could reasonably be seen as a conflict of interest with their Assurance Task — for example, also acting as a vendor in a PSSC — by disclosing and stepping back from decisions when possible and being open about any such situations.

## Smart Contract Configuration

There are two types of smart contracts initially designed for managing treasury funds: a Treasury Reserve Contract (TRSC) and a Vendor Contract (PSSC), which are associated to a TRSC.

* TRSCs hold funds withdrawn from the Cardano treasury
* PSSCs hold funds intended for a specific vendor, for a specific project

Where practically possible Intersect will configure only one TRSC for its Administration role, and all PSSCs associated with that TRSC inherit the respective TRSC’s permissions, as described below.

Should additional TRSCs be required, the identical OC configuration will be configured for such TRSCs. The OC will be consulted on the creation of any additional TRSCs.

### Smart Contract Actions and Permissions

In total, the two contracts allow for 13 separate actions, of which 7 are permissioned in the context of the Oversight Committee framework:

| Action          | Description                                                                                                            |
| --------------- | ---------------------------------------------------------------------------------------------------------------------- |
| TRSC Fund       | Vendor payment - Funding a project for a vendor with a set of delivery milestones                                      |
| TRSC Disperse   | Disbursing funds to an arbitrary address and datum                                                                     |
| TRSC Sweep      | Returns funds held at the treasury contract back to the cardano treasury (before contract expiry)                      |
| TRSC Reorganize | Send from and to treasury contract - for actions such as splitting and merging UTxOs                                   |
| PSSC Pause      | Pauses a specific milestone for a vendor, preventing it from being claimed in case of a dispute of delivered work      |
| PSSC Resume     | Resuming a paused milestone, after the dispute has been resolved                                                       |
| PSSC Modify     | Modifying a project, with a vendors permission, to restructure the milestones or pay funds back to the treasury script |

In all cases, actions must be initiated by Intersect. In the cases of Fund, Modify, Disburse, Pause, Resume and Sweep, Intersect has implemented a two step process where administration key(s) are used to initiate or create actions, but they will also require Senior Leadership Team (SLT) Key(s) as part of the permission set. This effectively adds two person control within the administrator as additional checks and balances on internal processes.&#x20;

Overview of possible Actions and required thresholds per entity

| Operation       | Intersect Admin | Intersect Leadership | Oversight Committee |
| --------------- | --------------- | -------------------- | ------------------- |
| TRSC Fund       | 2 of 3          | 1 of 2               | 2 of 5              |
| TRSC Disperse   | 2 of 3          | ALL (2 of 2)         | 3 of 5              |
| TRSC Sweep      | 1 of 3          | 1 of 2               | Not required        |
| TRSC Reorganize | 2 of 3          | Not required         | 3 of 5              |
| PSSC Pause      | 2 of 3          | 1 of 2               | Not required        |
| PSSC Resume     | 2 of 3          | 1 of 2               | Not required        |
| PSSC Modify     | 2 of 3          | 1 of 2               | 2 of 5              |

A full description of the smart contracts can be found [here](https://github.com/SundaeSwap-finance/treasury-contracts), and a full description of the permission configurations can be found [here](https://github.com/IntersectMBO/budget-management/blob/main/treasury-contracts-config-readable.md).
