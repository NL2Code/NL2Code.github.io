---
title: PolyCoder
author: coder
date: 2022-02-26 00:00:00 +0800
categories: [other]
tags: [models]
math: true
pin: false
---

- 📙Paper: [A systematic evaluation of large language models of code](https://dl.acm.org/doi/abs/10.1145/3520312.3534862)
- 📚Publisher: `MAPS`
- 🏠Author Affiliation: `Carnegie Mellon University`
- 🔑Public: ✅
- 🌐Architecture
  + [ ] Encoder-Decoder
  + [x] Decoder-Only
- 📏Model Size
  + `160M`; `400M`; `2.7B`
- 🗂️Data pre-processing
  + Data Resource
    * We cloned the most popular repositories for 12 popular programming languages with at least 50 stars (stopping at about 25K per language to avoid a too heavy skew towards popular programming languages) from GitHub in October 2021. For each project, each file belonging to the majority-language of that project was extracted, yielding the initial training set. This initial, unfiltered dataset spanned 631GB and 38.9M files.
  + De-duplication: ✅
  + Filter Strategies
    * They filter the files: \> 1MB;
    * \< 100 tokens.
- 🍉Tokenizer
  + Technology
    * [x] Byte-level Byte-Pair-Encoding (BBPE)
    * [ ] SentencePiece
  + Details
    * Trained GPT-2 tokenizer on a random 5% subset (all languages)
- 🧪Hyperparameters (PolyCoder 2.7B)
  + optimizer: AdamW
    * betas: 0.9, 0.999
    * eps: 1e-8
  + batch size: 262K tokens
  + context window: `2,048`
  + gradient accumulation steps: /
  + warmup steps: `1,600`
  + learning rate: `1.6e-4`
  + weight decay: /
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
  + trained tokens/steps: 39B tokens or 150K steps
  + hardware: 8 Nvidia RTX 8000 GPUs
  + training time: about 6 weeks
