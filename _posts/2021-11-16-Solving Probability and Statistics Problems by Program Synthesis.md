---
title: Solving Probability and Statistics Problems by Program Synthesis
author: coder
date: 2021-11-16 00:00:00 +0800
categories: [arxiv]
tags: [methods, benchmarks]
math: true
image:
  path: /assets/imgs/PS-1.png
  width: 800
  height: 500
  alt: Probabilistic Simulation Program Workflow Example.
---

## 🌸Method

- 📙Title: [Solving Probability and Statistics Problems by Program Synthesis](https://arxiv.org/pdf/2111.08267.pdf)
- 📚Publisher/Date: `Arxiv/2021`
- 🏠Author Affiliation: Harvard University; MIT; Columbia University
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
    * [ ] Other Resources
  + 🚀Platform
    * [x] GitHub
    * [ ] Gitee
    * [ ] StackOverFlow
    * [ ] CodeForces
    * [ ] LeetCode
    * [x] Other Platform
- 🗂️Downstream Benchmark
  + MIT's 18.05
  + Harvard's STAT110
- ✈️Relevant Model
  + Codex[^codex]
- 💕Contribution
  + To the best of our knowledge, we are the first to propose such a simulation based approach to solve probability questions.
  + To evaluate the efficacy of our approach, we collect two sets of $20$ undergraduate-level probability and statistics problems, curated from MIT’s 18.05 and Harvard’s STAT110.

## 📙Proposed Benchmark

- Benchmark Name: `MIT's 18.05`; `Harvard's STAT110`
- 📚Publisher/Date: `Arxiv/2021`
- 🏠Author Affiliation: Harvard University; MIT; Columbia University
- 🔗URL: The appendix in [https://arxiv.org/pdf/2111.08267.pdf](https://arxiv.org/pdf/2111.08267.pdf)
- Feature: University-level probability and statistics problems
- Details: 
  + The first dataset consists of applied questions in probability. We take $20$ questions that have numerical answers from MIT’s 18.05: Introduction to Probability and Statistics. Course topics include various probability and statistics concepts, including counting, conditional probability, discrete and continuous random variables, expectation and variance, central limit theorem, joint distributions, maximum likelihood estimators, Bayesian updating, null hypothesis significance testing, and confidence intervals.
  + The second dataset, in contrast to the first dataset, consists of conceptual questions in probability and statistics. We take 20 questions that have numerical answers from Harvard’s STAT110: Probability and Brainstellar online catalogue of quantitative finance probability brainteasers. Topics include: distributions, moment generating functions, expectation, variance, covariance, correlation, conditional probability, joint distributions, marginal distributions, conditional distributions, limit theorems, and Markov chains.
- Supported Metric: `Accuracy`
- Test Case: `Not involved`
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
- 🔑Output (code)
  + 🚩Language: `Python`
  + ⛺Domain
    * [ ] General
    * [ ] Data Analysis and Manipulation
    * [ ] Plotting
    * [ ] Mathematical
    * [ ] Chemical
    * [x] Educational
    * [ ] Other Domains
  + 👑Library
    * [x] Build-in Library
    * [ ] Public Library
    * [ ] Private Library
    * [ ] Other Libraries
  + 🎯Level
  	* [ ] Token Level
    * [ ] Line Level
    * [ ] Span Level
    * [x] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 📘Reference

[^codex]: [https://arxiv.org/pdf/2107.03374.pdf](https://arxiv.org/pdf/2107.03374.pdf)
