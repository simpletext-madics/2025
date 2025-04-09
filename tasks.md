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
The CLEF 2025 SimpleText track introduced the Cochrane-auto corpus, derived from biomedical literature abstracts and lay summaries from Cochrane systematic reviews. This corpus represents a significant expansion into the biomedical domain, building on methodologies used for datasets like Wiki-auto and Newsela-auto.

Cochrane-auto provides authentic parallel data produced by the same authors, enabling true document-level simplification. It incorporates advanced simplification techniques such as sentence merging, reordering, and alignment with discourse structure. This approach contrasts with more standard simplification corpora by realigning data at the paragraph, sentence, and document levels.

<br>One of the key benefits of Cochrane-auto is its contribution to reducing the manual effort for translation students and professionals. Instead of manually simplifying texts, they can focus on analyzing and annotating the evaluation data for types of information distortion, which in turn provides ground truth for other tasks.

### Task 1.1 - Sentence-level Scientific Text Simplification
The goal of this task is to simplify whole sentences extracted from the Cochrane-auto dataset

### Task 1.2 - Document-level Scientific Text Simplification 
The goal of this task is to simplify whole documents extracted from the Cochrane-auto dataset

## Task 2: Controlled Creativity: Identify and Avoid Hallucination

Task 2 focuses on identifying and evaluating creative generation and information distortion in text simplification.

### Task 2.1 - Identify Creative Generation at Document Level

This task aims to detect creative generation at the abstract or document level. Participants will analyze system outputs from previous years, along with deliberately generated outputs from known models. The goal is to identify which sentences are fully grounded in the source text, both without access to the original sentences and with access to them. Additionally, sentences that introduce significant new content must be labeled. This task serves as a post-hoc identification or explanation challenge.

### Task 2.2 - Detect and Classify Information Distortion Errors in Simplified Sentences

This task focuses on detecting information distortion in simplified sentences and classifying the types of errors.

### Task 2.3 - Avoid Creative Generation and Perform Grounded Generation by Design

This task introduces a text alignment challenge, emphasizing grounded generation over creative generation. This task mirrors Task 1 on text simplification and requires submissions in paired runs, both with and without explicit source attribution.

## Task 3: SimpleText 2024 Revisited: Selected tasks by popular request

The CLEF 2025 SimpleText track introduces significant changes compared to previous years. To support the transition, we are considering continuing selected activities from the CLEF 2024 SimpleText tasks, including:
  - **Content Selection** – Retrieving relevant passages to include in a simplified summary.
  - **Complexity Spotting** – Identifying complex passages that require simplification.
  - **State-of-the-Art Tracking** – Monitoring advancements in scholarly publications related to text simplification.
