---
title: A parallel corpus of Python functions and documentation strings for automated code documentation and code generation
author: coder
date: 2017-07-07 00:00:00 +0800
categories: [IJCNLP]
tags: [benchmarks]
math: true
image:
  path: /assets/imgs/code-doc-corpus.png
  width: 800
  height: 500
  alt: A Python function with its extracted declaration, docstring, body and repository metadata.
---

## 📙Proposed Benchmark

- Benchmark Name: `code-docstring-corpus`[^code-doc-corpus]
- 📚Publisher/Date: `IJCNLP/2017`
- 🏠Author Affiliation: University of Edinburgh
- 🔗URL: [https://github.com/EdinburghNLP/code-docstring-corpus](https://github.com/EdinburghNLP/code-docstring-corpus)
- Feature: In this work we introduce a large and diverse parallel corpus of a hundred thousands Python functions with their documentation strings (”docstrings”) to train a neural model.
- Details: We release a parallel corpus of `150370` triples of function declarations, function docstrings and function bodies. We include multiple corpus splits, and an additional "monolingual" code-only corpus with corresponding synthetically generated docstrings.

  ![Window shadow](/assets/imgs/code-doc-corpus-2.png){: .shadow width="500" height="30" }
  _Number of examples, tokens and lines of code in the corpora._

- Supported Metric: `BLEU`
- Test Case: ❌
- 🔏Input (NL)
  + 🚩Language: `English`
  + 🌟Format
    * [ ] Code Context
    * [ ] Plain Natural Language
    * [ ] Competition Problem
    * [x] Code Comment
    * [ ] TODO
    * [ ] Pseudocode
    * [ ] Other Formats
  + 💈Description Granularity
    * [ ] Why? (Background)
    * [x] What? (Requirement, Functionality, TODO)
    * [ ] How? (Algorithm Process)
    * [ ] Other Granularities
- 🔑Output (code)
  + 🚩Language: `Python`
  + ⛺Domain
    * [x] General
    * [ ] Data Analysis and Manipulation
    * [ ] Plotting
    * [ ] Mathematical
    * [ ] Chemical
    * [ ] Educational
    * [ ] Other Domains
  + 👑Library
    * [x] Build-in Library
    * [x] Public Library
    * [ ] Private Library
  + 🎯Level
  	* [ ] Token Level
    * [ ] Line Level
    * [ ] Span Level
    * [x] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 📘Reference

[^code-doc-corpus]: [https://arxiv.org/pdf/1707.02275.pdf](https://arxiv.org/pdf/1707.02275.pdf)
