---
title: CodeParrot
author: coder
date: 2021-11-01 00:00:00 +0800
categories: [other]
tags: [models]
math: true
pin: false
---

- 📙Paper: [CodeParrot](https://huggingface.co/codeparrot)
- 📚Publisher: `other`
- 🏠Author Affiliation: `huggingface`
- 🔑Public: ✅
- 🌐Architecture
  + [ ] Encoder-Decoder
  + [x] Decoder-Only
- 📏Model Size
  + `110M`; `1.5B`
- 🗂️Data pre-processing
  + Data Resource
    * CodeParrot dataset
  + De-duplication: ✅
  + Filter Strategies
    * \> 1MB
    * max line length \> 1000
    * mean line length \> 100
    * fraction of alphanumberic characters \< 0.25
    * containing the word "auto-generated"
    * similar in the first 5 lines
- 🍉Tokenizer
  + Technology
    * [x] Byte-level Byte-Pair-Encoding (BBPE)
    * [ ] SentencePiece
  + Details
    * Trained GPT-2 tokenizer on the training split
- 🧪Hyperparameters (CodeParrot 1.5B)
  + optimizer: AdamW
    * eps: 0.9, 0.999
    * bs: 1e-8
  + batch size: `512` or `524K` tokens
  + context window: `1,024`
  + gradient accumulation steps: `16`
  + warmup steps: `750`
  + learning rate: `5e-5`
  + weight decay: `0.1`
  + decay schedule
    * [x] Cosine
    * [ ] Linear
    * [ ] Polynomial
    * [ ] Inverse Square
  + precision floating point: /
- 🏃‍♀️Training
  + model initialization: from scratch
  + training strategies
    * [x] left-to-right
    * [ ] fill-in-the-middle
  + trained tokens/steps: 30K steps or 41B tokens
  + hardware: 16 x A100 (40GB)
  + training time: /
