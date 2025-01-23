# Turkish Question Answering System for Gebze Technical University Official Student Rules

## Objective

This project is a Question Answering (QA) system designed to process natural language queries and provide precise answers based on Gebze Technical University's official student regulations. The system combines BM25 for context retrieval and a fine-tuned BERTurk model for span extraction.

## System Workflow

### Data Preparation:

The dataset consists of 1,416 question-answer pairs derived from the university regulations, organized in SQuAD format.

Contexts were paired with questions, and the data was split into 80% training and 20% testing sets.

### Context Retrieval:

BM25 algorithm ranks and retrieves the most relevant context for a given query by comparing tokens in the query and dataset.

### Answer Extraction:

A fine-tuned BERTurk model identifies the start and end positions of the answer span within the retrieved context.

### Web Interface:

Users interact with the system through a Flask-based interface, entering questions to receive precise answers in real time.

## Features

**Context Retrieval:** Uses BM25 to identify relevant regulation sections.

**Answer Extraction:** Fine-tuned BERTurk model predicts precise answer spans.

**Web Interface:** User-friendly interface built with Flask for real-time interaction.

## Results

**Exact Match (EM):** 7.63%

**F1 Score:** 24.04%

## Future Improvements

Expand dataset for better generalization.

Incorporate advanced data augmentation techniques.

Optimize fine-tuning with additional hyperparameter adjustments.

## Example Usage

Users can input questions into the web interface, and the system retrieves the most relevant context and extracts the answer.

![Screenshot 2025-01-23 at 21 53 01](https://github.com/user-attachments/assets/1cb3ad02-12eb-4b07-a42e-60ac1555879e)
