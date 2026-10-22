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
- 📦 Dataset: *[link to be added]*
- 🏆 Benchmark: [Codabench — Task 2](https://www.codabench.org/competitions/12936/)

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
- 🏆 Benchmark: [Codabench — Task 1](https://www.codabench.org/competitions/12776/)

**How to cite**

> Fanfu Wei, Thibault Ehrhart, Raphaël Troncy. *From Rows to Narratives: Benchmarking Semantic Relatedness Across Tables and Paragraphs.* TRIPLET 2026 Workshop @ ESWC 2026, Dubrovnik, Croatia, May 2026.


## KONTRAST
TBD
