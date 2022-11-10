---
title: Program Synthesis from Natural Language Using Recurrent Neural Networks
author: coder
date: 2017-03-01 00:00:00 +0800
categories: [other]
tags: [methods, benchmarks, metrics]
math: true
image:
  path: /assets/imgs/tellina.png
  width: 800
  height: 500
  alt: Tellina's three-step architecture for program synthesis from natural language.
---

## 🌸Method

- 📙Title: [Program Synthesis from Natural Language Using Recurrent Neural Networks](https://dericpang.com/static/e511b5f8f6060087dc29dae9fed86200/tellina-tr170510.pdf)
- 📚Publisher/Date: `Other/2017`
- 🏠Author Affiliation: UW CSE
- 🔗URL: `None`
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
    * [ ] Abstract Syntax Tree (AST)
    * [ ] Data/Control Flow (DF/CF)
    * [ ] Variable 
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
  + We propose a novel deep-learning approach for synthesizing programs from natural language. Our approach combines stateof-the-art recurrent neural networks with a learning approach for inserting constants into the generated programs.
  + We instantiated the approach for a challenging domain: bash commands containing 17 file system utilities, more than 200 flags, 9 types of open-vocabulary constants, and nested command structures such as pipelines, command substitution, and process substitution.
  + In order to provide data for training and evaluation, we collected over 5,000 <NL, command> pairs.
  + We evaluated the accuracy of our approach. Our model achieves top-3 accuracy of 80.0% for determining program structure — that is, ignoring constant values. Our model achieves top-3 accuracy of 36.0% for full commands.
  + We conducted a controlled user study to determine whether a good, but not perfectly accurate, model aids end users’ programming efficiency. Compared to existing programming resources such as man pages, Stack Overflow, and Google, Tellina shortened the working time by 21.7% for end-user programmers on bash file system tasks. This improvement was statistically significant (p-value < 0.01).

## 📙Proposed Benchmark

- Benchmark Name: `Unnamed`
- 📚Publisher/Date: `Other/2017`
- 🏠Author Affiliation: UW CSE
- 🔗URL: `None`
- Details: our dataset contains 5,413 <NL, bash> pairs. these commands contain 17 different bash utilities and more than 200 tags. In descending order of frequency, the utilities are `find`, `xargs`, `grep`, `egrep`, `fgrep`, `ls`, `rm`, `cp`, `mv`, `wc`, `chmod`, `chown`, `chgrp`, `sort`, `head`, `tail`, `tar`.

![Window shadow](/assets/imgs/cmdnl.png){: .shadow width="700" height="300" .w-75 }
_Data statistics._

- Supported Metric: $Acc^k_F$; $Acc^k_T$
- Test Case: ❌
- 🔏Input (NL)
  + 🚩Language: `English`
  + 🌟Format
    * [ ] Code Context
    * [x] Plain Natural Language
    * [ ] Competition Problem
    * [ ] Code Comment
    * [ ] TODO
    * [ ] Pseudocode
    * [ ] Other Formats
  + 💈Description Granularity
    * [ ] Why? (Background)
    * [x] What? (Requirement, Functionality, TODO)
    * [ ] How? (Algorithm Process)
    * [ ] Other Granularities
  + 🎯Additional Input
    * [x] None
    * [ ] Class Information
    * [ ] File Information
    * [ ] Repository Information
    * [ ] Other Information
- 🔑Output (code)
  + 🚩Language: `Bash`
  + ⛺Domain
    * [x] General
    * [ ] Data Analysis and Manipulation
    * [ ] Plotting
    * [ ] Mathematical
    * [ ] Chemical
    * [ ] Educational
    * [ ] Other Domains
  + 👑Library
    * [x] Build-in Library
    * [ ] Public Library
    * [ ] Private Library
    * [ ] Other Libraries
  + 🎯Level
  	* [ ] Token Level
    * [x] Line Level
    * [ ] Span Level
    * [ ] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 🚩Proposed Metric#1

- Metric Name: $Acc^{k}_{F}$
- Definition: We define it to be the percentage of test examples for which a correct full command is ranked $k$ or above in the model output.

## 🚩Proposed Metric#2

- Metric Name: $Acc^{k}_{T}$
- Definition: We define it to be the percentage of test examples for which a correct command template is ranked $k$ or above in the model output (i.e. ignoring errors in the constants).
