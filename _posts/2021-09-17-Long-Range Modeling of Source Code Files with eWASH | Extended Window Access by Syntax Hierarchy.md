---
title: Long-Range Modeling of Source Code Files with eWASH | Extended Window Access by Syntax Hierarchy
author: coder
date: 2021-09-17 00:00:00 +0800
categories: [EMNLP]
tags: [methods, models, benchmarks, metrics]
math: true
image:
  path: /assets/imgs/eWASH.png
  width: 800
  height: 600
  alt: An example scenario where both method completion (top right) and code completion (bottom right) are performed by our eWASH models XPyMT5 and XGPT-C, respectively.
---

> Note that we only report the `nl2code` related parts.
{: .prompt-tip }

## 🌸Method

- 📙Title: [Long-Range Modeling of Source Code Files with eWASH Extended Window Access by Syntax Hierarchy](https://arxiv.org/pdf/2109.08780.pdf)
- 📚Publisher/Date: `EMNLP/2021`
- 🏠Author Affiliation: Microsoft Cloud and AI; Microsoft Research
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
    * [x] Pre-train and Fine-tune
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
    * [x] Abstract Syntax Tree (AST)
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
    * [ ] Other Platform
- 🗂️Downstream Benchmark
  + CodeXGLUE[^codexglue]
- ✈️Relevant Model
  + GPT-C[^gptc]
  + PyMT5[^pymt5]
  + XGPT-C
  + XPyMT5
- 💕Contribution
  + In this paper we introduce `eWASH`: Extended Window Access by Syntax Hierarchy, which leverages the syntax hierarchy of source code to give our models longer ranged vision by prioritizing higher level scopes and names for source code elements in a file which are not immediately in focus.
  + We also introduce new `CodeXGLUE` benchmarks[^codexglue] for userexperience-motivated tasks: code completion with normalized literals, method body completion/code summarization conditioned on filelevel context.

## 🎃Proposed Model#1

- Model Name: `XGPT-C`
- 📚Publisher/Date: `EMNLP/2021`
- 🏠Author Affiliation: Microsoft Cloud and AI; Microsoft Research
- Architecture: `Transformer-based neural networks (decoder)`
- Pre-Traing Corpus:  The corpus consists of all 5+ star GitHub repositories which are primarily Python, filtered by files which were either Python 3 compliant or were successfully fixed by lib2to3. Further, there was a time limit of `10` seconds placed on the parsing process to eliminate files which are essentially data files as they tend to contain very large lists for example. 
- Fine-tuning Corpus: We used the Py150 from CodeXGLUE[^codexglue], and for method and docstring completion we used the CodeSearchNet[^codesearchnet] dataset.
- Supported Natural Language: `English`
- Supported Programming Language: `Python`
- Model Size: `125M`
- Public Item: `None`
- 🔗URL: `None`

## 🎃Proposed Model#2

- Model Name: `XPyMT5`
- 📚Publisher/Date: `EMNLP/2021`
- 🏠Author Affiliation: Microsoft Cloud and AI; Microsoft Research
- Architecture: `Transformer-based neural networks (encoder-decoder)`
- Pre-Traing Corpus:  The corpus consists of all 5+ star GitHub repositories which are primarily Python, filtered by files which were either Python 3 compliant or were successfully fixed by lib2to3. Further, there was a time limit of `10` seconds placed on the parsing process to eliminate files which are essentially data files as they tend to contain very large lists for example. 
- Fine-tuning Corpus: We used the Py150 from CodeXGLUE[^codexglue], and for method and docstring completion we used the CodeSearchNet[^codesearchnet] dataset.
- Supported Natural Language: `English`
- Supported Programming Language: `Python`
- Model Size: `406M`
- Public Item: `None`
- 🔗URL: `None`

## 📙Proposed Benchmark

- Benchmark Name: `CodeXGLUE#code completion with normalized literals`; `CodeXGLUE#method body completion/code summarization conditioned on file-level context`
- 📚Publisher/Date: `EMNLP/2021`
- 🏠Author Affiliation: Microsoft Cloud and AI; Microsoft Research
- 🔗URL: `None`
- Sub-benchmark
  * CodeXGLUE#Py150[^py150]
  * CodeXGLUE#CodeSearchNet[^codesearchnet]
- Feature: Code completion with normalized literals; Method completion with file-level context
- Supported Metric: `PPL`; `ROUGE-L Prec.`; `Recall`; `Edit dist`; `EM@5(%)`
- Test Case: ❌
- 🔏Input (NL)
  + 🚩Language: `English`
  + 🌟Format
    * [x] Code Context
    * [x] Plain Natural Language
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
    * [ ] None
    * [ ] Class Information
    * [x] File Information
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
    * [ ] Token Level
    * [x] Line Level
    * [ ] Span Level
    * [x] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 🚩Proposed Metric

> The metric is proposed in SQuAD[^squad], and it was first introduced in `nl2code` for evaluating code completion models.
{: .prompt-info }

- Metric Name: `Exact Match@N (EM)`
- Definition: It counts the fraction of exactly correct predictions of some length (@N).

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
[^gptc]: [https://arxiv.org/pdf/2005.08025.pdf](https://arxiv.org/pdf/2005.08025.pdf)
[^pymt5]: [https://arxiv.org/pdf/2010.03150.pdf](https://arxiv.org/pdf/2010.03150.pdf)
[^py150]: [https://github.com/google-research-datasets/eth_py150_open](https://github.com/google-research-datasets/eth_py150_open)
[^squad]: https://arxiv.org/pdf/1606.05250.pdf
