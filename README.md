# AI Discourse NLP Analysis

## Project Overview

This project investigates how artificial intelligence is represented and perceived in German-language online discourse. The analysis combines transformer-based sentiment analysis with corpus-linguistic methods and an exploratory analysis of AI personification.

The project was originally developed as part of a university research project in the field of linguistics and corpus linguistics. The original study used a larger dataset that is not publicly redistributable.

This repository presents a publicly shareable demonstration version of the project.

## Project Background

The original university project focused on the linguistic analysis of public discourse surrounding artificial intelligence. It examined sentiment and linguistic patterns in German-language online discussions, with particular attention to the ways in which AI systems are described and attributed human-like characteristics.

The original dataset cannot be published due to data access and licensing restrictions. Therefore, this GitHub version uses a separate synthetic dataset of 30 Reddit-style entries created specifically for this repository.

The demonstration dataset was generated with the assistance of ChatGPT and designed to reproduce relevant linguistic characteristics and the analytical structure of the original project without exposing or redistributing protected source material.

The results presented in this repository are therefore intended to demonstrate the analytical workflow and methodology rather than to reproduce the findings of the original university study.

## Research Questions

The analysis addresses the following questions:

1. How does sentiment towards artificial intelligence change over time?
2. Which forms of AI personification occur in the analysed texts?
3. How frequently do different personification categories occur?
4. How are different forms of AI personification associated with sentiment?

## Methods

The project combines several NLP and corpus-linguistic approaches:

* Text preprocessing and cleaning
* German language detection
* Transformer-based sentiment classification using BERT
* Manual validation of sentiment predictions
* Linguistic pattern detection
* AI personification detection
* Rule-based classification
* Semantic similarity using Sentence Transformers
* Temporal analysis by month and year
* Sentiment analysis across personification categories
* Data visualisation

### Sentiment Analysis

Sentiment classification is performed using the German BERT model:

`oliverguhr/german-sentiment-bert`

Each text is classified as:

* Positive
* Negative
* Neutral

The model predictions are subsequently compared with a manually labelled validation sample.

### AI Personification

The project also investigates whether AI systems are described using human-like characteristics or actions.

The personification analysis combines:

* linguistic patterns,
* German humanisation verbs,
* pronoun and phrase patterns,
* rule-based classification,
* semantic similarity using Sentence Transformers.

The identified cases are grouped into categories such as:

* `chat_partner`
* `super_ki`
* `fehlerhafte_ki`
* `handlungsfaehige_ki`
* `ironische_personifikation`

## Analysis Pipeline

```text
Synthetic Dataset
        ↓
Text Preprocessing
        ↓
German Language Filtering
        ↓
BERT Sentiment Analysis
        ↓
Manual Validation
        ↓
AI Personification Detection
        ↓
Personification Categorisation
        ↓
Temporal Analysis
        ↓
Sentiment × Personification Analysis
```

## Technologies

* Python
* pandas
* scikit-learn
* PyTorch
* Hugging Face Transformers
* Sentence Transformers
* spaCy
* langdetect
* Matplotlib
* Jupyter Notebook

## Dataset

The repository contains a small synthetic demonstration dataset:

`sample_data.tsv`

It contains 30 Reddit-style entries created specifically for this public version of the project.

The dataset should not be interpreted as a representative sample of Reddit users or public opinion. It is provided solely to demonstrate the NLP workflow and analytical methods.

## Limitations

This GitHub version has several limitations.

First, the publicly available dataset is synthetic and considerably smaller than the dataset used in the original university project. Consequently, the results cannot be generalised to Reddit users or to public attitudes towards AI.

Second, the personification classification is an exploratory hybrid approach combining linguistic rules and semantic similarity rather than a fully supervised machine-learning classifier.

Third, the manual sentiment validation sample is relatively small. The validation results should therefore be interpreted as an indication of model performance on the demonstration data rather than as a comprehensive evaluation of the BERT model.

## Project Structure

```text
ai-discourse-analysis/
│
├── README.md
├── LICENSE
├── .gitignore
├── Sentiment Analysis .ipynb
└── sample_data.tsv
```

## Purpose

This repository demonstrates the application of NLP methods to a linguistically motivated research problem. It combines computational methods with corpus-linguistic analysis to investigate sentiment and representations of artificial intelligence in German-language discourse.
