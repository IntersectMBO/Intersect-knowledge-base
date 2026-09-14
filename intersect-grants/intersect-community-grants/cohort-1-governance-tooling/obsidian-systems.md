# Obsidian Systems

**Grant Value : 70,000 ADA**

## Scope:

* Apply Hydra payment channels to facilitating dRep voting incentives

## Deliverables:

*   Documentation covering, but not limited to;&#x20;

    (i)how Hydra payment channels could be applied to dRep voting incentives,&#x20;

    (ii) assumptions about the incentive model and amounts
* Design of proof of concept for making dRep incentive payment with Hydra
* Configure a demo of the payment channel to apply to dRep incentive payments;
* Create and publish use case documentation, including what was learned from the experiment;
* Conduct all activities as required for Sancho Network testing

## Updates:

* In progress - Completion due 31st May
* Report provided: [https://drive.google.com/file/d/1qNDQz23wAUMkDI2Y43H5rqnKJs2BA\_Xg/view?usp=drive\_link](https://drive.google.com/file/d/1qNDQz23wAUMkDI2Y43H5rqnKJs2BA_Xg/view?usp=drive_link)
* Open-Source Repository: [https://github.com/obsidiansystems/hydra-drep-incentives-poc](https://github.com/obsidiansystems/hydra-drep-incentives-poc)

## Takeaways:

1. The premise of this experiment was generally validated: DRep voting actions can be detected and tracked, then arbitrary incentives can be delivered to DRep addresses via Hydra head
   * Thanks to the governance state tracked on-chain, it is currently possible to know who has voted, when they voted, and on which proposals they voted
   * For builders requiring readily available data on transactions made as a response to votes (in or out of a hydra head) specific tooling for indexing could be considered
2. Builders interested in combining new governance functionality with hydra may require novel smart contract functionality operating within hydra that our work didn’t utilize but our work exposed no new limitations that would invalidate such development
   * This will depend on use-case specific tradeoffs
     * Ex. Community members could determine that distributing certain incentives via hydra is desirable but that a smart contract should trigger the distribution of funds to minimize the risk of malicious actors somehow misallocating or withholding incentives
3. The precise timing of our experimental implementation period meant that we experienced a late [compatibility issue](https://github.com/input-output-hk/hydra/issues/1462), as we developed much of our implementation using 8.11.0-pre before the respin had us using 8.11.0-sancho&#x20;
4. Given the rapid development - in the lead up to Chang - across so many core components, we still believe this marks an overall improvement in developer experience from previous network upgrade phases
   * Our hydra github issue was addressed immediately, so our team (and any similar projects) could plan accordingly, even if our specific issue wasn’t eligible for resolution and some mitigation was necessary&#x20;
   * &#x20;In the event of temporary new compatibility constraints, Hydra’s tooling enables development to continue with relatively predictable results (ex. Offline Mode)&#x20;
   * The hydra maintainers continue to do a great job of [communicating ](https://github.com/input-output-hk/hydra/releases)their specific upgrade path&#x20;
   * IOG’s Technical Community Discord maintains several sanchonet channels that are regularly updated and where help is available from/for a variety of technical community members
   * Sanchonet [documentation ](https://sancho.network/)represents an overall improvement over previous Cardano upgrade phases
5. Our work exposed some areas where improvements to developer experience and a reduction in confusion are still possible
   * Some documentation fell out of date or docs from different sources didn’t agree
     * Ex. The Cardano Operations Book continues to assume the use of cardano-node 8.11.0-pre ([here ](https://book.world.dev.cardano.org/env-sanchonet.html#configuration-files)and [here](https://book.world.dev.cardano.org/adv-sanchonet.html)) while [sancho.network](https://sancho.network/tutorials/start-node/) requires 8.11.0-sancho
   * cardano-cli continues to grow in complexity, accelerated by the addition of conway functionality
     * Community efforts improved the situation via the development of various wrappers as well as ‘[cheat sheets](https://able-pool.io/document)’
       * An organization like Intersect could possibly ensure such tools remain helpful by supporting or coordinating the various teams to ensure their tools remain rapidly updated and accurate
   * While some temporary incompatibility is to be expected as a network upgrade approaches, surprising cases (possibly resulting in lost productivity for community builders) could be minimized through a single source-of-truth; a living document that eagerly monitors all critical components, perhaps in the form of a compatibility checklist
     * An organization like Intersect could be well-suited to coordinate or support such an effort
     * The value of such coordination could compound when alternative nodes begin to come online

## **Close-out Report:**

* [https://drive.google.com/file/d/1sEGnLfoKAcvmYOhX5tZ6obBomU3p9Iu7/view](https://drive.google.com/file/d/1sEGnLfoKAcvmYOhX5tZ6obBomU3p9Iu7/view)
