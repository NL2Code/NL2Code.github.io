---
title: NL2Code | A Corpus and Semantic Parser for Natural Language to Code
author: coder
date: 2019-09-26 00:00:00 +0800
categories: [other]
tags: [benchmarks]
math: true
image:
  path: /assets/imgs/nl2code2019.png
  width: 800
  height: 500
  alt: Simple examples of text-code pairs of our corpus.
---

## 📙Proposed Benchmark 

- Benchmark Name: `NL2Code Corpus`[^paper]
- 📚Publisher/Date: `Other/2019`
- 🏠Author Affiliation: Novelis Lab; LSE2I ENSAO Lab
- 🔗URL: `None`
- Details: The proposed corpus consists of text-code pairs, each pair consisting of a code and a description in natural language. We used 13,000 text code pairs following a set of correct total filtering steps (using a python script). We divide randomly this data into two sets, the firsl one for learning (80%) and the second one for testing (20%).
- Supported Metric: `EM`; `ES`; `Accuracy`; `BLEU`; `CodeBLEU`
- Test Case: ❌
- 🔏Input (NL)
  + 🚩Language: `French`
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
    * [ ] What? (Requirement, Functionality, TODO)
    * [x] How? (Algorithm Process)
    * [ ] Other Granularities
  + 🎯Additional Input
    * [x] None
    * [ ] Class Information
    * [ ] File Information
    * [ ] Repository Information
    * [ ] Other Information
- 🔑Output (code)
  + 🚩Language: `Java`
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
    * [ ] Public Library
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

[^paper]: [NL2Code: A Corpus and Semantic Parser for Natural Language to Code](https://link.springer.com/chapter/10.1007/978-3-030-53187-4_65)
