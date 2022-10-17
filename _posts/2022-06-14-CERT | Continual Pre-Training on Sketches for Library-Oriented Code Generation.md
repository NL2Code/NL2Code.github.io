---
title: CERT | Continual Pre-Training on Sketches for Library-Oriented Code Generation
author: coder
date: 2022-06-14 00:00:00 +0800
categories: [IJCAI]
tags: [methods, models, benchmarks]
math: true
pin: false
---

## 🌸Method

- 📙Title: [CERT Continual Pre-Training on Sketches for Library-Oriented Code Generation](https://arxiv.org/pdf/2206.06888.pdf)
- 📚Publisher/Date: `IJCAI/2022`
- 🏠Author Affiliation: `Chinese Academy of Sciences`; `University of Chinese Academy of Sciences`; `Microsoft Research Asia`; `Korea University`; `Microsoft Azure AI`
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
  + HumanEval[^humaneval]
  + PandasEval[^pandas-numpy-eval]
  + NumpyEval[^pandas-numpy-eval]
- ✈️Base Model
  + PyCodeGPT[^pycodegpt]
  + CodeGen[^codegen]
- 💕Contribution
  + We propose CERT (for sketCher and gEneRaTor), a continual pre-training approach on sketches for library-oriented code generation. In CERT, a sketcher firstly focuses on predicting a sketch, which omits user-defined details; then, a generator uses the sketch as a prompt to generate the complete code. Both the sketcher and the generator are continually pre-trained based on a base language model for code, using unlabelled code corpora rather than pairwise labelled data. 
  + In addition, we craft two evaluation benchmarks for Python libraries, called PandasEval and NumpyEval, each including 101 programming problems using Pandas and NumPy, respectively. 
  + We perform extensive experiments on CERT. Results indicate that CERT has superior performance on library-oriented code generation. We further draw several insights via thorough analysis.

## 🎃Proposed Model

- Model Name: `PyCodeGPT`
- Publisher/Date: `IJCAI/2022`
- Author Affiliation: `OpenAI`
- Architecture: `Transformer-based neural networks (decoder)`
- Traing Corpus: `A lot of code files`
- Supported Natural Language: `English`
- Supported Programming Language: `Python`
- Model Size: `112M`
- Public Item: `checkpoint`; `training code`; `inference code`
- 🔗URL: [https://github.com/microsoft/PyCodeGPT](https://github.com/microsoft/PyCodeGPT)

## 📚Proposed Benchmark

- Benchmark Name: `PandasEval&NumpyEval`
- Publisher/Date: `IJCAI/2021`
- Author Affiliation: `Chinese Academy of Sciences`; `University of Chinese Academy of Sciences`; `Microsoft Research Asia`; `Korea University`; `Microsoft Azure AI`
- 🔗URL: [https://github.com/microsoft/PyCodeGPT/tree/main/cert/pandas-numpy-eval](https://github.com/microsoft/PyCodeGPT/tree/main/cert/pandas-numpy-eval)
- Supported Metric: `pass@k`
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
    * [ ] General
    * [x] Data Analysis and Manipulation
    * [ ] Mathematical
    * [ ] Chemical
    * [ ] Educational
    * [ ] Other Domains
  + 👑Library
    * [x] Public Library
    * [ ] Private Library
  + 🎯Level
  	* [ ] Token Level
    * [x] Line Level
    * [x] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 📘Reference

[^humaneval]: https://github.com/openai/human-eval
[^pandas-numpy-eval]: https://github.com/microsoft/PyCodeGPT/tree/main/cert/pandas-numpy-eval
[^pycodegpt]: https://github.com/microsoft/PyCodeGPT
[^codegen]: https://github.com/salesforce/CodeGen
