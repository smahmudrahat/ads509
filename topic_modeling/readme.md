# Topic Modeling with LDA on the Brown Corpus

This repository contains code and analysis for performing topic modeling on a subset of the Brown Corpus using Latent Dirichlet Allocation (LDA). The project includes preprocessing steps, fitting the LDA model, and visualizing the topics with pyLDAvis.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Visualization](#visualization)
- [Results](#results)
- [License](#license)

## Introduction

This project demonstrates the application of Latent Dirichlet Allocation (LDA) to extract topics from the Brown Corpus. The Brown Corpus is a well-known dataset in the field of natural language processing, containing a diverse collection of texts across different categories. The analysis includes:

- Preprocessing the text data.
- Vectorizing the text using TF-IDF and Count Vectorizer.
- Fitting an LDA model.
- Visualizing the topics and their relationships using pyLDAvis.

## Dataset

The Brown Corpus is a collection of text samples from a wide range of sources. For this project, we focus on the following categories:

- Editorial
- Government
- News
- Romance
- Hobbies

The dataset is available through the NLTK library.

## Installation

To run the code in this repository, you need to have Python and the following libraries installed:

- nltk
- numpy
- pandas
- scikit-learn
- spacy
- pyLDAvis

You also need to download the Brown Corpus and a spaCy language model:

```python

import nltk
nltk.download('brown')

import spacy
spacy.cli.download('en_core_web_sm')
```
Clone the repository:

```bash
git clone https://github.com/yourusername/topic-modeling-brown-corpus.git
cd topic-modeling-brown-corpus
```

