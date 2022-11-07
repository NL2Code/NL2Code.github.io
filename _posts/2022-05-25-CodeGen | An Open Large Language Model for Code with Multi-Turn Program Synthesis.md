---
title: CodeGen | An Open Large Language Model for Code with Multi-Turn Program Synthesis
author: coder
date: 2022-05-25 00:00:00 +0800
categories: [arxiv]
tags: [methods, models, benchmarks]
math: true
pin: false
---

## 🌸Method

- 📙Title: [CodeGen An Open Large Language Model for Code with Multi-Turn Program Synthesis](https://arxiv.org/pdf/2203.13474.pdf)
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: `Salesforce Research`
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
    * [ ] Repositories
    * [ ] Bugs and Debug Infos
    * [ ] API Document
    * [ ] Official Tutorial
    * [ ] Abstract Syntax Tree (AST)
    * [ ] Data/Control Flow (DF/CF)
    * [ ] Variable 
    * [ ] PL keywords
    * [ ] Code Comment
    * [ ] Other Resources
  + 🚀Platform
    * [x] GitHub
    * [ ] Gitee
    * [ ] StackOverFlow
    * [ ] CodeForces
    * [ ] LeetCode
    * [ ] Other Platform
- 🗂️Downstream Benchmark
  + HumanEval[^humaneval]
  + MTPB[^mtpb]
- ✈️Base Model
  + GPT-Neo
  + Codex
  + CodeGen
- 💕Contribution
  + We study multi-turn program synthesis emerging in autoregressive models under scaling laws.
  + We leverage this capacity to introduce a multi-turn program synthesis paradigm.
  + We investigate its properties quantitatively with a novel multi-turn programming benchmark.
  + We open source the model checkpoints and the custom training library: JAXFORMER.

## 🎃Proposed Model

- Model Name: `CodeGen`
- Publisher/Date: `Arxiv/2022`
- Author Affiliation: `Salesforce Research`
- Architecture: `Transformer-based neural networks (decoder)`
- Traing Corpus: `A lot of code files`
- Supported Natural Language: `English`
- Supported Programming Language: `C`; `C++`; `Go`; `Java`; `JavaScript`; `Python`
- Model Size: `350M`; `2.7B`; `6.1B`; `16.1B`
- Public Item: `checkpoint`; `training code`; `inference code`
- 🔗URL: [https://github.com/salesforce/CodeGen](https://github.com/salesforce/CodeGen)

## 📚Proposed Benchmark

- Benchmark Name: `MTPB`
- Publisher/Date: `Arxiv/2022`
- Author Affiliation: `Salesforce Research`
- 🔗URL: [https://github.com/salesforce/CodeGen/tree/main/benchmark](https://github.com/salesforce/CodeGen/tree/main/benchmark)
- Supported Metric: `pass@k`
- Feature: Multi-turn Evaluation
- Details: we construct an open benchmark, Multi-Turn Programming Benchmark (MTPB), consisting of `115` diverse problem sets that are factorized into multi-turn prompts.
- Test Case： ✅
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
    * [x] What? (Requirement, TODO)
    * [ ] How? (Algorithm Process)
    * [ ] Other Granularities
  + 🎯Additional Input
    * [x] None
    * [ ] Class Information
    * [ ] File Information
    * [ ] Repository Information
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
    * [x] Public Library
    * [ ] Private Library
    * [ ] Other Libraries
  + 🎯Level
  	* [ ] Token Level
    * [x] Line Level
    * [x] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 📘Reference

[^humaneval]: [https://github.com/openai/human-eval](https://github.com/openai/human-eval)
[^mtpb]: [https://github.com/salesforce/CodeGen/tree/main/benchmark](https://github.com/salesforce/CodeGen/tree/main/benchmark)
