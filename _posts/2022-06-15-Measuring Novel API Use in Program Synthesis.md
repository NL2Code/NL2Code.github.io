---
title: Measuring Novel API Use in Program Synthesis
author: coder
date: 2022-06-15 00:00:00 +0800
categories: [arxiv]
tags: [benchmarks]
math: true
---

## 📙Proposed Benchmark

- Benchmark Name: `API Use`
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: Unknow
- 🔗URL: [https://github.com/ethanachi/api_use](https://github.com/ethanachi/api_use)
- Feature: The Synthetic API Use package aims to evaluate large language models (LLMs)' ability to perform tool use during code generation.
- Details: The benchmark consists of synthetic API's: synthetic Python libraries, each of which tests various facets of reasoning in code synthesis. An accompanying Python testbed generates programming problems which must be solved using functions from these synthetic API's. At evaluation time, a large language model is first presented with the definition of the API(s), then prompted to complete the programming problem using the functions it has seen.
- Supported Metric: `Not involved`
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
    * [ ] Why? (Background)
    * [x] What? (Requirement, Functionality, TODO)
    * [ ] How? (Algorithm Process)
    * [ ] Other Granularities
- 🔑Output (code)
  + 🚩Language: `Python`
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
