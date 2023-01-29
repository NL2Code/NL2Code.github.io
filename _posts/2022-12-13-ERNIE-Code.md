---
title: ERNIE-Code
author: coder
date: 2022-12-13 00:00:00 +0800
categories: [arxiv]
tags: [models]
math: true
pin: false
---

- 📙Paper: [ERNIE-Code Beyond English-Centric Cross-lingual Pretraining for Programming Languages](https://arxiv.org/pdf/2212.06742.pdf)
- 📚Publisher: `arxiv`
- 🏠Author Affiliation: `Baidu`
- 🔑Public: ✅ (promise)
- 🌐Architecture
  + [x] Encoder-Decoder
  + [ ] Decoder-Only
- 📏Model Size
  + `560M`
- 🗂️Data pre-processing
  + Data Resource
    * CodeSearchNet
    * CC-100
    * OPUS
    * MultiUN
    * IIT
    * OPUS
    * WikiMatrix
  + De-duplication: ❌
  + Filter Strategies
    * /
- 🍉Tokenizer
  + Technology
    * [ ] Byte-level Byte-Pair-Encoding (BBPE)
    * [x] SentencePiece
  + Details
    * We add a set of tokens representing whitespace indentation of different lengths in PL
- 🧪Hyperparameters (ERNIE-Code 560M)
  + optimizer: AdaFa
    * eps: /
    * bs: /
  + batch size: a micro-batch size of 8/4
  + context window: `1,024`
  + gradient accumulation steps: `15`
  + warmup steps: `1,000`
  + learning rate: `1e-4`
  + weight decay: /
  + decay schedule
    * [ ] Cosine
    * [x] Linear
    * [ ] Polynomial
    * [ ] Inverse Square
  + precision floating point: `bf16`
- 🏃‍♀️Training
  + model initialization: `mT5`
  + training strategies
    * [x] left-to-right
    * [ ] fill-in-the-middle
  + trained tokens/steps: `100k` steps
  + hardware: 32 NVIDIA A100 GPUs with 40G memory
  + training time: 4 weeks
