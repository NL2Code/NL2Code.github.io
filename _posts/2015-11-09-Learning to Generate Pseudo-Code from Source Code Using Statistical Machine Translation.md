---
title: Learning to Generate Pseudo-Code from Source Code Using Statistical Machine Translation
author: coder
date: 2015-11-09 00:00:00 +0800
categories: [ACM]
tags: [benchmarks, metrics]
math: true
image:
  path: /assets/imgs/django.png
  width: 800
  height: 400
  alt: Example of source code written in Python and corresponding pseudo-code written in English.
---

## 📙Proposed Benchmark

- Benchmark Name: `Django`
- 📚Publisher/Date: `ACM/2015`
- 🏠Author Affiliation: Graduate School of Information Science, Nara Institute of Science and Technology
- 🔗URL: [https://github.com/odashi/ase15-django-dataset](https://github.com/odashi/ase15-django-dataset)
- Details: The Django dataset is a dataset for code generation comprising of `16000` training, `1000` development and `1805` test annotations. Each data point consists of a line of Python code together with a manually created natural language description.
- Supported Metric: `BLEU`; `HumanEvaluation-Acceptability`; `HumanEvaluation-Code Understanding`
- Test Case: ❌
- 🔏Input (NL)
  + 🚩Language: `English`; `Japanese`
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
    * [ ] What? (Requirement, TODO)
    * [x] How? (Algorithm Process)
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
    * [ ] General
    * [ ] Data Analysis and Manipulation
    * [ ] Plotting
    * [ ] Mathematical
    * [ ] Chemical
    * [ ] Educational
    * [x] Web Application
    * [ ] Other Domains
  + 👑Library
    * [x] Build-in Library
    * [ ] Public Library
    * [ ] Private Library
  + 🎯Level
  	* [ ] Token Level
    * [x] Line Level
    * [ ] Span Level
    * [x] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels
