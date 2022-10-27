---
title: Programming Puzzles
author: coder
date: 2021-06-16 00:00:00 +0800
categories: [arxiv]
tags: [benchmarks]
math: true
image:
  path: /assets/imgs/P3.png
  width: 800
  height: 500
  alt: Programming puzzles ranging from trivial to longstanding open algorithmic challenges in multiple domains.
---

## 📙Proposed Benchmark

- Benchmark Name: `P3`[^ppp]
- 📚Publisher/Date: `Arxiv/2021`
- 🏠Author Affiliation: MIT; Allen Inst. for AI; Microsoft Research
- 🔗URL: [https://github.com/microsoft/PythonProgrammingPuzzles](https://github.com/microsoft/PythonProgrammingPuzzles)
- Feature: Each puzzle takes the form of a Python function that takes an answer as an argument. The answer is an input which makes the function return `True`.
- Details: `P3` uses Python, the de facto language of ML research, as the programming language for specifying puzzles. At the time of publication, `P3` currently has `397` problems.
- Supported Metric: `The number of solved problems`
- Test Case： ✅
- 🔏Input (NL)
  + 🚩Language: `English`
  + 🌟Format
    * [x] Code Context
    * [ ] Plain Natural Language
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
    * [x] Build-in Library
    * [ ] Public Library
    * [ ] Private Library
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

[^ppp]: [https://arxiv.org/pdf/2106.05784.pdf](https://arxiv.org/pdf/2106.05784.pdf)
