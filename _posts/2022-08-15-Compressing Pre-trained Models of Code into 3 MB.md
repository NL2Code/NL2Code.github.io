---
title: Compressing Pre-trained Models of Code into 3 MB
author: coder
date: 2022-08-15 00:00:00 +0800
categories: [ACM, ASE]
tags: [methods]
math: true
image:
  path: /assets/imgs/compress-model.png
  width: 800
  height: 500
  alt: This figure illustrates an overview of the proposed model compression approach.
---

> Note that we only report the `nl2code` related parts, the paper do not have any `nl2code` related downstream tasks, and the proposed model is focusing code understanding and can not be used directly for code generation.
{: .prompt-tip }

## 🌸Method

- 📙Title: [Compressing Pre-trained Models of Code into 3 MB](https://arxiv.org/pdf/2208.07120.pdf)
- 📚Publisher/Date: `ASE/2022`
- 🏠Author Affiliation: Singapore Management University
- 🔗URL: `https://github.com/soarsmu/Compressor`
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
    * [ ] Non-pre-train
    * [x] Pre-train and Fine-tune
    * [ ] Zero-shot Learning
    * [ ] One/two/few-shot Learning
    * [ ] In-context Learning
    * [ ] Prompt/Adapt/LoRA Learning
    * [ ] Other
  + 🛳️Other Directions of NN
    * [x] Model Compression
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
    * [x] Code Files
    * [ ] Test Cases
    * [ ] Repositories
    * [ ] Warnings, Errors, Bugs, Debug and Compilable Infos
    * [ ] API Document
    * [ ] Official Tutorial
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
- ✈️Relevant Model
  + CodeBERT
  + GraphCodeBERT
- 💕Contribution
  + Our work is the first to highlight the necessity of compressing pre-trained models of code and refine this problem into a model simplification process for pre-trained models.
  + We propose Compressor, a novel compression method via genetic algorithm (GA)-guided model simplification and knowledge distillation.
  + We implement Compressor and evaluate it with CodeBERT and GraphCodeBERT across two downstream tasks. The results validate the feasibility of compressing pre-trained models with a negligible performance penalty.
