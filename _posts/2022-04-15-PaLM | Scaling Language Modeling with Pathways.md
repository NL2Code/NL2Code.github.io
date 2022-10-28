---
title: PaLM | Scaling Language Modeling with Pathways
author: coder
date: 2022-04-15 00:00:00 +0800
categories: [arxiv]
tags: [methods, models, benchmarks]
math: true
pin: false
---

> Note that we only report the `nl2code` related parts.
{: .prompt-tip }

## 🌸Method

- 📙Title: [PaLM Scaling Language Modeling with Pathways](https://arxiv.org/pdf/2204.02311.pdf)
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: `Google Research`
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
    * [ ] Bugs and Debug Infos
    * [ ] API Document
    * [ ] Official Tutorial
    * [ ] Abstract Syntax Tree (AST)
    * [ ] Data/Control Flow (DF/CF)
    * [ ] Variable 
    * [ ] PL keywords
    * [ ] Code Comment
    * [x] Other Resources
  + 🚀Platform
    * [x] GitHub
    * [ ] Gitee
    * [ ] StackOverFlow
    * [ ] CodeForces
    * [ ] LeetCode
    * [x] Other Platform
- 🗂️Downstream Benchmark
  + HumanEval[^humaneval]
  + MBPP[^mbpp]
  + GSM8K-Python
- ✈️Relevant Model
  + LaMDA[^lamda]
  + Codex[^codex]
  + PaLM[^palm]
- 💕Contribution
  + To further our understanding of the impact of scale on few-shot learning, we trained a 540-billion parameter, densely activated, Transformer language model, which we call Pathways Language Model (PaLM).
  + On a number of these tasks, PaLM (-Coder) achieves breakthrough performance, outperforming the finetuned stateof-the-art on a suite of multi-step reasoning tasks, and outperforming average human performance on the recently released BIG-bench benchmark. 

## 🎃Proposed Model

- Model Name: `PaLM-Coder`
- Publisher/Date: `Arxiv/2022`
- Author Affiliation: `Google Research`
- Architecture: `Transformer-based neural networks (decoder)`
- Pre-Traing Corpus: We finetune the  PaLM model[^palm] in two stages: (a) first finetuning for 6.5B tokens on a mixture of 60% Python code from ExtraPythonData, 30% code across languages (from the same source as the pre-training code data, but which was not included in pretraining), and 10% natural language, and (b) finetuning for an additional 1.9B tokens on more Python code from ExtraPythonData. 
- Supported Natural Language: `multilingual`
- Supported Programming Language: `Java`; `HTML`; `JavaScript`; `Python`; `C`; `PHP`; `C#`; `C++`
- Model Size: `8B`; `62B`; `540B`
- Public Item: `None`
- 🔗URL: `None`

## 📚Proposed Benchmark

- Benchmark Name: `GSM8K-Python`
- Publisher/Date: `Arxiv/2022`
- Author Affiliation: `Google Research`
- 🔗URL: `None`
- Sub-benchmark
  * GSM8K[^gsm8k]
- Feature: Mathematics word problem
- Details: We also introduce the GSM8K-Python task, which is derived from the GSM8K dataset[^gsm8k]. GSM8K consists of 8.5K high quality grade school math problems created by human problem writers.
- Supported Metric: `pass@k`
- Test Case： ✅
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
    * [x] Build-in Library
    * [ ] Public Library
    * [ ] Private Library
  + 🎯Level
  	* [ ] Token Level
    * [ ] Line Level
    * [x] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 📘Reference

[^palm]: [https://arxiv.org/pdf/2204.02311.pdf](https://arxiv.org/pdf/2204.02311.pdf)
[^humaneval]: [https://github.com/openai/human-eval](https://github.com/openai/human-eval)
[^mbpp]: [https://huggingface.co/datasets/Muennighoff/mbpp](https://huggingface.co/datasets/Muennighoff/mbpp)
[^gsm8k]: [https://github.com/openai/grade-school-math](https://github.com/openai/grade-school-math)
[^lamda]: [https://arxiv.org/pdf/2201.08239.pdf](https://arxiv.org/pdf/2201.08239.pdf)
[^codex]: [https://arxiv.org/pdf/2107.03374.pdf](https://arxiv.org/pdf/2107.03374.pdf)
