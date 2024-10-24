# Introduction
In this repository, we present a corpus of responses to semantic relation probes collected from human annotators.
Responses are filed in the `responses\human-responses.json`.
Six kinds of semantic relations are targeted:
- `ant`: antonymy
- `syn`: synonymy
- `hyp`: hypernymy
- `rhyp`: hyponymy
- `holo`: holonymy
- `mero`: meronymy

`human-responses.json`. has a structure as follows.
```
<target word>:
  <semantic relation>:
    <prompt>:
      [
        The response from annotator 1,
        The response from annotator 2,
        The response from annotator 3,
        The response from annotator 4,
      ]

```
For, example `human_outputs_sorted["mother"]["hyp"]["[DET] [W] is a kind of [V]"]` includes responses from human annotators to the probe *a mother is a kind of a ___*.


# Statistics
|  Relation   | #Target words  | #Prompts |
|  :----  | :----:  | :----: |

| Hypernymy | 692 | 7 |
| Hyponymy  | 310 | 4 |
| Holonymy  | 186 | 7 |
| Meronymy  | 144 | 6 |
| Antonymy  |  91 | 9 |
| Synonymy  | 211 | 7 |


# Data Collection
We collect responses to probes from humans on the Amazon Mechanical Turk~(MTurk) crowdsourcing platform. 
We split 10,546 probes into 276 questionnaires and ensured no duplicate combinations of target word and semantic relation in one questionnaire. 
For example, "*a mother is a kind of a ___*" and "*the word mother has a more specific meaning than the word ___*" will not appear in the same questionnaire.
We collected four responses for each questionnaire, and hence, there were four answers for each probe.
Participants are restricted to those
- whose answers are approved more than 500 times and the approval rate is beyond 95\%;
- who are currently living in either of the United States, the UK, Australia and Canada;
- who has the Mturk Master qualification.
We recruited 48 participants in total, and each answered 22 questionnaires on average. 

We included three bogus items in each questionnaire to confirm that participants had answered the questions carefully. 
We accepted all responses since every participant correctly answered all bogus items.

# Contact
If you have any questions, please contact Zhihan Cao (cao.z.ab@m.titech.ac.jp).
