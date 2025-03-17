---
permalink: /triplet/
title: "TRIPLET Challenge @ ISWC2025"
excerpt: "TRIPLET Challenge"
author_profile: true
---

TRIPLET (TRIPLET Extraction from Triplet Text, Table, Knowledge Graph) Challenge 2025 @ 24th International Semantic Web Conference (ISWC 2025), Nara, Japan

## Task Description
In recent years, the research community has shown increasing interest in the joint understanding of text and tabular data, often, for performing tasks such as question answering or fact checking where evidences can be found in texts and tables. 
Hence, various benchmarks have been developed for jointly querying tabular data and textual documents in domains such as finance, scientific publications, and open domain. 
While benchmarks for triple extraction from text for Knowledge Graph construction and semantic annotation of tabular data exist in the community, there remains a gap in benchmarks and tasks that specifically address the joint extraction of triples from text and tables by leveraging complementary clues across these different modalities.

In this context, the TRIPLET 2025 challenge aims at proposing three sub-tasks and a common benchmark for understanding the complementarity between tables, texts, and knowledge graphs, and in particular to propose a joint knowledge extraction and reconciliation process.
- Sub-task 1: the goal is to assess the relatedness between tables and textual passages (within documents and across documents). For example, in the figure below, a participant tool should identify the relatedness between the sentence containing the entity "AirPort Extreme 802.11n" (highlighted in yellow) and the data table providing information about output power and frequency for this entity. Participants will be provided with tables and textual passages that would need to be ranked. The evaluation will use metrics such as P@k, R@k and F1@k.
- Sub-task 2: the goal is to automatically extract knowledge jointly from tables and related texts. For example, in the figure below, a participant tool should extract triples composed of mentions located partly in the text and partly in the table and disambiguated with entities and predicates identified in the Wikidata reference knowledge graph. Knowledge extraction will be carried out in Open Extraction Information mode, using the Wikidata knowledge graph as a reference, but with the possibility that certain predicates or entities may not be present in the graph. Similar to the Text2KGBench evaluation, and because the set of triples are not exhaustive for a given sentence, to avoid false negatives, we will follow a locally closed approach by only considering the relations that are part of the ground truth. The evaluation will then use metrics such as P, R and F1.
- Sub-task 3: the goal is to check the consistency of knowledge extracted from tables and texts with existing triples in the Wikidata knowledge graph. Different kind of inconsistencies will be considered in this task.

<img src="https://github.com/ecladatta/ecladatta.github.io/blob/84263e7a843c3b5856911273614a5e6a85a34034/images/triplet_annotation_tool.png" alt="Annotation tool" />

## Data & Evaluation
For each of the 3 sub-tasks, we will release a dataset with ground-truth annotations, enabling participant teams to develop machine learning-based systems. 
The participants will be provided with a training set for training purposes and for hyperparameter optimizations and internal validations. 
A separate blind test dataset will remain private and be used for ranking the submissions.
Furthermore, we will rely on the AICrowd platform to host the challenge and to provide a live leaderboard to the participants. 
Each team will be allowed a limited number of daily submissions, and the highest achieved accuracy will be reported as the team's final result.
Additionally, we plan to encourage participants to develop open-source solutions, to utilise and fine-tune pre-trained language models and to experiment with LLMs of various size in zero-shot or few-shot settings.

## Call for Participants

### Important Dates

| Event                                 | Date          |
| ------------------------------------- | -------------- |
| Dataset (train and dev) release       | 30 March 2025 |
| Release of test set                   | 16 May 2025 |
| Submission of systems                 | 28 June 2025 |
| System Results & Notification of Acceptance | 19 July 2025 |
| Presentations@ISWC                    | November 2025 |

### Submission Details
TBD

## Challenge Organizers
- [Raphael Troncy](https://www.eurecom.fr/fr/people/troncy-raphael) (EURECOM, France)
- [Yoan Chabot](https://yoanchabot.github.io/) (Orange, France)
- [Véronique Moriceau](https://www.irit.fr/~Veronique.Moriceau/) (IRIT, France)
- [Nandana Mihindukulasooriya](https://scholar.google.es/citations?user=obOPbVQAAAAJ&hl=en) (IBM Research, USA)
    
Contact: 
For discussions, please use our [Google Group](https://groups.google.com/g/triplet-challenge)
