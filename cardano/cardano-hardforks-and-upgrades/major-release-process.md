# Major release process

{% hint style="info" %}
Please note that this overview is indicative of the process, some details have been omitted for simplicity and brevity. The process is also adaptable and subject to change.\
\
Also note that the process will change in the near future to reflect on-chain governance actions.
{% endhint %}

The following information is intended to provide the community an indicative overview of the major release process, major releases include such events as [hard forks](broken-reference). In blockchain technology a hard fork is one of the most significant upgrades. It is a radical change in a blockchain protocol that affects the validity of blocks and transactions on the decentralized network.&#x20;

The below provides an outline of the role different roles that Intersect committees, working groups and the community play in contributing to the major release process.

## Major release process

<figure><img src="../../.gitbook/assets/Major Release Process.gif" alt=""><figcaption><p>Indicative Major Release Process</p></figcaption></figure>

### **1. Continuity suppliers contribute to building a feature ready node which is a candidate for a major release**

<figure><img src="https://lh7-us.googleusercontent.com/_pm-76XatL2iPHXSVhkovkyiNrCuKkbtZ8MIEANexJen4ux_w_Asj-v8zmi8It5vI1MhjJZ26rtmf72tY5WHhZ6xlYM7gh_sYyWQu3lbReyBBUGHAuPXIUFEu-kAPl6p4YTzlZV3asa5PxY=s2048" alt=""><figcaption><p>Release 1</p></figcaption></figure>

[Continuity suppliers](../cardano-continuity/) play a crucial role in preparing for the upcoming hard fork by building a node that's ready for release.

<details>

<summary><strong>Here’s what each component entails:</strong></summary>

* **Ledger** - updates the system that keeps track of all transactions, making sure it's ready to handle the new types of transactions that the hard fork may introduce.
* **Node** - improves the core software of the blockchain to support enhanced features and performance.
* **Consensus** -  the rules for how transactions are verified across the network, ensuring everyone agrees on what is valid.
* **CLI (Command Line Interface)** - makes it easier for developers to interact with the blockchain by enhancing the tools they use to deploy and manage their applications.

Together, these and other updates from the continuity suppliers ensure the new node is robust, secure, and reliable for release, setting a solid foundation for a major release such as a hard fork

</details>

### 2. Intersect steers coordination of major release activity through the Technical Steering Committee and working groups

<figure><img src="https://lh7-us.googleusercontent.com/yzoSoimOX6N_e7-V3EJN7Zxp8-hj6FyqPPv_cdgdsx6_RVd8IZW9QdTzmvgTF1B1rG-l-xACP1IcUdn8og1Joe9Fxq69vGnoALCR2VHLyZ5X4veHF8E8VLpkFsCAkBSRJ5u_qtdAYOVoTAI=s2048" alt=""><figcaption><p>Release 2</p></figcaption></figure>

Intersect coordinates major releases, such as a hard fork, through its community led [Technical Steering Committee](../../intersect-overview/intersect-committees/technical-steering-committee-tsc/) and associated working groups. &#x20;

**Technical Steering Committee** - ensures that governance of Cardano is based upon sound technical awareness and best practices. The committee is a rally point for key members, suppliers and third parties to coordinate delivery of development services to support the Cardano blockchain.

**Intersect Hard Fork working group** - the hard fork working group focuses on the details of the hard fork. They are made up of relevant experts in different technical areas to facilitate the coordination on behalf of the TSC.

### 3. Continuity suppliers prove quality

<figure><img src="https://lh7-us.googleusercontent.com/kCbH6svXVvBYp6lvb3yiK0uYDovmKaArkuRMmAzGpsghJwluyvazFFOgpr4056pbk9WnA54H-U-RSEA5ZpP0io3CXpddNdp-nMJNHTKhRJfTrxhektyXx5-Bq4JmHix8DbblH3ysXKcSOTk=s2048" alt=""><figcaption><p>Release 3</p></figcaption></figure>

Continuity suppliers play a key role in making sure that new updates and changes to our software are of the highest quality before they go live. &#x20;

* **Development - push via quality -** the process starts in the development phase, where the main focus is on integrating quality right from the beginning. Instead of adding it later, quality is a priority from the start, which helps in building a more reliable and robust product.
* **Quality Reports -**  once the development integrates quality measures, the next step involves detailed quality reports. These reports are generated to assess the performance and reliability of the new updates.

### 4. Testing conducted with SPOs, Exchanges and dApps

<figure><img src="https://lh7-us.googleusercontent.com/XjMSqbrk9ihaN9tjEoWlKVTwAYei5vOzFYzXMtRGYHrQFUJ6EgxRkCP62Uds0q5qpzFnCeIBt6iwxSCwbvEFUQ7d2N74roYjh60qVzvxWoX8QY3xpam8KFGcN0rWrZRVFMm33bzCXh9m-x8=s2048" alt=""><figcaption><p>Release 4</p></figcaption></figure>

When preparing for major updates such as hard forks, community feedback and preparation is essential. Key members are invited to working groups, all of the community is encouraged to provide feedback.&#x20;

<details>

<summary><strong>Here’s how different community members can contribute:</strong></summary>

* **SPOs (Stake Pool Operators) -** play a crucial role in maintaining the blockchain network. Testing with SPOs helps ensure that the new updates will work smoothly in the live network environment. It checks the stability and efficiency of the network from the perspective of those who operate the network nodes.

<!---->

* **Wallets -** are tested to ensure that they can safely and effectively manage and store the new types of transactions that might be introduced by the update. This testing helps prevent issues that could affect users' funds.

<!---->

* **Exchanges -** need to integrate seamlessly with any new blockchain features to allow for smooth trading and liquidity. Testing with exchanges ensures that they can handle transactions without any disruptions or security risks.

<!---->

* **DApps (Decentralized Applications) -** Since dApps operate directly on the blockchain, testing with dApps checks for compatibility issues and ensures that they continue to operate efficiently even after the updates are applied.&#x20;

</details>

### 5. Feedback and major issues resolved by continuity suppliers

<figure><img src="https://lh7-us.googleusercontent.com/RfnIhOTxQw2H9zHTfy_ciMGwKqHKaYgytNh_3BSW03ZwpoDlNLfP7OPuKMjsvB0tzMdwbkMFkXZApKPVJdJ-fF9EjRWa-xN-BdeMkgfYqzZHE20wT57dXTGTUNJbMyiGjGQ6nuS8IjeDKBg=s2048" alt=""><figcaption><p>Release 5</p></figcaption></figure>

Feedback and issues are iteratively collected, triaged, categorised and resolved by the appropriate continuity suppliers.

<details>

<summary><strong>Here's how feedback and issues are managed:</strong></summary>

* **Collecting Feedback -** continuity suppliers actively gather feedback from users, stakeholders, and the community. This feedback is essential as it provides insights into quality and what needs improvement.

<!---->

* **Major Issues -** using the feedback collected, continuity suppliers work to resolve all major issues that could disrupt the service or product performance. These could include technical issues, performance inefficiencies, or community deployment problems.

<!---->

* **Resolving Issues -** once major issues are identified, the suppliers work on resolving them promptly. They prioritize these issues based on their impact and complexity.&#x20;

</details>

### 6. Community adoption

<figure><img src="https://lh7-us.googleusercontent.com/5hgljC8H6wxZ6Iz2obmtSWC-vfItDHULIFrs9yA4FjWVQIbnBvKGm4AolPhPmNAggvkzjQVsr-qARZ0ImwvQTXQijEv3hh3PqV8HKZJMWhVA_ICeXCKDkO_YrPMLbJ8TeVjYJk4DD3tOfBs=s2048" alt=""><figcaption><p>Release 6</p></figcaption></figure>

Once satisfactory time has passed, allowing major exchanges, SPOs and DApps to contribute to the quality process outlined and no high severity issues remain, a hard fork combinator event can be initiated - **pull of the community via adoption.**&#x20;

A hard fork combinator event is a way to update a blockchain without splitting it into two separate paths. Unlike a regular hard fork, which usually creates a new branch of the blockchain and leaves the old one behind, a hard fork combinator blends multiple updates into one smooth process. This means the blockchain can introduce new features or rules without stopping the system or losing any of its history.

**How this works?**

For example, when the Cardano blockchain moved from the Byron system to the Shelley system in 2020, they used a hard fork combinator. This tool allowed them to keep all the old Byron information while starting to add new Shelley features. This gradual change helped everyone on the network move over to the new system smoothly, without having to switch all at once

***

We hope you find the above a useful, as an indicative summary of how the major release process works, and the part the community has to play in the process.

To read more about, and to contribute to, quality and feedback please go to the following article on our knowledge base: [https://docs.intersectmbo.org/cardano-upgrades/quality-and-feedback](https://docs.intersectmbo.org/cardano-upgrades/quality-and-feedback)&#x20;
