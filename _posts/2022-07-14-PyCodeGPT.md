---
title: PyCodeGPT
author: coder
date: 2022-07-14 00:00:00 +0800
categories: [IJCAI]
tags: [models]
math: true
pin: false
---

- 📙Paper: [CERT Continual Pre-Training on Sketches for Library-Oriented Code Generation](https://arxiv.org/pdf/2206.06888.pdf)
- 📚Publisher: `IJCAI`
- 🏠Author Affiliation: `Microsoft`
- 🔑Public: ✅
- 🌐Architecture
  + [ ] Encoder-Decoder
  + [x] Decoder-Only
- 📏Model Size
  + `110M`
- 🗂️Data pre-processing
  + Data Resource
    * We first crawl 7.6M repository pages hosted on GitHub. Then we consider the language distribution tags in each page to filter the repositories without Python files. As a result, we obtain 1.2M Python-related repository URLs. With the filtered repository URLs, we download all the contents of each repository from GitHub. Following Codex, we remove files over 1MB, as experienced developers usually avoid creating large source code files to maintain good readability. As a result, we get 60.6M raw Python files under 1MB, with a total size of 330GB. Among these files, we further filter out duplicated files, which has been recognized as an important step by CodeParrot. Finally, the number of unique files is reduced to 13.0M, with a total size of 96GB.
  + De-duplication: ✅
  + Filter Strategies
    * Conditions: lines of code ≥ 5, average line length ≤ 100, maximum line length ≤1000, and alphanumeric rate ≥ 0.98.  Note that, the fourth condition is applied after removing comments with alphanumeric rate < 0.5, which is one of the following strategies
    * We also remove the automatically generated or meaningless files, for example, files with the name init .py, setup.py or pb2.py, because these files can mislead the model during training. In addition, we remove some useless contexts from the Python files. Specifically, we remove the contexts of license description and comments with alphanumeric rate < 0.5, where license description appears as a comment in the head of the code
    * To ensure the training quality, we design two methods to perform Python syntax checking. The first method is to use Python’s built-in module ast to check the correctness of the syntax. This strategy filter out non-Python files largely, even if the file name ends with .py. The second method applies pattern matching to leave files containing more than two typical Python keywords (e.g., def, if, return, and for)
- 🍉Tokenizer
  + Technology
    * [x] Byte-level Byte-Pair-Encoding (BBPE)
    * [ ] SentencePiece
  + Details
    * We train a new BBPE tokenizer from scrach on the collected code data.
- 🧪Hyperparameters (PyCodeGPT 110M)
  + optimizer: AdamW
    * eps: 0.9, 0.95
    * bs: 1e-8
  + batch size: 480K tokens
  + context window: `1,024`
  + gradient accumulation steps: `4`
  + warmup steps: `1,000`
  + learning rate: `5e-4`
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
    * [x] left-to-right
    * [ ] fill-in-the-middle
  + trained tokens/steps: 100B tokens or 200K steps
  + hardware: a cluster of 16 NVIDIA V100 GPUs with 32GB memory.
  + training time: about 2 days
