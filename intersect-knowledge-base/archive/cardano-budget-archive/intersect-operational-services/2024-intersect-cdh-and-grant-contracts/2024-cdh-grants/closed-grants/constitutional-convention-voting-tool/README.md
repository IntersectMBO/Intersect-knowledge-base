# Constitutional Convention Voting Tool

{% include "../../../../../../../.gitbook/includes/this-page-has-been-archived.md" %}

## Executive Summary

We are recommending that the voting tool described in the [Requirements](https://docs.google.com/document/d/1wRQwHj3HuQEOb59TNh4pvDD1IwCk8wJJaDqnTBku1lM/edit#heading=h.3znysh7) section of this document be put out to tender in an RFP. The RFP will be open for two weeks. This is so that we can find the most suitable provider, whilst allowing enough time for this provider to build the tool that Constitutional Delegates to the Constitutional Convention will use for voting to approve the Cardano Constitution.

## The purpose of a voting tool

There will be a Constitutional Convention in Buenos Aires, held in order to finalise the Cardano Constitution and then to ratify it with a vote. The people making these decisions will be Constitutional Delegates, each one representing a region in which a constitutional workshop was held, where they were elected by workshop attendees.

There are two purposes of this tool. Firstly, it is to facilitate a poll to approve the Constitution. In addition we want this to be a celebratory occasion for the Cardano community as a whole and we want the tooling to reflect this, both by being an on-chain voting tool and creating a spectacle.

Because of the nature of the constitutional delegates’ work, the organisers of the Convention will need to provide the constitutional delegates with a method of making decisions in a way that would be acceptable to both the constitutional delegates themselves and create legitimacy with the wider community as a whole.

## The method of voting during the Convention

Only someone who is a constitutional delegate elected from one of the global constitution workshops is eligible to vote, and they do so on a one-delegate-one vote basis. Any decision taken must be quorate in order to be legitimate. The threshold for approving the Constitution is a number of “yes” votes that is >50%\* of the constitutional delegates who have not cast a vote to abstain. This is consistent with how on-chain ratification is calculated.

#### Example

**Votes Cast**

| Senario | Did not vote | Voted abstain | Voted no | Voted yes | Total number of constitutional delegates | Result |
| ------- | ------------ | ------------- | -------- | --------- | ---------------------------------------- | ------ |
| A       | 2            | 20            | 15       | 23        | 60                                       | yes    |
| B       | 0            | 0             | 31       | 31        | 62                                       | no     |

**Scenario A Explained**

Threshold = (60 - 20)/2 =20

Result= 23>20 = constitution approved

**Scenario B Explained**

Threshold = (62 - 0)/2 =31

Result= 31==31 = constitution not approved

Because the number of yes votes (31) in scenario B was equal to, but not greater than the threshold (31) the result would be that the constitution would not be approved. Delegates and alternates would be asked to continue negotiating details of the constitution until it was felt a new poll could be held with a reasonable chance of approval, at this point a new poll would be held.

\*50% is an example of what the threshold might be, however there is a likelihood that the threshold will be set to the level required for DReps to ratify an Update to the Constitution governance action on-chain.
