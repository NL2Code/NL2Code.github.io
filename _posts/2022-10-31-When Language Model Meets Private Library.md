---
title: When Language Model Meets Private Library
author: coder
date: 2022-10-31 00:00:00 +0800
categories: [EMNLP, Findings]
tags: [methods, models, benchmarks]
math: true
image:
  path: /assets/imgs/APICoder.png
  width: 800
  height: 500
  alt: The training process of APIRetriever and CodeGenAPI.
---

## 🌸Method

- 📙Title: [When Language Model Meets Private Library](https://arxiv.org/pdf/2210.17236.pdf)
- 📚Publisher/Date: `EMNLP/2022`
- 🏠Author Affiliation: Chinese Academy of Sciences; University of Chinese Academy of Sciences; Microsoft Research Asia
- 🔗URL: [https://github.com/microsoft/PyCodeGPT/tree/main/apicoder](https://github.com/microsoft/PyCodeGPT/tree/main/apicoder)
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
    * [x] API Document
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
  + TorchDataEval (see below)
  + MonkeyEval (see below)
  + BeatNumEval (see below)
- ✈️Relevant Model
  + CodeT5[^codet5]
  + CodeGPT[^codexglue]
  + CodeClippy[^codeclippy]
  + CodeParrot[^codeparrot]
  + CodeGen[^codegen]
  + Codex[^codex]
- 💕Contribution
  + We propose a new scenario called private-library-oriented code generation, and delicately model the task as the process of a programmer learning to write code using private libraries.
  + We propose a novel framework with two modules: the `APIRetriever` finds useful APIs, and then the `APICoder` generates code using these APIs.
  + Three benchmarks of private libraries including `TorchDataEval`, `MonkeyEval` and `BeatNumEval` are proposed to foster the evolution of this research area.

## 🎃Proposed Model

- Model Name: `CodeGenAPI`
- 📚Publisher/Date: `EMNLP/2022`
- 🏠Author Affiliation: Chinese Academy of Sciences; University of Chinese Academy of Sciences; Microsoft Research Asia
- Architecture: `Transformer-based neural networks (decoder)`
- Pre-Traing Corpus: `A lot of code files`
- Continual Pre-Training Corpus: API information + Code files
- Supported Natural Language: `English`
- Supported Programming Language: `Python`
- Model Size: `350M`
- Public Item: `checkpoint`; `training code`; `inference code`
- 🔗URL: [https://github.com/microsoft/PyCodeGPT/releases/download/Private-Library/CodeGenAPI-350M-mono.zip](https://github.com/microsoft/PyCodeGPT/releases/download/Private-Library/CodeGenAPI-350M-mono.zip)

## 📙Proposed Benchmark#1

- Benchmark Name: `TorchDataEval`
- 📚Publisher/Date: `EMNLP/2022`
- 🏠Author Affiliation: Chinese Academy of Sciences; University of Chinese Academy of Sciences; Microsoft Research Asia
- 🔗URL: [https://github.com/microsoft/PyCodeGPT/tree/main/apicoder/private-eval/data](https://github.com/microsoft/PyCodeGPT/tree/main/apicoder/private-eval/data)
- Feature: Private oriented code generation
- Details: To create a realistic benchmark for evaluating code generation for private library, we use TorchData, a Python library released just recently. We carefully learnt the official API documentation of TorchData and made sure we were proficient in all APIs. Then, we manually created `50` programming problems based on the API usage examples in the documentation. Two volunteers with extensive experience in Python were invited to check the correctness of each problem. We control the difficulty of the programming problems by the number of APIs in the target code. The percentage of programming problems containing `1` API, `2` APIs, and more APIs is set to `6:3:1`.
- Supported Metric: `pass@k`
- Test Case: ✅
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
    * [ ] Build-in Library
    * [ ] Public Library
    * [x] Private Library
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

## 📙Proposed Benchmark#2#3

- Benchmark Name: `MonkeyEval`; `BeatNumEval`
- 📚Publisher/Date: `EMNLP/2022`
- 🏠Author Affiliation: Chinese Academy of Sciences; University of Chinese Academy of Sciences; Microsoft Research Asia
- 🔗URL: [https://github.com/microsoft/PyCodeGPT/tree/main/apicoder/private-eval/data](https://github.com/microsoft/PyCodeGPT/tree/main/apicoder/private-eval/data)
- Feature: Private oriented code generation
- Details: They each contains 101 programming problems. They are modified from PandasEval and NumpyEval, which were proposed for the public libraries Pandas and Numpy[^cert]. In detail, we manually modified all library-related keywords in PandasEval and NumpyEval.
- Supported Metric: `pass@k`
- Test Case: ✅
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
    * [ ] Build-in Library
    * [ ] Public Library
    * [x] Private Library
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
[^codeclippy]: [https://github.com/CodedotAl/gpt-code-clippy](https://github.com/CodedotAl/gpt-code-clippy)
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
[^cert]: [https://arxiv.org/pdf/2206.06888.pdf](https://arxiv.org/pdf/2206.06888.pdf)
