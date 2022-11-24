---
title: DS-1000 | A Natural and Reliable Benchmark for Data Science Code Generation
author: coder
date: 2022-11-18 00:00:00 +0800
categories: [arxiv]
tags: [benchmarks]
math: true
image:
  path: /assets/imgs/DS-1000.png
  width: 800
  height: 500
  alt: An example problem in DS-1000.
---

## 📙Proposed Benchmark 

- Benchmark Name: `DS-1000`[^ds1000]
- 📚Publisher/Date: Arxiv/2022
- 🏠Author Affiliation: The University of Hong Kong; Peking University; Stanford University; University of California; University of Washington; Meta AI; Carnegie Mellon University
- 🔗URL: [https://ds1000-code-gen.github.io](https://ds1000-code-gen.github.io)
- Feature: Data Science Code Generation
- Details: DS-1000 contains 1000 problems originating from 451 unique StackOverflow problems. To defend against potential memoriza- tion, more than half of the DS-1000 problems are modified from the original StackOverflow problems; they include 152 surface perturbations, 235 semantic perturbations, and 162 difficult rewrites.

![Window shadow](/assets/imgs/DS-statistics.jpeg){: .shadow width="1548" height="864" .w-75 }
_Statistics of the two TCG datasets._

- Supported Metric: `pass@k`
- Test Case: ✅
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

## 📘Reference

[^ds1000]: [https://arxiv.org/pdf/2211.11501.pdf](https://arxiv.org/pdf/2211.11501.pdf)
