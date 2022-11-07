---
title: Time-Efficient Code Completion Model for the R Programming Language
author: coder
date: 2021-08-01 00:00:00 +0800
categories: [ACL, NLP4Prog]
tags: [benchmarks]
math: true
---

> Note that the code completion task is considered a ranking problem in this paper, and we only report the `nl2code` related parts.
{: .prompt-tip }

## 📙Proposed Benchmark

- Benchmark Name: `RCED`[^rced]
- 📚Publisher/Date: `ACL/2021`
- 🏠Author Affiliation: JetBrains s.r.o; Lomonosov Moscow State University; ITMO University; Moscow Institute of Physics and Technology
- 🔗URL: [https://github.com/arti32lehtonen/rcompletion_evaluation_dataset](https://github.com/arti32lehtonen/rcompletion_evaluation_dataset)
- Details: The dataset used for the model training consists of `500k` R Markdown files (Rmd). Non-code information is erased from each file and the rest of the text is transformed into a script. Additionally, in one of the experiments we use a larger dataset that contains more than 4kk with both R and Rmd files. The evaluation dataset was collected from the Github open-source projects and consists of `35k` examples from the 9k R files. There is an issue with the using of the open-source project codes for the evaluation. It is very likely for the training and the test sets to intersect. A lot of repositories have forks with minimal differences and it is very hard to distinguish them from the source one. That is why we evaluate most of our models on R files only while training on Rmd files to avoid encountering the training samples in the test set.
- Supported Metric: `MRR`; `Recall@5`; `time` (They are all not metrics for nl2code)
- Test Case: ❌
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
  + 🚩Language: `R`
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
    * [ ] Line Level
    * [ ] Span Level
    * [ ] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [x] Other Levels

## 📘Reference

[^rced]: https://github.com/arti32lehtonen/rcompletion_evaluation_dataset
