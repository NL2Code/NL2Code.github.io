---
title: Yes, You Can Make an App Too | A Systematic Study of Prompt Engineering in the Automatic Generation of Mobile Applications from User Queries
author: coder
date: 2021-07-14 00:00:00 +0800
categories: [other]
tags: [methods, benchmarks]
math: true
image:
  path: /assets/imgs/make_app.png
  width: 800
  height: 500
  alt: Prompt engineering pipeline.
---

## 🌸Method

- 📙Title: [Yes, You Can Make an App Too A Systematic Study of Prompt Engineering in the Automatic Generation of Mobile Applications from User Queries](https://appinventor.mit.edu/assets/files/Shone_Jasmine_Rachel_RSIFinal.pdf)
- 📚Publisher/Date: `Other/2022`
- 🏠Author Affiliation: MIT
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
    * [ ] Supervised Transfer Learning
    * [ ] Weak Supervised Transfer Learning
    * [x] Unsupervised Transfer Learning
    * [ ] Reinforcement Learning (RL)
    * [ ] Multi-task Learning
    * [ ] Meta Learning
    * [ ] Contrastive Learning
    * [ ] Retrieved-based Learning
    * [ ] Other
  + 🧬Paradigm
    * [ ] Non-pre-train
    * [ ] Pre-train and Fine-tune
    * [ ] Zero-shot Learning
    * [ ] One/two/few-shot Learning
    * [x] In-context Learning
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
    * [ ] Warnings, Errors, Bugs and Debug Infos
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
  + This paper's dataset
- ✈️Relevant Model
  + Codex
- 💕Contribution
  + In order to improve Aptly's ability to generate full, workable apps from a user query, we examine techniques to optimize the generation of prompts on-the-fly from a user description typed into the Aptly platform and sent to Codex to obtain a code output.
  + Specifically, we focus on three characteristics of the prompt: 1. Does the quality of code generation differ based on how examples are chosen? 2. Does increasing the number of tokens (units of semantic meaning in the prompt) sent to Codex improve the quality of code generation? 3. Can we improve the quality of code generation by ordering the examples differently?

## 📙Proposed Benchmark

- Benchmark Name: `This paper's benchmark`
- 📚Publisher/Date: `Other/2022`
- 🏠Author Affiliation: MIT
- 🔗URL: `None`
- Details: A database of `85` unique app examples was compiled by the App Inventor team from apps created on the App Inventor platform. The app examples were selected to cover a wide range of the functionality within the App Inventor platform. These apps were converted from a block-coding-based expression to an intermediate language named Aptly-Script whose functions and classes have a one-to-one correspondence with App Inventor components (for example, having a Text-to-Speech component with the same callable methods). A basic description was also created for each app.
- Supported Metric: `BLEU`; `Manual Evaluation`
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
    * [x] Why? (Background)
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
  + 🚩Language: `Aptly-Script` that is an APP programming language
  + ⛺Domain
    * [x] General
    * [ ] Data Analysis and Manipulation
    * [ ] Plotting
    * [ ] Mathematical
    * [ ] Chemical
    * [ ] Educational
    * [ ] Other Domains
  + 👑Library
    * [ ] Build-in Library
    * [ ] Public Library
    * [ ] Private Library
    * [ ] Other Libraries
  + 🎯Level
  	* [ ] Token Level
    * [ ] Line Level
    * [ ] Span Level
    * [ ] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [x] Other Levels
