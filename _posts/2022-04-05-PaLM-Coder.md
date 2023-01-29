---
title: PaLM-Coder
author: coder
date: 2022-04-05 00:00:00 +0800
categories: [arxiv]
tags: [models]
math: true
pin: false
---

- 📙Paper: [PaLM Scaling Language Modeling with Pathways](https://arxiv.org/pdf/2204.02311.pdf)
- 📚Publisher: `arxiv`
- 🏠Author Affiliation: `Google Research`
- 🔑Public: ❌
- 🌐Architecture
  + [ ] Encoder-Decoder
  + [x] Decoder-Only
- 📏Model Size
  + `8B`; `62B`; `540B`
- 🗂️Data pre-processing
  + Data Resource
    * The PaLM pretraining dataset consists of a high-quality corpus of 780 billion tokens that represent a wide range of natural language use cases. The dataset is a mixture of filtered webpages,2 books, Wikipedia, news articles, source code, and social media conversations.
    * PaLM-Coder: ExtraPythonData contains 5.8B tokens from GitHub repositories that were not used during pre-training.
  + De-duplication: ✅
  + Filter Strategies
    * We filter the files by the license included in the repository;
    * copyleft licenses were excluded;
    * filename extension to restrict to one of 24 common programming languages, including Java, HTML, Javascript, Python, PHP, C#, XML, C++, and C, which results in 196GB of source code.
- 🍉Tokenizer
  + Technology
    * [ ] Byte-level Byte-Pair-Encoding (BBPE)
    * [x] SentencePiece
  + Details
    * /
- 🧪Hyperparameters (PaLM-Coder 540B)
  + optimizer: Adafa.
    * betas: /
    * eps: /
  + batch size: PaLM 540B: we use batch size 512 (1M tokens) until step 50k, then double it to 1024 (2M tokens) until step 115k, and finally double again it to 2048 (4M tokens) until training is complete at step 255k. The smaller models followed similar schedules.
  + context window: `2,048`
  + gradient accumulation steps: /
  + warmup steps: /
  + learning rate: `1e-2`
  + weight decay: /
  + decay schedule
    * [ ] Cosine
    * [ ] Linear
    * [ ] Polynomial
    * [ ] Inverse Square
  + precision floating point: /
- 🏃‍♀️Training
  + model initialization: PaLM
  + training strategies
    * [x] left-to-right
    * [ ] fill-in-the-middle
  + trained tokens/steps: PaLM-Coder includes total 46.8B code tokens and 8.7B Python tokens. 
  + hardware: We use 3072 TPU v4 chips in each Pod attached to 768 hosts. This system, the largest TPU configuration described to date, allowed us to efficiently scale training to 6144 chips without needing to use any pipeline parallelism.
  + training time: We trained PaLM-540B on 6144 TPU v4 chips for 1200 hours and 3072 TPU v4 chips for 336 hours including some downtime and repeated steps
