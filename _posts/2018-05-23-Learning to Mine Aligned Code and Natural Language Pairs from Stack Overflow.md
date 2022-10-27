---
title: Learning to Mine Aligned Code and Natural Language Pairs from Stack Overflow
author: coder
date: 2018-05-23 00:00:00 +0800
categories: [ACM]
tags: [benchmarks]
math: true
image:
  path: /assets/imgs/CoNaLa.png
  width: 700
  height: 500
  alt: Overview of our approach.
---

## 📙Proposed Benchmark

- Benchmark Name: `CoNaLa`[^conala]
- 📚Publisher/Date: `ACM/2018`
- 🏠Author Affiliation: Carnegie Mellon University
- 🔗URL: [https://conala-corpus.github.io](https://conala-corpus.github.io)
- Details: We have released a dataset crawled from `Stack Overflow`, automatically filtered, then curated by annotators, split into `2,379` training and `500` test examples. We also provide a large automatically-mined dataset with 600k examples, and links to other similar datasets. These data sets can be used for the `CoNaLa` challenge, or for any other research on the intersection of code and natural language.
- Supported Metric: `BLEU`
- Test Case: ❌
- 🔏Input (NL)
  + 🚩Language: `English`
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
- 🔑Output (code)
  + 🚩Language: `Python`; `Java`
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
    * [x] Line Level
    * [ ] Span Level
    * [ ] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 📘Reference

[^conala]: [https://arxiv.org/pdf/1805.08949.pdf](https://arxiv.org/pdf/1805.08949.pdf)
