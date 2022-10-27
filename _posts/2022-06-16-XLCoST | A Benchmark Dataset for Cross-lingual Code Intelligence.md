---
title: XLCoST | A Benchmark Dataset for Cross-lingual Code Intelligence
author: coder
date: 2022-06-16 00:00:00 +0800
categories: [arxiv]
tags: [benchmarks]
math: true
image:
  path: /assets/imgs/xlcost.png
  width: 800
  height: 400
  alt:  An illustration of the data and the tasks.
---

> Note that we only report the `nl2code` related parts.
{: .prompt-tip }

## 📙Proposed Benchmark

- Benchmark Name: `XLCoST`[^xlcost]
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: Virginia Tech
- 🔗URL: https://github.com/reddy-lab-code-research/XLCoST
- Feature: Cross-lingual code snippet dataset.
- Details: Our dataset contains fine-grained parallel data from `8` languages (`7` commonly used programming languages and English), and supports `10` cross-lingual code tasks.

  ![Window shadow](/assets/imgs/xlcost-2.png){: .shadow width="1200" height="500" .w-75 }
  _Comparison against other parallel code datasets (Py - Python, JS - JavaScript). Column "Size" refers to the number of parallel data pairs. *This number is for single programs, not pairs._

- Supported Metric: `BLEU`; `CodeBLEU`
- Test Case: ❌
- 🔏Input (NL)
  + 🚩Language: `English`
  + 🌟Format
    * [ ] Code Context
    * [x] Plain Natural Language
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
- 🔑Output (code)
  + 🚩Language: `C++`; `Java`; `Python`; `C#`; `JavaScript`; `PHP`; `C`
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
  	* [x] Token Level
    * [x] Line Level
    * [x] Span Level
    * [x] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 📘Reference

[^xlcost]: [https://arxiv.org/pdf/2206.08474.pdf](https://arxiv.org/pdf/2206.08474.pdf)
