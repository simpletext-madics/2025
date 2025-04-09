---
layout: default
title: Tasks
---

# Tasks

## How to participate
In order to participate, you should sign up at the [CLEF](https://clef2025.clef-initiative.eu/index.php?page=Pages/registration.html) website: [https://clef2025-labs-registration.dei.unipd.it/](https://clef2025-labs-registration.dei.unipd.it/). 

All team members should join the SimpleText mailing list:
[https://groups.google.com/g/simpletext](https://groups.google.com/g/simpletext). 

The data will be made available to all registered participants.

## Task 1: Text Simplification: Simplify scientific text

### Task 1.1 - Sentence-level Scientific Text Simplification

### Task 1.2 - Document-level Scientific Text Simplification 

## Task 2: Controlled Creativity: Identify and Avoid Hallucination

### Task 2.1 - Identify Creative Generation at Document Level

### Task 2.2 - Detect and Classify Information Distortion Errors in Simplified Sentences

### Task 2.3 - Avoid Creative Generation and Perform Grounded Generation by Design

## Task 3: SimpleText 2024 Revisited: Selected tasks by popular request
  - Search: content selection
  - Complex terminology analysis
  - Complexities in evaluating generated definitions/explanations
<!--
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

### Description: 
This is the core NLP task of the track, and we continue with both : Sentence-level and document-level scientific text simplification.

The main innovation is the very large new corpus we constructed in 2024, and the shift to the biomedical domain. We are discussing a third text alignment subtask, where two related abstracts (either source and reference, or source and predictions) need to be aligned at the sentence level, with possible n-to-n alignments (sentence splits or merges). Text alignment is a popular NLP task and key to CLEF 2025 SimpleText Task 2 below.

### Data
The task uses the newly constructed Cochrane-auto corpus, consisting of large-scale realigned abstracts and lay summaries. Data is aligned at multiple levels:

<br>**Sentence-level:** Simplification and realignment of individual sentences.
<br>**Paragraph-level:** Matching simplified and source paragraphs.
<br>**Document-level:** Ensuring discourse-structured alignment.

### Evaluation
Evaluation for the task includes both automatic and human assessment:

<br>**Automatic Measures:** SARI, BLEU, LENS, BERTscore, among others.
<br>**Human Evaluation:** Translation students and professionals will assess selected samples for quality, fidelity, and types of information distortion.

## Task 2: Controlled Creativity

### Description

Task 2 focuses on identifying and evaluating creative generation and information distortion in text simplification.

- **Task 2.1** aims to detect creative generation at the abstract or document level. Participants will analyze system outputs from previous years, along with deliberately generated outputs from known models. The goal is to identify which sentences are fully grounded in the source text, both without access to the original sentences and with access to them. Additionally, sentences that introduce significant new content must be labeled. This task serves as a post-hoc identification or explanation challenge.
- **Task 2.2** focuses on detecting information distortion in simplified sentences and classifying the types of errors.
- **Task 2.3 (under discussion)** introduces a text alignment challenge, emphasizing grounded generation over creative generation. This task mirrors Task 1 on text simplification and requires submissions in paired runs, both with and without explicit source attribution.

### Data

Over the past three years of running the SimpleText track, we have compiled a comprehensive dataset of realistic and representative system outputs.

- **For Task 2.1**, we will select predictions prone to spurious generation, using large-scale realigned sentence data that lacks clear support in the source text. These will serve as training data.
- **For Task 2.2**, we have manually annotated automatically simplified sentences from previous SimpleText participants, classifying them by types of information distortion. This dataset will now be expanded with synthetic data.
- **Task 2.3** follows the setup of Task 1, requiring paired submissions to compare outputs with and without source attribution.

### Evaluation

- **Task 2.1** will be evaluated as a sentence classification task using standard Precision, Recall, and F1 scores. Token-level evaluation will be measured using Jaccard similarity.
- **Task 2.2** will be assessed with standard automatic classification metrics.
- **Task 2.3** will combine automatic evaluation with human assessment, similar to Task 1 on Text Simplification. Paired runs will allow efficient sentence- and phrase-level comparisons using tools such as MT Unbabel.

## Task 3: SimpleText 2024 Revisited

### Description

The CLEF 2025 SimpleText track introduces significant changes compared to previous years. To support the transition, we are considering continuing selected activities from the CLEF 2024 SimpleText tasks, including:

- **Task 1: Content Selection** – Retrieving relevant passages to include in a simplified summary.
- **Task 2: Complexity Spotting** – Identifying complex passages that require simplification.
- **Task 4: State-of-the-Art Tracking** – Monitoring advancements in scholarly publications related to text simplification.
These activities will only continue if participants show sufficient interest. Discussions are ongoing, and we are exploring hosting selected tasks on CodaBench.

### Data and evaluation
For further reference on methodology and evaluation criteria, details are available in the LNCS track overview paper by Ermakova et al. (2024b), as well as in the CEUR task overview papers for CLEF 2024 SimpleText Task 1 (Sanjuan et al., 2024), Task 2 (Di Nunzio et al., 2024), and Task 4 (D’Souza et al., 2024).  We aim to set up leaderboards for these tasks at Codalabs.
-->
