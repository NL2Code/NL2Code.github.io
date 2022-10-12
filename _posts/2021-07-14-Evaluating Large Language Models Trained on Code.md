---
title: Evaluating Large Language Models Trained on Code
author: coder
date: 2021-07-14 00:00:00 +0800
categories: [arxiv]
tags: [methods, models, benchmarks, metrics]
pin: false
---

## 🌸Method

- 📙Title: [Evaluating Large Language Models Trained on Code](https://arxiv.org/pdf/2107.03374.pdf)
- 📚Publisher/Date: `Arxiv/2021`
- 🏠Author Affiliation: `OpenAI`
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
  + HumanEval
  + APPs
- ✈️Base Model
  + GPT-Neo
  + GPT-J
  + TabNine
  + Codex
- 💕Contribution
  + They introduce Codex, a GPT language model fine-tuned on publicly available code from GitHub, and study its Python code-writing capabilities.
  + They release HumanEval, a new evaluation set to measure functional correctness for synthesizing programs from docstrings.

## 🎃Proposed Model

- 🖊️Model Name: `Codex`
- 📚Publisher/Date: `Arxiv/2021`
- 🏠Author Affiliation: `OpenAI`
- ⚒️Architecture: `Transformer-based neural networks (decoder)`
- 📀Traing Corpus: `A lot of code files`
- 🔥Supported Natural Language: `English`
- 💧Supported Programming Language: `Python`
- 🧚Model Size: `12M`; `25M`; `42M`; `85M`; `300M`; `679M`; `2.5B`; `12B`; `175B`
- 📢Public Item: `None`
- 🔗URL: `None`

## 📚Proposed Benchmark

- 🖊️Benchmark Name: `HumanEval`
- 📚Publisher/Date: `Arxiv/2021`
- 🏠Author Affiliation: `OpenAI`
- 🚩Supported Metric: `pass@k`
- 🔏Input (NL)
  + 🚩Language: `English`
  + 🌟Format
    * [x] Code Context
    * [ ] Plain Natural Language
    * [ ] Competition Problem
    * [ ] Code Comment
    * [ ] TODO
    * [ ] Other Formats
  + 💈Description Granularity
    * [ ] Why? (Background)
    * [x] What? (Requirement, TODO)
    * [ ] How? (Algorithm Process)
    * [ ] Other Granularities
- 🔑Output (code)
  + 🚩Language: `Python`
  + ⛺Domain
    * [x] General
    * [ ] Mathematical
    * [ ] Chemical
    * [ ] Educational
    * [ ] Other Domains
  + 👑Library
    * [ ] Public Library
    * [ ] Private Library
  + 🎯Level
    * [ ] Line Level
    * [x] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels
- 🔗URL: `https://github.com/openai/human-eval`

## 🚩Proposed Metric
