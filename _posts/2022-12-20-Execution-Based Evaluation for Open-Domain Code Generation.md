---
title: Execution-Based Evaluation for Open-Domain Code Generation
author: coder
date: 2022-12-20 00:00:00 +0800
categories: [arxiv]
tags: [benchmarks]
math: true
---

## 📙Proposed Benchmark 

- Benchmark Name: `ODEX`[^odex]
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: `Carnegie Mellon University`; `Inspired Cognition`
- 🔗URL: [https://github.com/zorazrw/odex](https://github.com/zorazrw/odex)
- Feature: execution-based exaluation; open-domain code generation
- Details:  ODEX has 945 NL-Code pairs spanning 79 diverse libraries, along with 1,707 human-written test cases for execution.
- Supported Metric: `pass@k`; `BLEU`; `ROUGE`; `METEOR`; `ChrF`; `BLEU`
- Test Case: ✅
- 🔏Input (NL)
  + 🚩Language: `English`; `Spanish`; `Japanese`; `Russian`
  + 🌟Format
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
    * [ ] Data Analysis and Manipulation
    * [ ] Plotting
    * [ ] Mathematical
    * [ ] Chemical
    * [ ] Educational
    * [x] Open-domain Execution
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

[^odex]: [https://arxiv.org/pdf/2212.10481.pdf](https://arxiv.org/pdf/2212.10481.pdf)
