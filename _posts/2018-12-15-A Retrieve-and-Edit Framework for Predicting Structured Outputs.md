---
title: A Retrieve-and-Edit Framework for Predicting Structured Outputs
author: coder
date: 2018-12-15 00:00:00 +0800
categories: [NeurIPS]
tags: [methods, benchmarks]
math: true
image:
  path: /assets/imgs/Retrieve-Edit.png
  width: 800
  height: 500
  alt: The retrieve-and-edit approach consists of the retriever, which identifies a relevant example from the training set, and the editor, which predicts the output conditioned on the retrieved example.
---

## 🌸Method

- 📙Title: [A Retrieve-and-Edit Framework for Predicting Structured Outputs](https://proceedings.neurips.cc/paper/2018/file/cd17d3ce3b64f227987cd92cd701cc58-Paper.pdf)
- 📚Publisher/Date: `NeurIPS/2018`
- 🏠Author Affiliation: Stanford University
- 🔗URL: [https://worksheets.codalab.org/worksheets/0x1ad3f387005c492ea913cf0f20c9bb89](https://worksheets.codalab.org/worksheets/0x1ad3f387005c492ea913cf0f20c9bb89)
- 🌐Neural Network (NN)
  + ⚒️Architecture
    * [ ] Feedforward NN (FNN)
    * [ ] Convolutional NN (CNN)
    * [x] Recurrent NN (RNN)
    * [x] Long Short-Term Memory Neural Networks (LSTM)
    * [ ] Deep Belief Networks (DBN)
    * [ ] Variational Autoencoders (VAE)
    * [ ] Generative Adversarial Networks (GAN)
    * [ ] Diffussion
    * [ ] Transformer-based Neural Networks including Encode and Decode
    * [ ] Other
  + ⚙️How to learn
    * [x] Supervised Transfer Learning
    * [ ] Unsupervised Transfer Learning
    * [ ] Self-Supervised Transfer Learning
    * [ ] Semi-Supervised Transfer Learning
    * [ ] Weak Supervised Transfer Learning
    * [ ] Reinforcement Learning (RL)
    * [ ] Multi-task Learning
    * [ ] Meta Learning
    * [ ] Contrastive Learning
    * [x] Retrieved-based Learning
    * [ ] Other
  + 🧬Paradigm
    * [x] Non-pre-train
    * [ ] Pre-train and Fine-tune
    * [ ] Zero-shot Learning
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
  + Retrieve-and-edit's dataset (see below)
  + Hearthstone card[^mtg-hs]
- 💕Contribution
  + Our contribution is a computationally efficient method for learning a retrieval model that embeds the input in a task-dependent way without relying on a hand-crafted metric or incurring the expense of jointly training the retriever with the editor. Our retrieve-and-edit framework can be applied on top of any base model.
  + We show that on a new autocomplete task for GitHub Python code and the Hearthstone cards benchmark, retrieve-and-edit significantly boosts the performance of a vanilla sequence-to-sequence model on both tasks.

## 📙Proposed Benchmark

- Benchmark Name: `Retrieve-and-edit's dataset`
- 📚Publisher/Date: `NeurIPS/2018`
- 🏠Author Affiliation: Stanford University
- 🔗URL: [https://worksheets.codalab.org/worksheets/0x1ad3f387005c492ea913cf0f20c9bb89](https://worksheets.codalab.org/worksheets/0x1ad3f387005c492ea913cf0f20c9bb89)
- Details: Our Python autocomplete dataset is a representative sample of Python code from GitHub, obtained from Google Bigquery by retrieving Python code containing at least one block comment with restructured text (reST) formatting. The dataset consists of `76k` functions, where the task is to predict the next token given partially written code and natural language description.
- Supported Metric: `BLEU`; `Accuracy`
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
    * [ ] Other Libraries
  + 🎯Level
  	* [x] Token Level
    * [ ] Line Level
    * [ ] Span Level
    * [ ] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 📘Reference

[^roberta]: [https://arxiv.org/pdf/1907.11692.pdf%5C](https://arxiv.org/pdf/1907.11692.pdf%5C)
[^codexglue]: [https://microsoft.github.io/CodeXGLUE](https://microsoft.github.io/CodeXGLUE)
[^mbpp]: [https://huggingface.co/datasets/Muennighoff/mbpp](https://huggingface.co/datasets/Muennighoff/mbpp)
[^codeforce]: [https://codeforces.com](https://codeforces.com)
[^codecontests]: [https://github.com/deepmind/code_contests](https://github.com/deepmind/code_contests)
[^apps]: [https://github.com/hendrycks/apps](https://github.com/hendrycks/apps)
[^humaneval]: [https://github.com/openai/human-eval](https://github.com/openai/human-eval)
[^gptneo]: [https://huggingface.co/docs/transformers/model_doc/gpt_neo](https://huggingface.co/docs/transformers/model_doc/gpt_neo)
[^codebert]: [https://github.com/microsoft/CodeBERT](https://github.com/microsoft/CodeBERT)
[^plbart]: [https://github.com/wasiahmad/PLBART](https://github.com/wasiahmad/PLBART)
[^codet5]: [https://github.com/salesforce/CodeT5](https://github.com/salesforce/CodeT5)
[^codeparrot]: [https://huggingface.co/codeparrot/codeparrot](https://huggingface.co/codeparrot/codeparrot)
[^polycoder]: [https://github.com/VHellendoorn/Code-LMs](https://github.com/VHellendoorn/Code-LMs)
[^gptj]: [https://huggingface.co/EleutherAI/gpt-j-6B](https://huggingface.co/EleutherAI/gpt-j-6B)
[^codegen]: [https://github.com/salesforce/CodeGen](https://github.com/salesforce/CodeGen)
[^gptneox]: [https://github.com/EleutherAI/gpt-neox](https://github.com/EleutherAI/gpt-neox)
[^lamda]: [https://blog.google/technology/ai/lamda](https://blog.google/technology/ai/lamda)
[^alphacode]: [https://www.deepmind.com/blog/competitive-programming-with-alphacode](https://www.deepmind.com/blog/competitive-programming-with-alphacode)
[^codex]: [https://arxiv.org/pdf/2107.03374.pdf](https://arxiv.org/pdf/2107.03374.pdf)
[^incoder]: [https://github.com/dpfried/incoder/blob/main/README.md](https://github.com/dpfried/incoder/blob/main/README.md)
[^codesearchnet]: [https://github.com/github/CodeSearchNet](https://github.com/github/CodeSearchNet)
[^spider]: [https://arxiv.org/pdf/1809.08887.pdf](https://arxiv.org/pdf/1809.08887.pdf)
[^nl2bash]: [https://aclanthology.org/L18-1491](https://aclanthology.org/L18-1491)
[^github-code]: [https://huggingface.co/datasets/lvwerra/github-code](https://huggingface.co/datasets/lvwerra/github-code)
[^gpt2]: [https://huggingface.co/gpt2](https://huggingface.co/gpt2)
[^gpt3]: [https://nl2code.github.io/posts/GPT-3-Language-Models-are-Few-Shot-Learners](https://nl2code.github.io/posts/GPT-3-Language-Models-are-Few-Shot-Learners)
[^django]: [https://github.com/odashi/ase15-django-dataset](https://github.com/odashi/ase15-django-dataset)
[^mtg-hs]: [https://github.com/deepmind/card2code](https://github.com/deepmind/card2code)
[^bigbench]: [https://github.com/google/BIG-bench](https://github.com/google/BIG-bench)
[^concode]: [https://github.com/sriniiyer/concode](https://github.com/sriniiyer/concode)
