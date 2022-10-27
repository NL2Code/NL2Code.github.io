---
title: CodeXGLUE | A Machine Learning Benchmark Dataset for Code Understanding and Generation
author: coder
date: 2021-05-16 00:00:00 +0800
categories: [arxiv]
tags: [benchmarks, models]
math: true
pin: false
---

## 🎃Proposed Model

- Model Name: `CodeGPT`
- Publisher/Date: `Arxiv/2021`
- Author Affiliation: Peking University; Sun Yat-sen University; Beihang University; Microsoft
- Architecture: `Transformer-based neural networks (decoder)`
- Traing Corpus: `CodeSearchNet`[^codesearchnet]
- Supported Natural Language: `English`
- Supported Programming Language: `Java`; `Python`
- Model Size: `CodeGPT-small`
- Public Item: `checkpoint`
- 🔗URL: [https://huggingface.co/microsoft/CodeGPT-small-java-adaptedGPT2](https://huggingface.co/microsoft/CodeGPT-small-java-adaptedGPT2)

## 📚Proposed Benchmark

- Benchmark Name: [CodeXGLUE](https://arxiv.org/pdf/2102.04664.pdf)
- Publisher/Date: `Arxiv/2021`
- Author Affiliation: Peking University; Sun Yat-sen University; Beihang University; Microsoft
- 🔗URL
  + [https://github.com/microsoft/CodeXGLUE](https://github.com/microsoft/CodeXGLUE)
  + [https://microsoft.github.io/CodeXGLUE](https://microsoft.github.io/CodeXGLUE/)
- Sub-benchmark
  + PY150[^py150]
  + CONCODE[^concode]
- Feature: CodeXGLUE is a benchmark dataset and open challenge for code intelligence. It includes a collection of code intelligence tasks and a platform for model evaluation and comparison. CodeXGLUE stands for General Language Understanding Evaluation benchmark for CODE. It includes 14 datasets for 10 diversified code intelligence tasks.
- Details: Please refer [the origin paper](https://arxiv.org/pdf/2102.04664.pdf) for more details.
- Supported Metric: `EM`; `ES`; `Accuracy`; `BLEU`; `CodeBLEU`
- Test Case： ❌
- 🔏Input (NL)
  + 🚩Language: `English`
  + 🌟Format
    * [x] Code Context
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
- 🔑Output (code)
  + 🚩Language: `Python`; `Java`
  + ⛺Domain
    * [x] General
    * [ ] Mathematical
    * [ ] Chemical
    * [ ] Educational
    * [ ] Other Domains
  + 👑Library
    * [x] Public Library
    * [ ] Private Library
  + 🎯Level
    * [x] Token Level
    * [ ] Line Level
    * [x] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 📘Reference

[^py150]: [https://raw.githubusercontent.com/microsoft/CodeXGLUE/main/Code-Code/CodeCompletion-line/dataset/py150/line_completion/test.json](https://raw.githubusercontent.com/microsoft/CodeXGLUE/main/Code-Code/CodeCompletion-line/dataset/py150/line_completion/test.json)
[^concode]: [https://arxiv.org/abs/1808.09588](https://arxiv.org/abs/1808.09588)
[^codesearchnet]: [https://arxiv.org/pdf/1909.09436](https://arxiv.org/pdf/1909.09436)
