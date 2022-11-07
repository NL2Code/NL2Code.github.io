---
title: Repository-Level Prompt Generation for Large Language Models of Code
author: coder
date: 2022-06-26 00:00:00 +0800
categories: [arxiv]
tags: [methods, benchmarks, metrics]
math: true
image:
  path: /assets/imgs/repo.png
  width: 800
  height: 500
  alt: Repository-Level prompt generator.
---

## 🌸Method

- 📙Title: [Repository-Level Prompt Generation for Large Language Models of Code](https://arxiv.org/pdf/2206.12839.pdf)
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: Google Research
- 🔗URL: [https://github.com/shrivastavadisha/repo_level_prompt_generation](https://github.com/shrivastavadisha/repo_level_prompt_generation)
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
    * [x] Repositories
    * [ ] Warnings, Errors, Bugs and Debug Infos
    * [ ] API Document
    * [ ] Official Tutorial
    * [x] Abstract Syntax Tree (AST)
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
    * [x] Google Code
    * [ ] Other Platform
- 🗂️Downstream Benchmark
  + RLPG's dataset[^rlpg]
- ✈️Relevant Model
  + Codex[^codex]
- 💕Contribution
  + We propose a framework called the Repo-Level Prompt Generator (`RLPG`) that learns to generate prompts conditioned on the example, without requiring access to the weights of the LLM.
  + To incorporate domain-knowledge in the prompt design process, RLPG uses a set of repository level prompt proposals. These prompt proposals are designed to incorporate both the structure of the repository as well as the relevant context from all files in the repository.
  + On the task of single-line code-autocompletion, we show that an oracle constructed from our proposed prompt proposals gives up to `36%` relative improvement over Codex. This improvement is pleasantly surprising as Codex has never seen prompts made from these prompt proposals during training. Further, we show that when we use our prompt proposal classifier to predict the best prompt proposal, we can achieve up to `17%` relative improvement over Codex.

## 📙Proposed Benchmark

- Benchmark Name: `RLPG's dataset`
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: Google Research
- 🔗URL: [https://github.com/shrivastavadisha/repo_level_prompt_generation](https://github.com/shrivastavadisha/repo_level_prompt_generation)
- Feature: Repository-level code generation
- Details: We selected the repositories that had a permissive license giving us a total of `47` repositories. We divided the repositories into train, validation and test splits, where each repository in its entirety is part of a split. In each file within a repository, we remove lines that are blank and comments, and set the hole position to be the middle character in the line. All the characters from the middle position to the end of the line constitute the target hole.
- Supported Metric: `success rate (SR)`
- Test Case: ❌
- 🔏Input (NL)
  + 🚩Language: `English`
  + 🌟Format
    * [x] Code Context
    * [ ] Plain Natural Language
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
    * [ ] None
    * [ ] Class Information
    * [ ] File Information
    * [x] Repository Information
    * [ ] Other Information
- 🔑Output (code)
  + 🚩Language: `Java`
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

## 🚩Proposed Metric

- Metric Name: `success rate (SR)`
- Definition:  In our experiments, we report the percentage of successful holes divided by the total number of holes for each split. We will call this success rate (SR) going forward.

## 📘Reference

[^codex]: [https://arxiv.org/pdf/2107.03374.pdf](https://arxiv.org/pdf/2107.03374.pdf)
[^rlpg]: [https://github.com/shrivastavadisha/repo_level_prompt_generation](https://github.com/shrivastavadisha/repo_level_prompt_generation)
