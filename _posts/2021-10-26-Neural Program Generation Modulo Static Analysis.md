---
title: Neural Program Generation Modulo Static Analysis
author: coder
date: 2021-10-26 00:00:00 +0800
categories: [NeurIPS]
tags: [methods, models]
math: true
---

## 🌸Method

- 📙Title: [Neural Program Generation Modulo Static Analysis](https://arxiv.org/pdf/2111.01633.pdf)
- 📚Publisher/Date: `NeurIPS/2021`
- 🏠Author Affiliation: Rice University; UT Austin; University of Wisconsin
- 🔗URL: [https://github.com/rohanmukh/nsg](https://github.com/rohanmukh/nsg)
- 🌐Neural Network (NN)
  + ⚒️Architecture
    * [ ] Feedforward NN (FNN)
    * [ ] Convolutional NN (CNN)
    * [ ] Recurrent NN (RNN)
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
    * [ ] Self-Supervised Transfer Learning
    * [ ] Semi-Supervised Transfer Learning
    * [x] Weak Supervised Transfer Learning
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
    * [ ] Other
- 🧑🏻‍💻Software Engineering (SE)
  + [ ] Software Development
  + [x] Intergrated Development Environment (IDE) and Tool
  + [ ] Software Maintenance
  + [ ] Other
- 🤖Programming Language (PL)
  + 🪪Characteristics
    * [ ] Executable
    * [ ] Dynamic/Statical PL
    * [x] Procedure/Object/Aspect Orient PL
    * [ ] Other Characteristics
  + 🪵Resource
    * [ ] Code Files
    * [ ] Test Cases
    * [ ] Repositories
    * [ ] Warnings, Errors, Bugs and Debug Infos
    * [x] API Document
    * [ ] Official Tutorial
    * [x] Abstract Syntax Tree (AST)
    * [ ] Data/Control Flow (DF/CF)
    * [x] Variable
    * [ ] PL keywords
    * [ ] Code Comment
    * [ ] Natural Language to Code Pairs
    * [x] Other Resources
  + 🚀Platform&Tool
    * [ ] GitHub
    * [ ] Gitee
    * [ ] StackOverFlow
    * [ ] CodeForces
    * [ ] LeetCode
    * [ ] Google Code
    * [x] Modulo Static Analysis Tool
    * [ ] Other Platform
- 🗂️Downstream Benchmark
  + NSG's data[^nsg]
- ✈️Relevant Model
  + GPT-Neo
  + CodeGPT
  + Codex
- 💕Contribution
  + We present a new approach to the generative modeling of source code that uses a static-analysis tool as a weak supervisor.
  + We embody this approach in the specific form of neurosymbolic attribute grammars (NSGs).
  + We evaluate the NSG approach on the long-horizon task of generating entire Java method bodies, and show that it significantly outperforms several larger, state-of-the-art transformer models.

## 🎃Proposed Model

- Model Name: `NSG`
- 📚Publisher/Date: `NeurIPS/2021`
- 🏠Author Affiliation: Rice University; UT Austin; University of Wisconsin
- Architecture: `LSTM`
- Traing Corpus: We implemented an NSG for our subset of Java. Here, attributes are used to keep track of the state of the symbol table, the expected return type of each method, expected types of actual parameters, variable initialization, whether the variable has been used, and whether the method has a return statement. The symbol table contains entries for all formal parameters, class variables, and internal methods within the class.
- Supported Natural Language: `English`
- Supported Programming Language: `Java`
- Model Size: `63M`
- Public Item: `training data`; `training code`; `inference code`
- 🔗URL: [https://github.com/rohanmukh/nsg](https://github.com/rohanmukh/nsg)

## 📘Reference

[^nsg]: [https://github.com/rohanmukh/nsg](https://github.com/rohanmukh/nsg)
