---
title: Natural Language to Code Generation in Interactive Data Science Notebooks
author: coder
date: 2022-12-19 00:00:00 +0800
categories: [arxiv]
tags: [models, benchmarks]
---

## 🎃Proposed Model

- Model Name: `PaChiNCo`[^arcade]
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: `Google`
- Architecture: `Transformer-based neural networks (decoder)`
- Pre-Training Corpus: `A lot of code files` and `A lot of notebooks`
- Supported Natural Language: `English`
- Supported Programming Language: `Python`
- Model Size: `62B`
- Public Item: `None`
- 🔗URL: `None`

## 📙Proposed Benchmark 

- Benchmark Name: `ARCADE`[^arcade]
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: `Google`
- 🔗URL: Dataset will be released shortly
- Feature: Data Science Notebooks
- Details: ARCADE consists of 1,082 NL-to-code problems from both existing data science notebooks on GitHub and new ones curated from scratch.
- Supported Metric: `pass@k`
- Test Case: ✅ 
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
    * [x] Why? (Background)
    * [x] What? (Requirement, Functionality, TODO)
    * [ ] How? (Algorithm Process)
    * [ ] Other Granularities
  + 🎯Additional Input
    * [ ] None
    * [x] Code Context
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
    * [ ] Line Level
    * [ ] Span Level
    * [x] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 📘Reference

[^arcade]: [https://arxiv.org/pdf/2212.09248.pdf](https://arxiv.org/pdf/2212.09248.pdf)
