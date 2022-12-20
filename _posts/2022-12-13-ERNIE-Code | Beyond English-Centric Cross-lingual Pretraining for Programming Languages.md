---
title: ERNIE-Code | Beyond English-Centric Cross-lingual Pretraining for Programming Languages
author: coder
date: 2022-12-13 00:00:00 +0800
categories: [arxiv]
tags: [methods, models]
math: true
---

> Note that we only report the `nl2code` related parts.
{: .prompt-tip }

## 🌸Method

- 📙Title: [ERNIE-Code Beyond English-Centric Cross-lingual Pretraining for Programming Languages](https://arxiv.org/pdf/2212.06742)
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: `Baidu`
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
    * [x] Unsupervised Transfer Learning
    * [ ] Self-Supervised Transfer Learning
    * [ ] Semi-Supervised Transfer Learning
    * [ ] Weak Supervised Transfer Learning
    * [ ] Reinforcement Learning (RL)
    * [x] Multi-task Learning
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
  + [x] Software Development
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
    * [x] Other Platform
- 🗂️Downstream Benchmark
  + CoNaLa
  + mCoNaLa
- ✈️Relevant Model
  + mBART
  + mT5
  + PLBART
  + CodeT5
- 💕Contribution
  + (1) We first propose a unified cross-lingual pre-trained LLM for both multilingual NLs and multilingual PLs, enlarging the capacity of LLMs towards jointly learning the universal multilingualism. 
  + (2) We adopt the pivotbased translation language modeling with prompting to build connections between multi-NLs and multi-PLs (with English pivots) and mitigate the problem when the parallel corpus of multilingualNL↔multilingual-PL is unavailable. 
  + (3) We obtain superior performance compared with previous multilingual LLMs across a wide range of code intelligence tasks, including text-to-code, code-to-text, code repair, and code documentation translation.
  + (4) To some extent, our model has shown zeroshot prompting ability on multilingual code-to-text, text-to-code, and text-to-text generation. Moreover, ERNIE-Code is well-performed at naming a function and completing corresponding arguments given multilingual NL instructions. 
  + (5) We release a Chinese-Python parallel test set to accelerate the research of this field.

## 🎃Proposed Model

- Model Name: `ERNIE-Code`
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: `Baidu`
- Architecture: `Transformer-based neural networks (encoder-decoder)`
- Pre-Training Corpus:  PL-NL query pairs on CodeSearchNet; CC10[^cc10];  OPUS[^opus]
- Supported Natural Language: Multiligual
- Supported Programming Language: Multiligual
- Model Size: `560M`
- Public Item: The authors will make the code and pre-trained models publicly available.
- 🔗URL: `None`

## 📘Reference

[^cc10]: [Unsupervised Cross-lingual Representation Learning at Scale](https://aclanthology.org/2020.acl-main.747)
[^opus]: [https://opus.nlpl.eu](https://opus.nlpl.eu)
