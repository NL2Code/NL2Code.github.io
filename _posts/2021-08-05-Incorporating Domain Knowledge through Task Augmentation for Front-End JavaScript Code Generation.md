---
title: Incorporating Domain Knowledge through Task Augmentation for Front-End JavaScript Code Generation
author: coder
date: 2021-08-05 00:00:00 +0800
categories: [FSE]
tags: [benchmarks]
math: true
---

## 📙Proposed Benchmark

- Benchmark Name: `Front-end Field Binding Dataset`[^front_end]
- 📚Publisher/Date: `FSE/2021`
- 🏠Author Affiliation: Alibaba; Peking University
- 🔗URL: [https://tianchi.aliyun.com/dataset/107819](https://tianchi.aliyun.com/dataset/107819)
- Details: Front-end Field Binding Dataset is a dataset used to automatically generate corresponding code snippet based on natural language description, in the actual front-end development work. It includes 3 files, train.xlsx is a training file containing 2150 training samples; test.xlsx is a test file containing 150 test samples. Both training and testing samples consist of two parts: the former is the generated code, and the latter is the natural language description. variable.xlsx is a variable vocabulary, containing 15525 pieces of information，each piece is a variable name that is often used in the front end and its corresponding Chinese description. It can be used as additional information to assist code generation. The task is to automatically generate corresponding code snippet based on natural language descriptions.

  ```json
  {
    "natural language description": '{text.title.length>5?text.title.slice(0,5):text.title}',
    "natural language description": '{("已售"+item.currentSellOut+"件")}'
  }
  ```

- Supported Metric: `Exact Match Accuracy`; `BLEU`; `Edit Similarity`
- Test Case: `Not involved`
- 🔏Input (NL)
  + 🚩Language: `Chinese`
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
  + 🚩Language: `Front-end Programming Language`
  + ⛺Domain
    * [x] General
    * [ ] Data Analysis and Manipulation
    * [ ] Plotting
    * [ ] Mathematical
    * [ ] Chemical
    * [ ] Educational
    * [ ] Other Domains
  + 👑Library
    * [ ] Build-in Library
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

[^front_end]: [https://arxiv.org/pdf/2208.10091.pdf](https://arxiv.org/pdf/2208.10091.pdf)
