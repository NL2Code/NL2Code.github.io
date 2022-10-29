---
title: Generating Regular Expressions from Natural Language Specifications | Are We There Yet?
author: coder
date: 2018-06-01 00:00:00 +0800
categories: [AAAI]
tags: [benchmarks]
math: true
---

## 📙Proposed Benchmark

- Benchmark Name: `RegexLib`
- 📚Publisher/Date: `AAAI/2018`
- 🏠Author Affiliation: University of Illinois at Urbana-Champaign;  Xi’an Jiaotong University; Microsoft Research Asia
- 🔗URL: [https://regexlib.com](https://regexlib.com)
- Feature: Real world dataset
- Details: We collect a real-world dataset from `RegexLib`, an online library for regular expressions. The library includes various regular expressions and the corresponding NL descriptions contributed by authors of the regular expressions. For our study, we use all the `3,619` pairs of NL and regular expression that can be retrieved from the search interface of the library.
- Supported Metric: `Accuracy`
- Test Case: ❌
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
  + 🎯Additional Input
    * [x] None
    * [ ] Class Information
    * [ ] File Information
    * [ ] Repository Information
    * [ ] Other Information
- 🔑Output (code)
  + 🚩Language: `Regular Expression`
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
