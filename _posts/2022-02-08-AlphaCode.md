---
title: AlphaCode
author: coder
date: 2022-02-08 00:00:00 +0800
categories: [Science]
tags: [models]
math: true
pin: false
---

- 📙Paper: [Competition-level code generation with AlphaCode](https://www.science.org/doi/full/10.1126/science.abq1158)
- 📚Publisher: `Science`
- 🏠Author Affiliation: `Deepmind`
- 🌐Architecture
  + [x] Encoder-Decoder
  + [ ] Decoder-Only
- 📏Model Size
  + `284M`; `1.1B`; `2.8B`; `8.7B`; `41.1B`
- 🗂️Data pre-processing
  + Data Resource
    * Our pre-training dataset is based on a snapshot of selected public GitHub repositories taken on 2021/07/14.
  + De-duplication: ✅
  + Filter Strategies
    * We filtered out files which were likely auto-generated
    * all files larger than 1MB
    * lines longer than 1000 characters
- 🍉Tokenizer
  + Technology
    * [ ] Byte-level Byte-Pair-Encoding (BBPE)
    * [x] SentencePiece
  + Details: /
- 🧪Hyperparameters (AlphaCode 41.1B)
  + optimizer: AdamW
    * eps: 0.9, 0.95
    * bs: /
  + batch size: `2,048`
  + context window: `6,144`
  + gradient accumulation steps: \
  + warmup steps: `1,000`
  + learning rate: `1e-4`
  + weight decay: `0.1`
  + decay schedule
    * [x] Cosine
    * [ ] Linear
    * [ ] Polynomial
    * [ ] Inverse Square
  + precision floating point: `bf16`
- 🏃‍♀️Training
  + model initialization: /
  + training strategies
    * [x] left-to-right
    * [ ] fill-in-the-middle
  + trained tokens/steps: 967B tokens
  + hardware: TPUv4
  + training time: /
