---
title: PanGu-Coder
author: coder
date: 2022-06-22 00:00:00 +0800
categories: [arxiv]
tags: [models]
math: true
pin: false
---

- 📙Paper: [PanGu-Coder Program Synthesis with Function-Level Language Modeling](https://arxiv.org/pdf/2207.11280.pdf)
- 📚Publisher: `arxiv`
- 🏠Author Affiliation: `Huawei`
- 🔑Public: ❌
- 🌐Architecture
  + [ ] Encoder-Decoder
  + [x] Decoder-Only
- 📏Model Size
  + `317M`; `2.6B`
- 🗂️Data pre-processing
  + Data Resource
    * The initial dataset was collected through GHTorrent, an online tool that collects and stores Github public event metadata. In an effort to make our pre-training data comparable to previous work, we focused exclusively on Github repositories established before May 2021.
  + De-duplication: ✅
  + Filter Strategies
    * To establish data quality, we only kept the collected files that met the following criteria:  the file size is under 1MB;
    * the code is Python3 compatible, as determined through its Abstract Syntactic Tree (AST);
    * there are fewer than 100 characters per line on average;
    * and there are fewer than 1,000 characters in any single line.
- 🍉Tokenizer
  + Technology
    * [ ] Byte-level Byte-Pair-Encoding (BBPE)
    * [x] SentencePiece
  + Details
    * /
- 🧪Hyperparameters (PanGu-Coder 2.6B)
  + optimizer: Adam
    * betas: 0.9, 0.95
    * eps: /
  + batch size: `256`
  + context window: `1,024`
  + gradient accumulation steps: /
  + warmup steps: /
  + learning rate: /
  + weight decay: `0.01`
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
  + trained tokens/steps: 387B tokens
  + hardware: Nvidia V100 GPU
  + training time: /
