---
title: Program Synthesis with Large Language Models
author: coder
date: 2021-07-14 00:00:00 +0800
categories: [arxiv]
tags: [models, benchmarks]
math: true
pin: false
---

## 🎃Proposed Model

- Model Name: `None`
- 📚Publisher/Date: `Arxiv/2021`
- 🏠Author Affiliation: `Google Research`
- Architecture: `Transformer-based neural networks (decoder)`
- Pre-Traing Corpus: This data included web sites with both computer code and text, such as question and answer sites and tutorials, but source code files themselves were not specifically included, except where code appeared in other web sites. These web sites with code and text comprised about 13.8M documents containing 18.7B BPE tokens out of the pre-training data.
- Supported Natural Language: `English`
- Supported Programming Language: `Python`
- Model Size: `244M`; `422M`; `1B`; `4B`; `8B`; `68B`; `137B`
- Public Item: `None`
- 🔗URL: `None`

## 📚Proposed Benchmark#1

- Benchmark Name: `MBPP`
- 📚Publisher/Date: `Arxiv/2021`
- 🏠Author Affiliation: `Google Research`
- 🔗URL: [https://github.com/google-research/google-research/tree/master/mbpp](https://github.com/google-research/google-research/tree/master/mbpp)
- Feature: The short language descriptions in mostly baic programming problems.
- Details: The Mostly Basic Programming Problems dataset contains 974 short Python programs constructed by crowd-sourcing to an internal pool of crowdworkers who have basic knowledge of Python. We asked crowd-sourcing participants to write a short problem statement, a single self-contained Python function solving the problem specified, and three test cases that check for semantic correctness of the function. Participants also provided a ground-truth solution that passes all three test cases. Participants were instructed to write descriptions concrete enough that a human would be able to translate them into code without clarifications. They were also instructed to write code that is self-contained (that is, it runs by itself) and that does not print any results to the console. Use of internet references was allowed.
- Supported Metric: `pass@100`
- Test Case： ✅
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
    * [x] What? (Requirement, TODO)
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
    * [x] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 📚Proposed Benchmark#2

- Benchmark Name: `MathQA-Python`
- 📚Publisher/Date: `Arxiv/2021`
- 🏠Author Affiliation: `Google Research`
- 🔗URL: [https://github.com/google/trax/blob/master/trax/examples/MathQA_Python_generation_notebook.ipynb](https://github.com/google/trax/blob/master/trax/examples/MathQA_Python_generation_notebook.ipynb)
- Feature: We translate the MathQA benchmark[^mathqa] into a Python program synthesis dataset by translating the ground-truth programs from the domain-specific language given in the paper to Python code (mostly straight-line code, but more complex natural language descriptions).
- Details: We are left with 23914 problems, of which we use 19209 for training, 2822 for validation and 1883 for testing. The translation between DSL and Python is straightforward and we supply code that can be used to perform it.
- Supported Metric: `pass@100`
- Test Case： ✅
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
    * [x] What? (Requirement, TODO)
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
    * [ ] Data Analysis and Manipulation
    * [ ] Plotting
    * [x] Mathematical
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
    * [ ] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 📘Reference

[^mathqa]: [https://arxiv.org/pdf/1905.13319.pdf](https://arxiv.org/pdf/1905.13319.pdf)
