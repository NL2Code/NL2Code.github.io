---
title: Unified Pre-training for Program Understanding and Generation
author: coder
date: 2021-04-10 00:00:00 +0800
categories: [NAACL]
tags: [methods, models]
math: true
pin: false
---

## 🌸Method

- 📙Title: [Unified Pre-training for Program Understanding and Generation](https://arxiv.org/pdf/2103.06333.pdf)
- 📚Publisher/Date: `NAACL/2021`
- 🏠Author Affiliation: `University of California, Los Angeles`; `Columbia University`
- 🌐Neural Network (NN)
  + ⚒️Architecture
    * [ ] Feedforward NN (FNN)
    * [ ] Convolutional NN (CNN)
    * [ ] Recurrent NN (RNN)
    * [ ] Long Short-Term Memory Neural Networks (LSTM)
    * [ ] Deep Belief Networks (DBN)
    * [ ] Variational Autoencoders (VAE)
    * [ ] Generative Adversarial Networks (GAN)
    * [ ] Diffussion
    * [x] Transformer-based Neural Networks including Encode and Decode
    * [ ] Other
  + ⚙️How to learn
    * [ ] Supervised Transfer Learning
    * [x] Unsupervised Transfer Learning
    * [ ] Reinforcement Learning (RL)
    * [ ] Multi-task Learning
    * [ ] Meta Learning
    * [ ] Contrastive Learning
    * [ ] Retrieved-based Learning
    * [ ] Other
  + 🧬Paradigm
    * [ ] Non-pre-train
    * [x] Pre-train and Fine-tune
    * [ ] Zero-shot Learning
    * [ ] One/two/few-shot Learning
    * [ ] In-context Learning
    * [ ] Prompt/Adapt/LoRA Learning
    * [ ] Other
  + 🛳️Other Directions of NN
    * [ ] Model Compression
    * [ ] Social Bias
    * [ ] Interpretability
    * [ ] Multi-Modal
    * [ ] Other
- 🧑🏻‍💻Software Engineering (SE)
  + [ ] Software Development
  + [ ] Intergrated Development Environment (IDE) and Tool
  + [ ] Software Maintenance
  + [ ] Other
- 🤖Programming Language (PL)
  + 🪪Characteristics
    * [ ] Executable
    * [ ] Dynamic/Statical PL
    * [ ] Procedure/Object/Aspect Orient PL
    * [ ] Other Characteristics
  + 🪵Resource
    * [x] Code Files
    * [ ] Test Cases
    * [ ] Repositories
    * [ ] Bugs and Debug Infos
    * [ ] API Document
    * [ ] Official Tutorial
    * [ ] Abstract Syntax Tree (AST)
    * [ ] Data/Control Flow (DF/CF)
    * [ ] Variable 
    * [ ] PL keywords
    * [ ] Code Comment
    * [ ] Other Resources
  + 🚀Platform
    * [x] GitHub
    * [ ] Gitee
    * [ ] StackOverFlow
    * [ ] CodeForces
    * [ ] LeetCode
    * [ ] Other Platform
- 🗂️Downstream Benchmark
  + CodeXGLUE[^codexglue]
- ✈️Base Model
  + PLBART
- 💕Contribution
  + They introduce PLBART (Program and Language BART), a bidirectional and autoregressive transformer pre-trained on unlabeled data across PL and NL to learn multilingual representations applicable to a broad spectrum of PLUG applications.

## 🎃Proposed Model

- Model Name: `PLBART`
- Publisher/Date: `NAACL/2021`
- Author Affiliation: University of California, Los Angeles; Columbia University
- Architecture: `Transformer-based neural networks (encoder-decoder)`
- Traing Corpus: `GitHub repositories on Google BigQuery`； `StackOverflow posts`
- Supported Natural Language: (Mostly) `English`
- Supported Programming Language: `Java`; `Python`
- Model Size: `140M`
- Public Item: `checkpoint`; `training data`; `training code`; `inference code`
- 🔗URL: [https://github.com/wasiahmad/PLBART](https://github.com/wasiahmad/PLBART)

## 📘Reference

[^codexglue]: https://microsoft.github.io/CodeXGLUE
