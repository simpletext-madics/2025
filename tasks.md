# CLEF 2025 SimpleText: Tasks

[Home](./) | [Call for papers](./CFP) | [Important dates](./dates) | [Tasks](./tasks)  | [Tools](./tools) | 
[Program](./program) | [Publications](./publications) | [Organizers](./organizers) | [Contact](./contact) | [CLEF-2024](https://simpletext-project.com/2024/en/)

---
## How to participate
In order to participate, you should sign up at the [CLEF](https://clef2025.clef-initiative.eu/index.php) website: [http://clef2025-labs-registration.dei.unipd.it/](http://clef2024-labs-registration.dei.unipd.it/). 

All team members should join the SimpleText mailing list:
[https://groups.google.com/g/simpletext](https://groups.google.com/g/simpletext). 

The data will be made available to all registered participants.

## Task 1: Text Simplification (simplify scientific text)

### Description
This is the core NLP task of the track, and we continue with both sentence-level (Task 1.1 ) and document-level (Task 1.2 ) scientific text simplification. The main innovation is the very large new corpus we constructed in 2024, and the shift to the biomedical domain. We are discussing a third text alignment task, where two related abstracts (either source and reference, or source and predictions) need to be aligned at the sentence level, with possible n-to-n alignments (sentence splits or merges). Text alignment is a popular NLP task and key to CLEF 2025 SimpleText Task 2 below.

### Data
We constructed a large scientific text simplification corpus, based on realigning abstracts and lay summaries at scale at sentence, paragraph, and document-level. 

### Evaluation
We will use standard automatic evaluation measures (SARI, Blue, LENS, BERTscore,...) in combination human assessment of samples of the submissions by translation students and professionals. CLEF SimpleText has been the first and main driver of research in this IR/NLP area, but we align with related activities such as Scholarly Document Processing, and the new TREC PABLA track.

## Task 2: Identifying and explaining difficult concepts

To our own surprise, the SimpleText track has collected a massive collection of spurious (or over-) generation content from it’s participants. 

Our text simplification setup has sources, predictions, and references that are closely aligned and in the same language, in order
to study source attribution and creative variation, as well as to identify and avoid what is informally called “hallucinations”

### Description

Task 2.1 is to identify creative generation, at the abstract or document level. We will provide realistic system output from participants in earlier years, and some intentionally generated from known models. The task is to detect what sentences are fully grounded on source input (a) without and (b) with access to the source sentences, and hence also label those introducing significant new content. Task 2.1 is a post hoc identification or explanation task. Task 2.2 is to avoid creative generation, and perform grounded generation by design. This is mimicking Task 1 above, and asks to submit pairs of runs with/without source attribution by design. We are discussing a third text alignment task, related to both Task 1 and Task 2, in which we ask for optimal alignmentment of source attribution to align sentences/paragraphs in source and run output.

### Data

In running the SimpleText track over the last three years, we have collected a very large set of realistic and representative predictions in the run submission. For Task 2.1, we will select a sample of models and predictions known to be prone to spurious generation. We have large scale data available with realigned sentences lacking support in the source to be used as training data. For Task 2.2, we follow the setup of Task 1: Text Simplification above, but request paired runs.

### Evaluation

Task 2.1 is essentially a sentence label task, evaluated in the standard way (Precision, Recall, F1). For token level evaluation, we use standard Jaccard.6 Task 2.2 is evaluated by both standard automatic measures, and human evaluation, similar to Task 1 (Text Simplification) above. The paired runs allow us to sample for difference at sentence and phrase level and efficiently evaluate these, using for example MT Unbabel.


## Task 3: LeaderBoardQA

### Description
CLEF 2024 was the pilot year of the SOTA? task at SimpleText. We focused and evaluated in 2024 the important pre-processing step of information extraction, for which advance LLMs show high performance (Giglou et al., 2023). We expand the leader board construction task to a domain specific QA task on AI model performance against a corpus of full-text scientific documents. This LeaderBoardQA task ask for nuggets of information on a given model or model and benchmark pair, in terms of exact performance and metrics. We expect participants to use LLMs and RAGs, and will provide open corpus and closed book submissions

### Data and evaluation
We will significant revise the track setup and evaluation, re-using the CLEF 2024 community aligned data as training data, and providing human gold standard annotation for the evaluation and analysis. This will deliver a unique and valuable text collection for benchmarking this specific QA task. We will follow standard LLM/RAG evaluation for QA tasks. See also the details in the CEUR task overview paper for CLEF 2024 SimpleText Task 4 (D’Souza et al., 2024).

## Task 4: SimpleText 2024 Revisited

### Description
CLEF 2025 SimpleText is very different from the earlier years. In order to facilitate the transition to the new track setup, we consider continuing one of the other CLEF 2024 SimpleText tracks (Task 1 on Content Selection: abstract re- trieval, Task 2 on Complexity Spotting: identifying and explaining difficult concepts). We will only continue those activities by request of, and with sufficient interest from, our active participants. We will discuss this with participants and the current team of organizers at CLEF 2024 in Grenoble

### Data and evaluation
See details in the LNCS track overview paper (Ermakova et al., 2024b), and the CEUR task overview papers for CLEF 2024 SimpleText Task 1 (Sanjuan et al., 2024) and Task 2 (Di Nunzio et al., 2024).
