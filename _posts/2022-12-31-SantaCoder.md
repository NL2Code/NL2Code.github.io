---
title: SantaCoder
author: coder
date: 2022-12-31 00:00:00 +0800
categories: [arxiv]
tags: [models]
math: true
pin: false
---

- 📙Paper: [SantaCoder don't reach for the stars!](https://arxiv.org/pdf/2301.03988.pdf)
- 📚Publisher: `arxiv`
- 🏠Author Affiliation: `huggingface`
- 🔑Public: ✅
- 🌐Architecture
  + [ ] Encoder-Decoder
  + [x] Decoder-Only
- 📏Model Size
  + `1.1B`
- 🗂️Data pre-processing
  + Data Resource
    * The Stack v1.1
  + De-duplication: ✅
  + Filter Strategies
    * removing data from opt-out requests, near-deduplication, PII-redaction
    * filtering based on line-length and percentage of alphanumeric characters
    * removing files that contained test-samples from the following benchmarks: HumanEval, APPS, MBPP, MultiPL-E
- 🍉Tokenizer
  + Technology
    * [x] Byte-level Byte-Pair-Encoding (BBPE)
    * [ ] SentencePiece
  + Details
    * We train a HuggingFace Tokenizer on 600k rows (around 2.6GB) of data.
- 🧪Hyperparameters (SantaCoder 1.1B)
  + optimizer: Adam
    * betas: 0.9, 0.95
    * eps: 1e-8
  + global batch-size: `192`
  + context window: /
  + gradient accumulation steps: /
  + warmup steps: /
  + learning rate: `2e-4`
  + weight decay: `0.1`
  + decay schedule
    * [x] Cosine
    * [ ] Linear
    * [ ] Polynomial
    * [ ] Inverse Square
  + precision floating point: `fp16`
- 🏃‍♀️Training
  + model initialization: from scratch
  + training strategies
    * [ ] left-to-right
    * [x] fill-in-the-middle
  + trained tokens/steps: 118B tokens
  + hardware: 96 Tesla V100 GPUs
  + training time: Each training run takes 3.1 days
