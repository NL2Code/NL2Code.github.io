---
title: Efficient Training of Language Models to Fill in the Middle
author: coder
date: 2022-07-28 00:00:00 +0800
categories: [arxiv]
tags: [methods, models, benchmarks]
math: true
pin: false
---

> Note that we only report the `nl2code` related parts.
{: .prompt-tip }

## 🌸Method

- 📙Title: [Efficient Training of Language Models to Fill in the Middle]([https://arxiv.org/pdf/2107.03374.pdf](https://arxiv.org/pdf/2207.14255.pdf))
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: `OpenAI`
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
  + HumanEvalInfilling-smline[^humaneval-sm][^footnote]
  + HumanEvalInfilling-random[^footnote][^humaneval-rr]
- ✈️Relevant Model
  + InCoder[^incoder]
  + Codex[^codex]
- 💕Contribution
  + We perform an extensive scaling study by training a suite of 8 models, with and without FIM, and show that FIM can be learned without compromising the left-to-right capability in pretraining. We examine this claim in both code and language, using both perplexity and sampling-based benchmarks.
  + We clarify the effects of many hyperparameters related to training FIM models using comprehensive ablations. In particular, we study the FIM rate (the probability at which FIM transformation is applied to the data), different variants of FIM transformation, and the choice of middle span.
  + An alternative to training FIM models from scratch is to learn this capability by finetuning existing language models. We show that finetuning with FIM is computationally inefficient. While FIM can be learned for free during pretraining, learning FIM during finetuning requires a significant amount of additional compute to reach similar levels of performance as pretraining.
  + However since line-based evaluations do not capture all the use cases of FIM, we create two new benchmarks called random span infilling and random span infilling light.[^humaneval-rr]
  + We find that changing various hyperparameters in FIM training often leads to negligible differences in FIM test losses but large differences in sampling based benchmarks.

## 🎃Proposed Model

- Model Name: `FIM`
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: `OpenAI`
- Architecture: `Transformer-based neural networks (decoder)`
- Pre-Traing Corpus: `A lot of code files` same with Codex[^codex]
- Supported Natural Language: `English`
- Supported Programming Language: `Python`
- Model Size: `50M`; `77M`; `164M`; `411M`; `844M`; `1.4B`; `2.8B`; `6.9B`
- Public Item: `OpenAI API`
- 🔗URL: `None`

## 📚Proposed Benchmark

- Benchmark Name: `HumanEvalInfilling-random`
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: `OpenAI`
- 🔗URL: [https://github.com/openai/human-eval-infilling](https://github.com/openai/human-eval-infilling)
- Sub-benchmark
  * HumanEval[^humaneval]
- Feature: Span prediction.
- Details: For each HumanEval[^humaneval] problem, we create infilling tasks by selecting the middle span from the canonical solution uniformly at random.
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
  	* [x] Span Level
    * [ ] Line Level
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
[^humaneval-sm]: [https://arxiv.org/pdf/2204.05999.pdf](https://arxiv.org/pdf/2204.05999.pdf)
[^humaneval-rr]: [https://github.com/openai/human-eval-infilling](https://github.com/openai/human-eval-infilling)
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
[^codesearchnet]: [https://github.com/github/CodeSearchNet](https://github.com/github/CodeSearchNet)
[^footnote]: The original paper does not name the benchmark.
