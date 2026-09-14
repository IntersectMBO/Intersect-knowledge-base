# CIP-95 support for Cardano Transaction Library (CTL)

The Cardano-Transaction-Library will be updated to support new Conway primitives and implement a CIP-95-enabled wallet connector. Successful implementation of this proposal would benefit Cardano transaction library users, who will unlock the ability to interact with CIP-1694 primitives via CIP-95 wallet interfaces.&#x20;

**Grant value: 106,000 ADA**

**Project complete.**

* **Milestone 1** - Serialization Support: [https://drive.google.com/file/d/1-wKUytjk6u4ZIZWs2O4QXPLgTHJwR9R4/view?usp=drive\_link](https://drive.google.com/file/d/1-wKUytjk6u4ZIZWs2O4QXPLgTHJwR9R4/view?usp=drive_link)
  1. Conway-compatible version of purescript- cardano- serialization-lib library (PS-CSL).
  2. Release notes.
* **Milestone 2** - Core types implementation: [https://drive.google.com/file/d/1dIvx1BDH1hx3B8TvZ-oAyAp50jR2JLVc/view?usp=drive\_link](https://drive.google.com/file/d/1dIvx1BDH1hx3B8TvZ-oAyAp50jR2JLVc/view?usp=drive_link)
  1.  Conway-compatible version of purescript- cardano-types library

      (formerly part of CTL, now afactored out standalone library).
  2. Release notes.
* **Milestone 3** - CIP-0095 PureScript implementation
  1. A new PureScript package (library) is created,similar in spirit to purescript- cip30-typesafe,that provides CIP-95 primitives as a PureScript API.
* **Milestone 4** - Prepare for CTL update
  1. An intermediate version of CTL with dependencies updated to support Conway features.
*   **Milestone 5** - CTL Update

    1. The final release of CTL with Conway transactions and CIP-0095 support included.
    2. CTL release notes.

    -> [Milestone 3, 4 and 5 Acceptance form](https://drive.google.com/file/d/1GNBwYnG7K27dFeMQCPZU2gjKFEJ1cBy7/view?usp=sharing)
