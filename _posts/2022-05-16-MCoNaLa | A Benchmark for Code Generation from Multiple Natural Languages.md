---
title: MCoNaLa | A Benchmark for Code Generation from Multiple Natural Languages
author: coder
date: 2022-05-16 00:00:00 +0800
categories: [arxiv]
tags: [benchmarks]
math: true
image:
  path: /assets/imgs/MCoNaLa.png
  width: 500
  height: 450
  alt:  Examples in the MCoNaLa dataset, that aim to generate general-purpose Python code snippets from source intent of multiple natural languages.
---

## 📙Proposed Benchmark

- Benchmark Name: `MCoNaLa`
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: Carnegie Mellon University; Princeton University
- 🔗URL: [https://github.com/zorazrw/multilingual-conala](https://github.com/zorazrw/multilingual-conala)
- Sub-benchmark
  * CoNaLa[^conala]
- Feature: A benchmark for code generation from multiple natural languages.
- Details: Modeled off of the methodology from the English Code/Natural Language Challenge (`CoNaLa`) dataset, we annotated a total of `896` NL-code pairs in three languages: Spanish, Japanese, and Russian.
- Supported Metric: `BLEU`
- Test Case: ❌
- 🔏Input (NL)
  + 🚩Language: `English`; `Spanish`; `Japanese`; `Russian`
  + 🌟Format
    * [ ] Code Context
    * [x] Plain Natural Language
    * [ ] Competition Problem
    * [ ] Code Comment
    * [ ] TODO
    * [ ] Pseudocode
    * [ ] Other Formats
  + 💈Description Granularity
    * [ ] Why? (Background)
    * [x] What? (Requirement, Functionality, TODO)
    * [ ] How? (Algorithm Process)
    * [ ] Other Granularities
  + 🎯Additional Input
    * [x] None
    * [ ] Class Information
    * [ ] File Information
    * [ ] Repository Information
    * [ ] Other Information
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
    * [ ] Other Libraries
  + 🎯Level
  	* [ ] Token Level
    * [x] Line Level
    * [ ] Span Level
    * [ ] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 📘Reference

[^conala]: [https://conala-corpus.github.io](https://conala-corpus.github.io)
