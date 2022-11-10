---
title: Neural Attribute Machines for Program Generation
author: coder
date: 2017-05-25 00:00:00 +0800
categories: [arxiv]
tags: [methods]
math: true
image:
  path: /assets/imgs/NAM.png
  width: 800
  height: 500
  alt: (a) Vanilla RNN (b) NAM with context (c) Full NAM.
---

## 🌸Method

- 📙Title: [Neural Attribute Machines for Program Generation](https://arxiv.org/pdf/1705.09231.pdf)
- 📚Publisher/Date: `Arxiv/2017`
- 🏠Author Affiliation: Univ. of Wisconsin; GrammaTech, Inc.
- 🔗URL: `None`
- 🌐Neural Network (NN)
  + ⚒️Architecture
    * [ ] Feedforward NN (FNN)
    * [ ] Convolutional NN (CNN)
    * [x] Recurrent NN (RNN)
    * [x] Long Short-Term Memory Neural Networks (LSTM)
    * [ ] Deep Belief Networks (DBN)
    * [ ] Variational Autoencoders (VAE)
    * [ ] Generative Adversarial Networks (GAN)
    * [ ] Diffussion
    * [ ] Transformer-based Neural Networks including Encode and Decode
    * [ ] Other
  + ⚙️How to learn
    * [ ] Supervised Transfer Learning
    * [ ] Unsupervised Transfer Learning
    * [x] Self-Supervised Transfer Learning
    * [ ] Semi-Supervised Transfer Learning
    * [ ] Weak Supervised Transfer Learning
    * [ ] Reinforcement Learning (RL)
    * [ ] Multi-task Learning
    * [ ] Meta Learning
    * [ ] Contrastive Learning
    * [ ] Retrieved-based Learning
    * [ ] Other
  + 🧬Paradigm
    * [x] Non-pre-train
    * [ ] Pre-train and Fine-tune
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
    * [ ] Prompt Design
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
    * [ ] Code Files
    * [ ] Test Cases
    * [ ] Repositories
    * [ ] Warnings, Errors, Bugs, Debug and Compilable Infos
    * [ ] API Document
    * [ ] Official Tutorial
    * [x] Abstract Syntax Tree (AST)
    * [x] Data/Control Flow (DF/CF)
    * [x] Variable 
    * [ ] PL keywords
    * [ ] Code Comment
    * [x] Natural Language to Code Pairs
    * [ ] Jupyter Notebook
    * [ ] Programmatic Idioms
    * [ ] Other Resources
  + 🚀Platform&Tool
    * [ ] GitHub
    * [ ] Gitee
    * [ ] StackOverFlow
    * [ ] CodeForces
    * [ ] LeetCode
    * [ ] Google Code
    * [ ] Modulo Static Analysis Tool
    * [ ] Other Platform
- 🗂️Downstream Benchmark
  + This paper's dataset
- 💕Contribution
  + We present a new neural network and logical architecture that incorporates background knowledge in the form of attribute-grammar constraints.
  + We give a framework to train this new architecture that uses a three-valued loss function to penalize correct, incorrect-but-legal, and incorrect-and-illegal predictions differently.
  + Our experiments show the difficulties existing neural models have with learning in constrained domains, and the advantages of using the proposed framework.
