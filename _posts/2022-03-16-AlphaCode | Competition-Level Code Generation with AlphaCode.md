---
title: Competition-Level Code Generation with AlphaCode
author: coder
date: 2022-03-16 00:00:00 +0800
categories: [arxiv]
tags: [methods, models, benchmarks, metrics]
math: true
pin: false
---

## 🌸Method

- 📙Title: [Competition-Level Code Generation with AlphaCode](https://arxiv.org/pdf/2203.07814.pdf)
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: `DeepMind`
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
    * [x] Test Cases
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
    * [x] CodeForces
    * [ ] LeetCode
    * [ ] Other Platform
- 🗂️Downstream Benchmark
  + Online Codeforces platform[^codeforce]
  + CodeContests[^codecontests]
  + APPs[^apps]
  + HumanEval[^humaneval]
- ✈️Base Model
  + GPT-Neo[^gpeneo]
  + [Codex](https://nl2code.github.io/posts/Evaluating-Large-Language-Models-Trained-on-Code/)
  + AlphaCode
- 💕Contribution
  + In this paper we present AlphaCode, a code generation system applied to solving competitive programming problems.
  + We release a new training and evaluation competitive programming dataset, named CodeContests.

## 🎃Proposed Model

- Model Name: `AlphaCode`
- Publisher/Date: `Arxiv/2022`
- Author Affiliation: `DeepMind`
- Architecture: `Transformer-based neural networks (encoder-decoder)`
- Traing Corpus: Pre-training on `A lot of code files`; Fine-tuning on CodeContests[^codecontests].
- Supported Natural Language: `English`
- Supported Programming Language: `C++`; `C#`; `Go`; `Java`; `JavaScript`; `Lua`; `PHP`; `Python`; `Ruby`; `Rust`; `Scala`; `TypeScript`
- Model Size: `300M`; `1B`; `3B`; `9B`; `41B`
- Public Item: `None`
- 🔗URL: [https://alphacode.deepmind.com](https://alphacode.deepmind.com)

## 📚Proposed Benchmark

- Benchmark Name: `CodeContests`
- Publisher/Date: `Arxiv/2022`
- Author Affiliation: `DeepMind`
- 🔗URL: [https://github.com/deepmind/code_contests](https://github.com/deepmind/code_contests)
- Supported Metric: `pass@k`; `10@k`
- 🔏Input (NL)
  + 🚩Language: `English`
  + 🌟Format
    * [ ] Code Context
    * [ ] Plain Natural Language
    * [x] Competition Problem
    * [ ] Code Comment
    * [ ] TODO
    * [ ] Other Formats
  + 💈Description Granularity
    * [x] Why? (Background)
    * [x] What? (Requirement, TODO)
    * [ ] How? (Algorithm Process)
    * [ ] Other Granularities
- 🔑Output (code)
  + 🚩Language: `C++`; `C#`; `Go`; `Java`; `JavaScript`; `Lua`; `PHP`; `Python`; `Ruby`; `Rust`; `Scala`; `TypeScript`
  + ⛺Domain
    * [x] General
    * [ ] Data Analysis and Manipulation
    * [ ] Plotting
    * [ ] Mathematical
    * [ ] Chemical
    * [ ] Educational
    * [ ] Other Domains
  + 👑Library
    * [x] Public Library
    * [ ] Private Library
  + 🎯Level
  	* [ ] Token Level
    * [ ] Line Level
    * [x] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 🚩Proposed Metric

- Metric Name: `10@k`
- Definition: The percentage of problems solved when we take $k$ samples from the model for each problem but can only submit $10$ of them for evaluation on the hidden tests. This measures factors including the filtering process and how models behave at a very large number of samples.

## 📘Reference

[^codeforce]: [https://codeforces.com](https://codeforces.com)
[^codecontests]: [https://github.com/deepmind/code_contests](https://github.com/deepmind/code_contests)
[^apps]: [https://github.com/hendrycks/apps](https://github.com/hendrycks/apps)
[^humaneval]: [https://github.com/openai/human-eval](https://github.com/openai/human-eval)
[^gpeneo]: https://huggingface.co/docs/transformers/model_doc/gpt_neo

