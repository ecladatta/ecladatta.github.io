---
permalink: /datasets/
title: "Datasets & Resources"
excerpt: "ECLADATTA Datasets & Resources"
author_profile: true
---

## ReTaT - Relation Extraction across Text and Table

A manually annotated benchmark for **joint relation extraction across text and tables**: each gold triple (subject, relation, object) draws its evidence from both a paragraph and a table, so it cannot be recovered from either one alone.

| | |
|---|---|
| **Task** | Cross-modal (text + table) relation extraction |
| **Evaluation metrics** | Precision, Recall, F1 at three levels: exact triple match, entity-level partial match, relation-level partial match |
| **Languages** | English, French |
| **Size** | 3 subsets - 387 Wikipedia pages - 1,064 tables - ~6,400 annotated triples |
| **Relation schemas** | CORE company relations (Business) and Wikidata properties (Female Celebrities, Telecommunications) |
| **Format** | Paired files per document: paragraphs (TXT), tables (CSV), and gold triples in a separate annotation file indexed by document ID |
| **Sources** | English and French Wikipedia dumps (2024); Business subset built on CORE |
| **Licence** | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |

**Subsets**

| Subset | Language | Content | Relations | Triples |
|---|---|---|---|---|
| Business | English | 255 table–paragraph pairs | 9 CORE relations (closed list) | 2,997 |
| Female Celebrities | French | 100 full pages, 665 tables | 11 Wikidata properties (open) | 1,836 |
| Telecommunications | English | 32 full pages, 144 tables | 35 Wikidata properties (open) | 1,574 |

**Access**
- 📦 Dataset: [https://github.com/ecladatta/ReTaT](https://github.com/ecladatta/ReTaT)
- 📄 Paper: [https://aclanthology.org/2026.lrec-1.104.pdf](https://aclanthology.org/2026.lrec-1.104.pdf)

**How to cite**

> Mohamed Ettaleb, Thibault Ehrhart, Nathalie Aussenac-Gilles, Yoan Chabot, Mouna Kamel, Véronique Moriceau, Raphaël Troncy, Fanfu Wei. *ReTaT: A Unified Benchmark for Relation Extraction across Text and Table.* In Proceedings of the Fifteenth Language Resources and Evaluation Conference (LREC 2026), pages 1341–1351, May 2026. ELRA.


## LATTE - Linking Across Table and Text for Relatedness Evaluation

A human-annotated benchmark for **semantic relatedness classification between tables and text paragraphs**, built from Wikipedia.

| | |
|---|---|
| **Task** | Table–text relatedness classification |
| **Evaluation metrics** | P@k, R@k, F1@k |
| **Language** | English |
| **Size** | 7,674 tables - 41,880 paragraphs - 3,826 Wikipedia pages |
| **Annotations** | 70,031 table–paragraph pairs (9,784 related / 60,247 unrelated) |
| **Sources** | Wikipedia, reconstructed from [HybridQA](https://hybridqa.github.io/) and [QTSumm](https://github.com/yale-nlp/QTSumm) |
| **Licence** | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |

**Access**
- 📦 Dataset: [github.com/ecladatta/LATTE](https://github.com/ecladatta/LATTE)
- 📄 Paper: *[to be completed]*

**How to cite**

> Fanfu Wei, Thibault Ehrhart, Raphaël Troncy. *From Rows to Narratives: Benchmarking Semantic Relatedness Across Tables and Paragraphs.* TRIPLET 2026 Workshop @ ESWC 2026, Dubrovnik, Croatia, May 2026.


## KONTRAST - Detecting Knowledge Inconsistencies Across Text, Tables, and Knowledge Graphs

A benchmark and framework for **modality-level inconsistency detection**: for questions grounded in Wikipedia tables and text, KONTRAST compares the table-based answer with the answer retrieved from Wikidata through Text-to-SPARQL, then classifies any disagreement.

| | |
|---|---|
| **Task** | Detect whether a table-based answer and a KG answer agree and, if not, categorize the inconsistency |
| **Labels** | Same - Higher accuracy in KG than in Table - Higher accuracy in Table than in KG - Different answer - Temporal changes |
| **Evaluation** | SPARQL execution validity, value-bearing answer rate, distribution of inconsistency labels |
| **Language** | English |
| **Size** | 2,870 questions (1,370 SimpleQA / 1,500 ComplexQA) from 9 Table-QA sources, with SPARQL outputs and inconsistency labels for 3 Qwen3 models |
| **Sources** | Wikipedia tables, infoboxes and text (via NQ-Table, CompMix, QAMPARI, MoNaCo, OTT-QA, SportReason); Wikidata dump of 2025-05-10 |
| **Contents** | Raw and filtered QA inputs, generated SPARQL queries and KG results (GRASP), LLM-as-a-judge pipeline, final labelled files and statistics |
| **Licence** | *[to be completed]* |

**Question groups**

| Group | Source datasets | Evidence | Questions |
|---|---|---|---|
| SimpleQA | NQ-Table, CompMix-simple, QAMPARI | Table, infobox, or table + text | 1,370 |
| ComplexQA | CompMix-infobox, CompMix-table, MoNaCo, MoNaCo-time, OTT-QA, SportReason | Table, infobox, text, multi-hop | 1,500 |

**Access**
- 📦 Dataset and code: [github.com/ecladatta/KONTRAST](https://github.com/ecladatta/KONTRAST)
- 📄 Paper: [arXiv:2607.25959](https://arxiv.org/abs/2607.25959)

**How to cite**

> Fanfu Wei, Thibault Ehrhart, Raphaël Troncy. *Detecting Knowledge Inconsistencies Across Text, Tables, and Knowledge Graphs.* In Proceedings of the 25th International Conference on Knowledge Engineering and Knowledge Management (EKAW 2026), Turin, Italy, 2026.
