---
title: CoCoMIC | Code Completion By Jointly Modeling In-file and Cross-file Context
author: coder
date: 2022-12-20 00:00:00 +0800
categories: [arxiv]
tags: [methods, benchmarks]
math: true
---

## 🌸Method

- 📙Title: [CoCoMIC Code Completion By Jointly Modeling In-file and Cross-file Context](https://arxiv.org/pdf/2212.10007.pdf)
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: `Columbia University`; `AWS AI Labs`
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
    * [x] Zero-shot Learning
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
    * [ ] Programmatic Idioms
    * [ ] Code Sketches
    * [ ] Other Resources
  + 🚀Platform&Tool
    * [ ] GitHub
    * [ ] Gitee
    * [ ] StackOverFlow
    * [ ] CodeForces
    * [ ] LeetCode
    * [ ] Google Code
    * [ ] Modulo Static Analysis Tool
    * [x] PyPI
    * [ ] Other Platform
- 🗂️Downstream Benchmark
  + This paper's dataset
- ✈️Relevant Model
  + CodeGen
- 💕Contribution
  + We build CCFinder, a tool that is effective at collecting cross-file context, a critical yet overlooked resource for code completion in modern software development.
  + We propose CoCoMIC, a framework on top of existing code LMs that jointly learns in-file and cross-file context for code completion.
  + We show that CoCoMIC with cross-file context from CCFINDER significantly outperforms baselines by up to 19.30% improvement in exact match.

## 📙Proposed Benchmark 

- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: `Columbia University`; `AWS AI Labs`
- 🔗URL: Not yet released
- Feature: Project level code generation
- Details: We use Python Package Index (PyPI) data for experiments. PyPI is a repository of open-source Python projects, and each project builds a reusable package. We collect permissivelylicensed packages and filter out those with too few files (≤ 5 files containing python code) or too memory-consuming to build the project-context graph (more than 5k nodes), ending up with 60,891 packages. Then, we divide the dataset into 80%/10%/10% train, validation, and test split with different sets of packages.
- Supported Metric: `EM`; `BLEU-4`; `Precision`; `Recall`
- Test Case: `Not involved`
- 🔏Input (NL)
  + 🚩Language: `English`
  + 🌟Format
    * [ ] Plain Natural Language
    * [ ] Competition Problem
    * [x] Code Comment
    * [ ] TODO
    * [ ] Pseudocode
    * [ ] Other Formats
  + 💈Description Granularity
    * [ ] Why? (Background)
    * [x] What? (Requirement, Functionality, TODO)
    * [ ] How? (Algorithm Process)
    * [ ] Other Granularities
  + 🎯Additional Input
    * [ ] None
    * [x] Code Context
    * [x] Class Information
    * [x] File Information
    * [x] Repository Information
    * [ ] Other Information
- 🔑Output (code)
  + 🚩Language: `Python`
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
    * [x] Other Libraries
  + 🎯Level
  	* [ ] Token Level
    * [x] Line Level
    * [ ] Span Level
    * [ ] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels
