# Hash

{% include "../../../../.gitbook/includes/this-page-has-been-archived.md" %}

Constitutional Delegates were elected to represent their Constitutional Workshop and work to approve a Cardano Constitution to be put on-chain for DReps and the CC to vote. Although different file formats have been used along the way for drafting purposes, the version of the Constitution that must go on-chain is a text file (.txt) and a hash of that text file.

Hashing is used to confirm if a file matches the one being referenced. The hash of a file is like a fingerprint, and is unique to each file. If a single character changes in the file, the hash no longer matches.

A text file is used to ensure the hash matches as long as all of the written characters match. Text files strip away all except the written characters in the file, ensuring the hash will match so long as none of the words are changed in the file. Other programs, like Google Docs and Word, will add invisible information in the file. The hash of “Hello World” in a Google Document would not match the hash of “Hello World” in a Word document.

So, the Constitution text being voted on is being shared as a .txt file with the associated hash. This allows you to confirm that the document up for vote matches, word for word, the one that’s been distributed to you ahead of time.

\\

BLAKE2b-256 hash digest: `2a61e2f4b63442978140c77a70daab3961b22b12b63b13949a390c097214d1c5`

**How-to Check the hash**

**Easy Way**

Please see [Instructions to **verify** the constitution hash](https://docs.google.com/document/d/1xmDkMrL6ebaLNBsysiNQrtABcVnYBmsteQQcsrzGOpo/edit?tab=t.0#heading=h.bxb46qftdspf).

**CLI Way**

Using straight Cardano CLI pull from repo (no repo cloning needed).

```
cardano-cli hash anchor-data --url https://raw.githubusercontent.com/IntersectMBO/draft-constitution/refs/heads/main/2024-12-05/cardano-constitution-1.txt
```

Using Cardano CLI with local repo.

```
cardano-cli hash anchor-data --file-text ./2024-12-05/cardano-constitution-1.txt
```

Using hashing script (which uses Cardano CLI and b2sum).

```
./scripts/hash.sh ./2024-12-05/cardano-constitution-1.txt
```

\\
