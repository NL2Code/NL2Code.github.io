---
title: DeepFuzz | Automatic Generation of Syntax Valid C Programs for Fuzz Testing
author: coder
date: 2019-01-15 00:00:00 +0800
categories: [AAAI]
tags: [methods]
math: true
image:
  path: /assets/imgs/DeepFuzz.png
  width: 800
  height: 500
  alt: Workflow of DeepFuzz.
---

> Note that we only report the `nl2code` related parts.
{: .prompt-tip }

## 🌸Method

- 📙Title: [DeepFuzz | Automatic Generation of Syntax Valid C Programs for Fuzz Testing](https://faculty.ist.psu.edu/wu/papers/DeepFuzz.pdf)
- 📚Publisher/Date: `AAAI/2019`
- 🏠Author Affiliation: College of Information Sciences and Technology, The Pennsylvania State University, University Park
- 🔗URL: [https://github.com/s3team/DeepFuzz](https://github.com/s3team/DeepFuzz)
- 🌐Neural Network (NN)
  + ⚒️Architecture
    * [ ] Feedforward NN (FNN)
    * [ ] Convolutional NN (CNN)
    * [x] Recurrent NN (RNN)
    * [ ] Long Short-Term Memory Neural Networks (LSTM)
    * [ ] Deep Belief Networks (DBN)
    * [ ] Variational Autoencoders (VAE)
    * [ ] Generative Adversarial Networks (GAN)
    * [ ] Diffussion
    * [ ] Transformer-based Neural Networks including Encode and Decode
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
  + [x] Software Maintenance
  + [ ] Other
- 🤖Programming Language (PL)
  + 🪪Characteristics
    * [x] Executable
    * [ ] Dynamic/Statical PL
    * [ ] Procedure/Object/Aspect Orient PL
    * [ ] Other Characteristics
  + 🪵Resource
    * [x] Code Files
    * [x] Test Cases
    * [ ] Repositories
    * [x] Warnings, Errors, Bugs, Debug and Compilable Infos
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
- 🗂️Downstream Benchmark
  + GCC
  + Clang
- 💕Contribution
  + First, the proposed framework is fully automatic. By training a Sequence-to-Sequence model which can be viewed as an implicit representation of the language patterns for the training data, C syntax in our context, our framework DeepFuzz will continuously provide new syntactic correct C programs.
  + Second, we build a practical tool for fuzzing off-the-shelf C compilers. We conduct a detailed analysis of how key factors will affect the accuracy of the generative model and fuzzing performance.
  + Third, we apply our DeepFuzz technique to test GCC and Clang/LLVM. During our preliminary analysis, the testing coverage (line, function, and branch) is increased and we have found and reported 8 real-world bugs.
