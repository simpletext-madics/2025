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

The goal of this task is to decide which concepts in scientific abstracts require explanation and contextualization in order to help a reader understand the scientific text. The task has two steps: 

i) to retrieve up to 5 difficult terms in a given passage from a scientific abstract
ii) to provide a definition or an explanation or both of these difficult terms.

The corpus of Task 2 is based on the sentences in high-ranked abstracts to the requests of Task 1.

### Evaluation
We will evaluate complex concept spotting in terms of their complexity and the detected concept spans. We will automatically evaluate provided explanations by comparing them to references (e.g. ROUGE, cosine similarity, etc.). In addition, we will manually evaluate the provided explanations in terms of their usefulness with regard to a query as well as their complexity for a general audience. Note that the provided explanations can have different forms, e.g. abbreviation deciphering, examples, use cases, etc.

## Task 3: Simplify Scientific Text

The goal of this task is to provide a simplified version of sentences extracted from scientific abstracts. Participants will be provided with the popular science articles and queries and matching abstracts of scientific papers, split into individual sentences.

### Data
3 uses the same corpus based on the sentences in high-ranked abstracts to the requests of Task 1. Our training data is a truly parallel corpus of directly simplified sentences coming from scientific abstracts from the DBLP Citation Network Dataset for _Computer Science_ and Google Scholar and PubMed articles on _Health and Medicine_. In 2024, we will expand the training and evaluation data. In addition to sentence-level text simplification, we will provide passage-level input and reference simplifications.

### Evaluation
We will emphasize large-scale automatic evaluation measures (SARI, ROUGE, compression, readability) that provide a reusable test collection. This automatic evaluation will be supplemented with a detailed human evaluation of other aspects, essential for deeper analysis. We evaluate the complexity of the provided simplifications in terms of vocabulary and syntax as well as the errors (incorrect syntax; unresolved anaphora due to simplification; unnecessary repetition/iteration; spelling, typographic or punctuation errors). In previous runs almost all participants used generative models for text simplification, yet existing evaluation measures are blind to potential hallucinations with extra or distorted content. In 2024, we will provide new evaluation measures that detect and quantify hallucinations in the output.

## Task 4: Tracking the State-of-the-Art in Scholarly Publications
In Artificial Intelligence (AI), a common research objective is the development of new models that can report state-of-the-art (SOTA) performance. The reporting usually comprises four integral elements: Task, Dataset, Metric, and Score. These (Task, Dataset, Metric, Score) tuples coming from various AI research papers go on to power leaderboards in the community. Leaderboards, akin to scoreboards, traditionally curated by the community, are platforms displaying various AI model scores for specific tasks, datasets, and metrics. Examples of such platforms include the benchmarks feature on the Open Research Knowledge Graph and Papers with Code (PwC). Utilizing text mining techniques allows for a transition from the conventional community-based leaderboard curation to an automated text mining approach. Consequently, the goal of Task 4 is to develop systems which given the full text of an AI paper, are capable of recognizing whether an incoming AI paper indeed reports model scores on benchmark datasets, and if so, to extract all pertinent (Task, Dataset, Metric, Score) tuples presented within the paper. 

Please visit the [Task 4 website](https://sites.google.com/view/simpletext-sota/home) for information on registration, how to participate, task timelines, and dataset download links.
### Data
The training and test datasets for this task are derived from community-curated (T, D, M, S) annotations for thousands of AI articles available on PwC (CC BY-SA). These articles, originally sourced from arXiv under CC-BY licenses, are available in TEI XML format, each accompanied by one or more (T, D, M, S) annotations from PwC. The test set will strategically include only those articles with TDMs seen in the
training set, creating a few-shot evaluation setting. In addition to the few-shot evaluation, we intend to introduce a second evaluation setting for Task 4, evaluating models in a zero-shot context, for which a new test dataset will be created. This dataset will be enriched by articles which do not report leaderboards in order to train participants systems to also assign correct labels to articles from other domains.

### Evaluation
Participants systems will be evaluated in two evaluation settings:

For __Few-shot__ evaluation, trained systems will have to predict (T, D, M, S) annotations on a new collection of articles’ full-text. The labels in the gold dataset will include only (T, D, M, S)’s seen at least once in training.
For __Zero-shot__ evaluation, the task is as above with a different collection of articles, which have (T, D, M, S) with unseen T, D, or M in the training set.

In both settings, the standard recall, precision, and F-score metrics will be used to report scores to the participant systems.
