---
title: CodeT5 | Identifier-aware Unified Pre-trained Encoder-Decoder Models for Code Understanding and Generation
author: coder
date: 2021-09-02 00:00:00 +0800
categories: [EMNLP]
tags: [methods, models]
math: true
pin: false
---

## 🌸Method

- 📙Title: [CodeT5 Identifier-aware Unified Pre-trained Encoder-Decoder Models for Code Understanding and Generation](https://arxiv.org/pdf/2109.00859.pdf)
- 📚Publisher/Date: `EMNLP/2021`
- 🏠Author Affiliation: Salesfore Research Asia; Nanyang Technological University
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
    * [x] Supervised Transfer Learning
    * [ ] Unsupervised Transfer Learning
    * [ ] Self-Supervised Transfer Learning
    * [ ] Semi-Supervised Transfer Learning
    * [ ] Weak Supervised Transfer Learning
    * [ ] Reinforcement Learning (RL)
    * [x] Multi-task Learning
    * [ ] Meta Learning
    * [ ] Contrastive Learning
    * [ ] Retrieved-based Learning
    * [ ] Other
  + 🧬Paradigm
    * [ ] Non-pre-train
    * [x] Pre-train and Fine-tune
    * [x] Zero-shot Learning
    * [ ] One/two/few-shot Learning
    * [ ] In-context Learning
    * [ ] Prompt/Adapt/LoRA Learning
    * [ ] Other
  + 🛳️Other Directions of NN
    * [ ] Model Compression
    * [ ] Social Bias
    * [ ] Interpretability
    * [x] Multi-Modal
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
    * [x] Variable 
    * [x] PL keywords
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
  + CodeT5-small
  + CodeT5-base
- 💕Contribution
  + We present one of the first unified encoderdecoder models CodeT5 to support both coderelated understanding and generation tasks, and also allows for multi-task learning.
  + We propose a novel identifier-aware pretraining objective that considers the crucial token type information (identifiers) from code. Besides, we propose to leverage the NL-PL pairs that are naturally available in source code to learn a better cross-modal alignment.
  + Extensive experiments show that CodeT5 yields state-of-the-art results on the fourteen sub-tasks in CodeXGLUE. Further analysis shows our CodeT5 can better capture the code semantics with the proposed identifier-aware pre-training and bimodal dual generation primarily benefits NL↔PL tasks.

## 🎃Proposed Model

- Model Name: `CodeT5`
- 📚Publisher/Date: `EMNLP/2021`
- 🏠Author Affiliation: Salesfore Research Asia; Nanyang Technological University
- Architecture: `Transformer-based neural networks (encoder-decoder)`
- Traing Corpus: `CodeSearchNet`
- Supported Natural Language: (mostly) `English`
- Supported Programming Language: `Python`; `Ruby`; `JavaScript`; `Go`; `Java`; `PHP`; `C`; `C#`
- Model Size: `CodeT5-small`; `CodeT5-base`
- Public Item: `checkpoint`; `finetuning code`; `inference code`
- 🔗URL: [https://github.com/salesforce/CodeT5](https://github.com/salesforce/CodeT5)

## 📘Reference

[^codexglue]: [https://microsoft.github.io/CodeXGLUE](https://microsoft.github.io/CodeXGLUE)
