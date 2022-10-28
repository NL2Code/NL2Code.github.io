---
title: SPoC | Search-based Pseudocode to Code
author: coder
date: 2019-06-12 00:00:00 +0800
categories: [NeurIPS]
tags: [benchmarks]
math: true
image:
  path: /assets/imgs/SPOC.png
  width: 800
  height: 500
  alt: Datasets for natural language to code. In contrast to other datasets, our SPoC dataset contains human-authored pseudocode with a consistent granularity of description and test cases.
---

## 📙Proposed Benchmark

- Benchmark Name: `SPoC`[^spoc]
- 📚Publisher/Date: `NeurIPS/2019`
- 🏠Author Affiliation: Stanford University
- 🔗URL: [https://sumith1896.github.io/spoc](https://sumith1896.github.io/spoc)
- Details: We collected the `SPoC` dataset (Search-based Pseudocode to Code) containing `18,356` programs with human-authored pseudocode and test cases.
- Supported Metric: `accuracy`
- Test Case： ✅
- 🔏Input (NL)
  + 🚩Language: `English`
  + 🌟Format
    * [ ] Code Context
    * [ ] Plain Natural Language
    * [ ] Competition Problem
    * [ ] Code Comment
    * [ ] TODO
    * [x] Pseudocode
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
  + 🚩Language: `C++`
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

[^spoc]: [https://arxiv.org/pdf/1906.04908.pdf](https://arxiv.org/pdf/1906.04908.pdf)
