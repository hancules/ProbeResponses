# Introduction
In this repository, we present a corpus of responses to semantic relation probes collected from human annotators.
Responses are filed in the `responses\human_responses.json`.
Six kinds of semantic relations are targeted:
- `ant`: antonymy
- `syn`: synonymy
- `hyp`: hypernymy
- `rhyp`: hyponymy
- `holo`: holonymy
- `mero`: meronymy
`human_outputs-sorted.json`. has a structure as follows.
```
<target word>:
  <semantic relation>:
    <prompt>:
      [
        The response from annotator 1,
        The response from annotator 1,
        The response from annotator 1,
        The response from annotator 1,
      ]

```
For, example `human_outputs_sorted["mother"]["hyp"]["the {0} is a kind of {1}"]` includes responses from human annotators to the probe *the mother is a kind of ___*.

# Statistics
|  Relation   | #Target words  | #Prompts |
|  :----  | :----:  | :----: |
| Antonymy  | 105 | 9 |
| Synonymy  | 218 | 7 |
| Hypernymy | 718 | 7 |
| Hyponymy  | 319 | 7 |
| Holonymy  | 195 | 7 |
| Meronymy  | 146 | 6 |

# Data Collection
We collect responses to probes from humans on the Amazon Mechanical Turk~(MTurk) crowdsourcing platform. 
We split 11,971 probes into 276 questionnaires and ensured no duplicate combinations of target word and semantic relation in one questionnaire. 
For example, "*my favorite relative is the V*" and "*the word relative has a vaguer meaning than the word V*" will not appear in the same questionnaire.
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
