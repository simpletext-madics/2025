---
layout: default
title: Tasks
---

# CLEF 2025 SimpleText: Tasks

---
## How to participate
In order to participate, you should sign up at the [CLEF](https://clef2025.clef-initiative.eu/index.php?page=Pages/registration.html) website: [https://clef2025-labs-registration.dei.unipd.it/](https://clef2025-labs-registration.dei.unipd.it/). 

All team members should join the SimpleText mailing list:
[https://groups.google.com/g/simpletext](https://groups.google.com/g/simpletext). 

The data will be made available to all registered participants.

## Task 1: Text Simplification (simplify scientific text)

The CLEF 2025 SimpleText track introduced the Cochrane-auto corpus, derived from biomedical literature abstracts and lay summaries from Cochrane systematic reviews. This corpus represents a significant expansion into the biomedical domain, building on methodologies used for datasets like Wiki-auto and Newsela-auto. An example of this new dataset is shown in Figure 1.

Cochrane-auto provides authentic parallel data produced by the same authors, enabling true document-level simplification. It incorporates advanced simplification techniques such as sentence merging, reordering, and alignment with discourse structure. This approach contrasts with more standard simplification corpora by realigning data at the paragraph, sentence, and document levels. A comparative analysis with existing simplification corpora is summarized in Table 3.

<br>One of the key benefits of Cochrane-auto is its contribution to reducing the manual effort for translation students and professionals. Instead of manually simplifying texts, they can focus on analyzing and annotating the evaluation data for types of information distortion, which in turn provides ground truth for other tasks.

### Descrption : 
This task remains the core NLP challenge of the track, divided into:

<br>**Task 1.1:** Sentence-level simplification.
<br>**Task 1.2:** Document-level simplification.
<br>The introduction of Cochrane-auto and the focus on the biomedical domain highlight the task's main innovation. Additionally, discussions are ongoing to introduce a third subtask on text alignment, where related abstracts (e.g., source and reference or source and predictions) are aligned at the sentence level. This involves n-to-n alignments, including sentence splits and merges, which are pivotal for downstream tasks like Task 2.

### Data
<br>The task uses the newly constructed Cochrane-auto corpus, consisting of large-scale realigned abstracts and lay summaries. Data is aligned at multiple levels:

<br>**Sentence-level:** Simplification and realignment of individual sentences.
<br>**Paragraph-level:** Matching simplified and source paragraphs.
<br>**Document-level:** Ensuring discourse-structured alignment.

### Evaluation
Evaluation for the task includes both automatic and human assessment:

<br>**Automatic Measures:** SARI, BLEU, LENS, BERTscore, among others.
<br>**Human Evaluation:** Translation students and professionals will assess selected samples for quality, fidelity, and types of information distortion.

## Task 2: Identification and avoidance of hallucination

This focuses on identifying creative text generation while avoiding spurious or hallucinatory content. This task was introduced after observing substantial over-generation in the outputs from previous participants in the SimpleText track. For 2024, 47% of submissions contained spurious sentences in at least 10% of their inputs, while 19% had hallucinations in 50% or more of their input sentences. The setup includes aligned sources, predictions, and references, enabling an analysis of source attribution, creative variation, and information distortion.

### Data

The SimpleText track has collected a vast dataset of realistic and representative outputs over the past three years.

<br>**For Task 2.1**, we will use outputs from models known for spurious generation, providing data to identify sentences fully grounded in the source input. This includes cases both with and without access to the source.
<br>**For Task 2.2**, we will utilize manually annotated sentences that exhibit types of information distortion, along with synthetic data to enhance coverage.
<br>**Task 2.3** follows the paired submission format used in Task 1, focusing on text alignment and grounded generation.
<br>All datasets include realigned sentences and predictions categorized by types of distortion, forming a comprehensive resource for training and evaluation.


### Evaluation

<br>**Task 2.1** will evaluate sentence labels using standard metrics like Precision, Recall, and F1, as well as token-level measures such as Jaccard similarity.
<br>**Task 2.2** will be assessed via automatic classification measures, categorizing distortion types.
<br>**Task 2.3** involves both automatic and human evaluation, examining sentence- and phrase-level differences with tools like MT Unbabel.
<br>Additionally, paired submissions will allow efficient evaluation of grounded generation. This task is being coordinated with other CLEF tracks, such as Eloquent and JOKER, and related events like SemEval (e.g., SHROOM and Mu-SHROOM), with the goal of potential joint tasks in the future.

## Task 3: SimpleText 2024 Revisited

CLEF 2025 introduces a restructured SimpleText track, aimed at adapting to new objectives and participant interests. Task 4 serves as a transitional track, potentially continuing work from CLEF 2024 tasks based on demand. Specifically, it considers re-running Task 1 on Content Selection (abstract retrieval) and Task 2 on Complexity Spotting (identifying and explaining difficult concepts), and Task 4 on State of the Art (information extraction in scientific documents). The continuation of these tracks is contingent on active interest and input from participants and organizers, with discussions planned at the CLEF 2024 conference in Grenoble.

### Description

CLEF 2025 SimpleText is very different from the earlier years. In order to facilitate the transition to the new track setup, we consider continuing some of the other CLEF 2024 SimpleText tasks (Task 1 on Content Selection: abstract retrieval, Task 2 on Complexity Spotting: identifying and explaining difficult concepts, Task 4 on SotA: tracking the state-of-the-art in scholarly publications). We will only continue those activities by request of, and with sufficient interest from, our active participants. 

### Data and evaluation

For further reference on methodology and evaluation criteria, details are available in the LNCS track overview paper by Ermakova et al. (2024b), as well as in the CEUR task overview papers for CLEF 2024 SimpleText Task 1 (Sanjuan et al., 2024), Task 2 (Di Nunzio et al., 2024), and Task 4 (D’Souza et al., 2024).  We aim to set up leaderboards for these tasks at Codalabs.
