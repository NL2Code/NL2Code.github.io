---
title: CodeSearchNet Challenge | Evaluating the State of Semantic Code Search
author: coder
date: 2019-09-20 00:00:00 +0800
categories: [arxiv]
tags: [benchmarks, metrics]
math: true
pin: false
---

## 📚Proposed Benchmark

- Benchmark Name: `CodeSearchNet`
- Publisher/Date: `Arxiv/2019`
- Author Affiliation: `Github`; `Microsoft Research`
- 🔗URL: [https://github.com/github/CodeSearchNet](https://github.com/github/CodeSearchNet)
- Feature: This benchmark was originally intended for code retrieval and can also be used for code generation.
- Details: To enable evaluation of progress on code search, we are releasing the `CodeSearchNet` Corpus and are presenting the `CodeSearchNet` Challenge, which consists of `99` natural language queries with about `4k` expert relevance annotations of likely results from CodeSearchNet Corpus. The corpus contains about `6` million functions from open-source code spanning six programming languages (Go, Java, JavaScript, PHP, Python, and Ruby). The CodeSearchNet Corpus also contains automatically generated query-like natural language for `2` million functions, obtained from mechanically scraping and preprocessing associated function documentation.
- Supported Metric: `Mean Reciprocal Rank (MRR)`[^mrr]
- 🔏Input (NL)
  + 🚩Language: `English`
  + 🌟Format
    * [ ] Code Context
    * [x] Plain Natural Language
    * [ ] Competition Problem
    * [ ] Code Comment
    * [ ] TODO
    * [ ] Other Formats
  + 💈Description Granularity
    * [ ] Why? (Background)
    * [x] What? (Requirement, TODO)
    * [ ] How? (Algorithm Process)
    * [ ] Other Granularities
- 🔑Output (code)
  + 🚩Language: `Go`; `Java`; `JavaScript`; `PHP`; `Python`; `Ruby`
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
  + 🎯Level
  	* [ ] Token Level
    * [x] Line Level
    * [x] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 📘Reference

[^mrr]: [https://en.wikipedia.org/wiki/Mean_reciprocal_rank](https://en.wikipedia.org/wiki/Mean_reciprocal_rank)
