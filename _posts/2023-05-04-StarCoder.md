---
title: StarCoder
author: coder
date: 2023-05-04 00:00:00 +0800
categories: [arxiv]
tags: [models]
math: true
pin: false
---

- 📙Paper: [StarCoder may the source be with you](https://drive.google.com/file/d/1cN-b9GnWtHzQRoE7M7gAEyivY0kl4BYs/view)
- 📚Publisher: `Arxiv`
- 🏠Author Affiliation: `Hugging Face`
- 🔑Public: ✅
- 🌐Architecture
  + [ ] Encoder-Decoder
  + [x] Decoder-Only
- 📏Model Size
  + `15.5B`
- 🗂️Data pre-processing
  + Data Resource
    * The Stack
  + De-duplication: ✅
- 🍉Tokenizer
  + Technology
    * [x] Byte-level Byte-Pair-Encoding (BBPE)
    * [ ] SentencePiece
  + Details
    *  we use the Hugging Face Tokenizers library (MOI et al., 2022) to train a byte-level Byte-Pair-Encoding with a vocabulary size of 49,152 tokens — including the sentinel tokens. The pre-tokenization step includes a digit-splitter and the regex splitter from the GPT-2 pre-tokenizer.
- 🧪Hyperparameters (StarCoder 15.5B)
  + optimizer: Adam
    * betas: 0.9
    * eps: 0.95
  + batch size: `4M`
  + context window: `8K`
  + gradient accumulation steps: /
  + warmup steps: `1000`
  + learning rate: `5e-5`
  + weight decay: `0.1`
  + decay schedule
    * [x] Cosine
    * [ ] Linear
    * [ ] Polynomial
    * [ ] Inverse Square
  + precision floating point: Since it requires the gradient reduction step in FP32, the training in BF16 leads to 10% lower throughput than FP16, but we used it anyway to avoid training instabilities.
- 🏃‍♀️Training
  + model initialization: `StarCoderBase`
  + training strategies
    * [ ] left-to-right
    * [x] fill-in-the-middle
  + trained tokens/steps: 35B Python tokens
  + hardware: We trained our model on a GPU cluster with 512 A100 80 GB GPUs distributed across 64 nodes. We partitioned the model with a 3D-parallel layout that shards the model with both tensor and pipeline parallelism rank 4, requiring 16 GPUs (two nodes) for one replica. To fully leverage the cluster’s capabilities, we used 32-fold data parallelism. To optimize GPU utilization and reduce idle compute bubbles, we maintained a micro-batch size of 1 and accumulated for 16 steps, resulting in a global batch size of 512 (equivalent to 4M tokens).
  + training time: /
