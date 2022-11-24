---
title: Execution-based Evaluation for Data Science Code Generation Models
author: coder
date: 2022-11-17 00:00:00 +0800
categories: [arxiv]
tags: [benchmarks, metrics]
math: true
image:
  path: /assets/imgs/ExeDS.png
  width: 800
  height: 500
  alt: An example from ExeDS.
---

## 📙Proposed Benchmark 

- Benchmark Name: `ExeDS`[^exeds]
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: Beihang University; Microsoft; Hong Kong University of Science and Technology; Toronto University
- 🔗URL: [https://github.com/Jun-jie-Huang/ExeDS](https://github.com/Jun-jie-Huang/ExeDS)
- Feature: Data Science Code Generation
- Details: Automatically generating code is beneficial to the productivity of data science practitioners. Future progress towards this goal requires systems to generate executable code and measure execution correctness. In this repo we introduce ExeDS, a data science code generation dataset for execution evaluation, which contains 534 problems with execution outputs from Jupyter Notebooks, together with 123K examples for training and validation. ExeDS leverages three novel execution metrics to evaluate the executability and output correctness of code, including no error rate, execution exact match, and execution F1 score. We hope our dataset and execution metrics could draw more attention to the execution correctness of code and result in significant advances in code generation!
- Supported Metric: `BLEU`; `CodeBLEU`; `EM`; `OutputEM`
- Test Case: ❌
- 🔏Input (NL)
  + 🚩Language: `English`
  + 🌟Format
    * [x] Code Context
    * [ ] Plain Natural Language
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
    * [ ] General
    * [x] Data Analysis and Manipulation
    * [ ] Plotting
    * [ ] Mathematical
    * [ ] Chemical
    * [ ] Educational
    * [ ] Other Domains
  + 👑Library
    * [ ] Build-in Library
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

## 🚩Proposed Metric

- Metric Name: `OutputEM`
- Definition: OutputEM is the proportion of examples with correct output.

## 📘Reference

[^exeds]: [https://arxiv.org/pdf/2211.09374.pdf](https://arxiv.org/pdf/2211.09374.pdf)
