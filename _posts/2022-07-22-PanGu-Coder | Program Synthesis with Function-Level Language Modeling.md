---
title: PanGu-Coder | Program Synthesis with Function-Level Language Modeling
author: coder
date: 2021-07-22 00:00:00 +0800
categories: [arxiv]
tags: [methods, models, benchmarks, metrics]
math: true
pin: false
---

## 🌸Method

- 📙Title: [Evaluating Large Language Models Trained on Code](https://arxiv.org/pdf/2107.03374.pdf)
- 📚Publisher/Date: `Arxiv/2021`
- 🏠Author Affiliation: `OpenAI`
- 🔗URL: [xxx]
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

- Model Name: `Codex`
- Publisher/Date: `Arxiv/2021`
- Author Affiliation: `OpenAI`
- Architecture: `Transformer-based neural networks (decoder)`
- Traing Corpus: `A lot of code files`
- Supported Natural Language: `English`
- Supported Programming Language: `Python`
- Model Size: `12M`; `25M`; `42M`; `85M`; `300M`; `679M`; `2.5B`; `12B`; `175B`
- Public Item: `checkpoint`; `training data`; `training code`; `inference code`
- 🔗URL: `None`

## 📚Proposed Benchmark

- Benchmark Name: `HumanEval`
- Publisher/Date: `Arxiv/2021`
- Author Affiliation: `OpenAI`
- 🔗URL: [https://github.com/openai/human-eval](https://github.com/openai/human-eval)
- Sub-benchmark
  * XXX
- Feature: Multi-turn Evaluation
- Supported Metric: `pass@k`; `EM`; `ES`; `Accuracy`; `BLEU`; `CodeBLEU`
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

- Metric Name: `pass@k`
- Definition: We generate $n \geq k$ samples per task (in this paper, we use $n=200$ and $k \leq 100$), count the number of correct samples $c \leq n$ which pass unit tests. If $n - c < k$, then pass@k=1; otherwise, pass@k = $1-\prod\nolimits_{i=n-c+1}^{n} (1-k/i)$.
- 😄Merits and 😒Demerits
  + This allows to accurately evaluate the produced code quality via test cases.
  + Annotating test cases is difficult and costly.


## ⛳Products

- 📗Product Name: [Copilot](https://github.com/features/copilot/)
- Date: `2021-06-29`
- Developer: `GitHub`; `OpenAI`
- ☂️Technology
  + [x] Pre-trained model
    * Codex
  + [ ] Other rule-based method
- 🔏Supported Natural Language (NL): `English`; `Chinese` and so on
- 🔑Supported Programming Language (PL): `Python`; `TypeScript`; `JavaScript`; `Java`; `Ruby`; `Go`; `C#`; `C++` and so on
- 🚗Supported Integrated Development Environment (IDE): `Visual Studio Code`; `Visual Studio`; `Neovim`; `JetBrains IDEs`
- 🔆Supported Feature
  + Generating one or more code snippets
- Is It Free: `No`

## 📘Reference

[^roberta]: [https://arxiv.org/pdf/1907.11692.pdf%5C](https://arxiv.org/pdf/1907.11692.pdf%5C)
[^codexglue]: [https://microsoft.github.io/CodeXGLUE](https://microsoft.github.io/CodeXGLUE)
[^mbpp]: [https://huggingface.co/datasets/Muennighoff/mbpp](https://huggingface.co/datasets/Muennighoff/mbpp)
[^codeforce]: [https://codeforces.com](https://codeforces.com)
[^codecontests]: [https://github.com/deepmind/code_contests](https://github.com/deepmind/code_contests)
[^apps]: [https://github.com/hendrycks/apps](https://github.com/hendrycks/apps)
[^humaneval]: [https://github.com/openai/human-eval](https://github.com/openai/human-eval)
[^gpeneo]: [https://huggingface.co/docs/transformers/model_doc/gpt_neo](https://huggingface.co/docs/transformers/model_doc/gpt_neo)
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
