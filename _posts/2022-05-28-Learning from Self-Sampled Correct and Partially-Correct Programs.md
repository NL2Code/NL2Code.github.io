---
title: Learning from Self-Sampled Correct and Partially-Correct Programs
author: coder
date: 2022-05-28 00:00:00 +0800
categories: [arxiv]
tags: [methods]
math: true
image:
  path: /assets/imgs/selfsampled.png
  width: 500
  height: 800
  alt: Examples of self-sampled correct and partially correct programs from MathQA. The program statements and states marked in red are incorrect.
---

## 🌸Method

- 📙Title: [Learning from Self-Sampled Correct and Partially-Correct Programs](https://arxiv.org/pdf/2205.14318.pdf)
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: Yale University; Microsoft Research; X, the moonshot factory; University of Washington
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
    * [ ] Google Code
    * [ ] Other Platform
- 🗂️Downstream Benchmark
  + MathQA-Python[^mathqa]
  + MathQA-Python-Filtered[^mathqa]
  + GSM5.5K-Python[^gsm]
- ✈️Relevant Model
  + GPT-Neo
  + Codex
  + LaMDA
  + PaLM
- 💕Contribution
  + We propose to let the model perform sampling during training and learn from both self-sampled fullycorrect programs, which yield the gold execution results, as well as partially-correct programs, whose intermediate execution state matches another correct program. 
  + We show that our use of self-sampled correct and partially-correct programs can benefit learning and help guide the sampling process, leading to more efficient exploration of the program space.
  + Additionally, we explore various training objectives to support learning from multiple programs per example and find they greatly affects the performance. Experiments on the MathQA and GSM8K datasets show that our proposed method improves the `pass@k` performance by 3.1% to 12.3% compared to learning from a single reference program with MLE.

## 📘Reference

[^gsm]: [https://github.com/openai/grade-school-math](https://github.com/openai/grade-school-math)
[^mathqa]: [https://github.com/google/trax/blob/master/trax/examples/MathQA_Python_generation_notebook.ipynb](https://github.com/google/trax/blob/master/trax/examples/MathQA_Python_generation_notebook.ipynb)
