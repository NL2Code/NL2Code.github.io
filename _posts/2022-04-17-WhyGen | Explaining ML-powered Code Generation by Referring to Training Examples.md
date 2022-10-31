---
title: WhyGen | Explaining ML-powered Code Generation by Referring to Training Examples
author: coder
date: 2022-04-17 00:00:00 +0800
categories: [ACM, ICSE]
tags: [methods]
math: true
image:
  path: /assets/imgs/WhyGen.png
  width: 800
  height: 500
  alt: The workflow of WhyGen to explain DNN-powered code generation by examples.
---

## 🌸Method

- 📙Title: [WhyGen Explaining ML-powered Code Generation by Referring to Training Examples](https://arxiv.org/pdf/2204.07940.pdf)
- 📚Publisher/Date: `ICSE/2022`
- 🏠Author Affiliation: Beijing University of Posts and Telecommunications
- 🔗URL: [https://github.com/WeixiangYAN/WhyGen](https://github.com/WeixiangYAN/WhyGen)
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
    * [x] Unsupervised Transfer Learning
    * [ ] Reinforcement Learning (RL)
    * [ ] Multi-task Learning
    * [ ] Meta Learning
    * [ ] Contrastive Learning
    * [x] Retrieved-based Learning
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
    * [x] Interpretability
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
    * [ ] Warnings, Errors, Bugs and Debug Infos
    * [ ] API Document
    * [ ] Official Tutorial
    * [ ] Abstract Syntax Tree (AST)
    * [ ] Data/Control Flow (DF/CF)
    * [ ] Variable 
    * [ ] PL keywords
    * [ ] Code Comment
    * [x] Natural Language to Code Pairs
    * [ ] Other Resources
  + 🚀Platform
    * [x] GitHub
    * [ ] Gitee
    * [ ] StackOverFlow
    * [ ] CodeForces
    * [ ] LeetCode
    * [ ] Google Code
    * [ ] Other Platform
- 🗂️Downstream Benchmark
  + PY150[^py150]
- ✈️Relevant Model
  + CodeGPT[^codegpt]
- 💕Contribution
  + `WhyGen` explains the generated code by referring to training examples.
  + Our experiments have shown that `WhyGen` is able to precisely notify the users about possible recitations and highly similar imitations with a top-10 accuracy of 81.21%. The demo video can be found at [https://youtu.be/EtoQP6850To](https://youtu.be/EtoQP6850To).

## 📘Reference

[^py150]: [https://raw.githubusercontent.com/microsoft/CodeXGLUE/main/Code-Code/CodeCompletion-line/dataset/py150/line_completion/test.json](https://raw.githubusercontent.com/microsoft/CodeXGLUE/main/Code-Code/CodeCompletion-line/dataset/py150/line_completion/test.json)
[^codegpt]: [https://microsoft.github.io/CodeXGLUE](https://microsoft.github.io/CodeXGLUE)
