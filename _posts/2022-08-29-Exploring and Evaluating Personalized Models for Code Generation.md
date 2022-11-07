---
title: Exploring and Evaluating Personalized Models for Code Generation
author: coder
date: 2022-08-29 00:00:00 +0800
categories: [FSE]
tags: [methods]
math: true
image:
  path: /assets/imgs/customization-approach.png
  width: 800
  height: 500
  alt: Overview of the Customization Approaches.
---

## 🌸Method

- 📙Title: [Exploring and Evaluating Personalized Models for Code Generation](https://arxiv.org/pdf/2208.13928.pdf)
- 📚Publisher/Date: `FSE/2022`
- 🏠Author Affiliation: McGill University; Anthropic; Microsoft
- 🔗URL: `None`
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
    * [x] Prompt/Adapt/LoRA Learning
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
    * [x] Test Cases
    * [x] Repositories
    * [ ] Warnings, Errors, Bugs and Debug Infos
    * [ ] API Document
    * [x] Official Tutorial
    * [ ] Abstract Syntax Tree (AST)
    * [ ] Data/Control Flow (DF/CF)
    * [ ] Variable 
    * [ ] PL keywords
    * [ ] Code Comment
    * [ ] Natural Language to Code Pairs
    * [ ] Jupyter Notebook
    * [ ] Other Resources
  + 🚀Platform&Tool
    * [x] GitHub
    * [ ] Gitee
    * [ ] StackOverFlow
    * [ ] CodeForces
    * [ ] LeetCode
    * [ ] Google Code
    * [ ] Modulo Static Analysis Tool
    * [ ] Other Platform
- 🗂️Downstream Benchmark
  + 20 GitHub repositories
- 💕Contribution
  + We consider three key approaches: (i) custom fine-tuning; (ii) lightweight fine-tuning;  (iii) prefix tuning.
  + We compare these fine-tuning strategies for code generation and discuss the potential generalization and cost benefits of each in various deployment scenarios.
