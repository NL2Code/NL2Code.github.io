---
title: InCoder | A Generative Model for Code Infilling and Synthesis
author: coder
date: 2022-04-12 00:00:00 +0800
categories: [arxiv]
tags: [methods, models, benchmarks]
math: true
pin: false
---

## 🌸Method

- 📙Title: [InCoder A Generative Model for Code Infilling and Synthesis](https://arxiv.org/pdf/2204.05999.pdf)
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: Facebook AI Research; University of Washington; UC Berkeley; TTI-Chicago; Carnegie Mellon
- 🔗URL: [https://sites.google.com/view/incoder-code-models](https://sites.google.com/view/incoder-code-models)
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
    * [x] StackOverFlow
    * [ ] CodeForces
    * [ ] LeetCode
    * [ ] Other Platform
- 🗂️Downstream Benchmark
  + HumanEval[^humaneval]
  + MBPP[^mbpp]
  + CodeXGLUE[^codexglue]
- ✈️Relevant Model
  + RoBERTa[^roberta] (Finetuned)
  + CodeBERT[^codebert] (Finetuned)
  + PLBART[^plbart] (Finetuned)
  + CodeT5[^codet5] (Finetuned)
  + CodeParrot[^codeparrot]
  + PolyCoder[^polycoder]
  + GPT-J[^gptj]
  + CodeGen[^codegen]
  + GPT-NeoX[^gptneox]
  + LaMDA[^lamda]
  + AlphaCode[^alphacode]
  + Codex[^codex]
  + InCoder[^incoder]
- 💕Contribution
  + We introduce InCoder, a unified generative model that can perform program synthesis (via left-to-right generation) as well as editing (via infilling).
  + We find that the ability to condition on bidirectional context substantially improves performance on these tasks, while still performing comparably on standard program synthesis benchmarks in comparison to left-to-right only models pretrained at similar scale. The InCoder models and code are publicly released.[^incoder]


## 🎃Proposed Model

- Model Name: `InCoder`
- Publisher/Date: `Arxiv/2022`
- Author Affiliation: Facebook AI Research; University of Washington; UC Berkeley; TTI-Chicago; Carnegie Mellon
- Architecture: `Transformer-based neural networks (decoder)`
- Traing Corpus: `A lot of code files`
- Supported Natural Language: `English`; `Chinese`, etc.
- Supported Programming Language: `C`; `C++`; `CSS`; `C#`; `Common Lisp`; `Dart`; `Forth`; `Go`; `HTML`; `Haskell`; `Java`; `JavaScript`; `Julia`; `Jupyter`; `Kotlin`; `Lua`; `Matlab`; `PHP`; `Perl`; `Python`; `R`; `Ruby`; `Rust`; `SQL`; `Scala`; `Shell`; `Swift`; and `TypeScript`
- Model Size: `1.3B`; `6.7B`
- Public Item: `checkpoint`; `inference code`
- 🔗URL: [https://github.com/dpfried/incoder/blob/main/README.md](https://github.com/dpfried/incoder/blob/main/README.md)

## 📚Proposed Benchmark

> The paper does not name the dataset.
{: .prompt-warning }

- Benchmark Name: `HumanEvalInfilling-smline`
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: Facebook AI Research; University of Washington; UC Berkeley; TTI-Chicago; Carnegie Mellon
- 🔗URL: [https://github.com/dpfried/incoder/tree/main/evaluation](https://github.com/dpfried/incoder/tree/main/evaluation)
- Sub-benchmark
  * HumanEval[^humaneval]
- Feature: Single-line and multi-line infilling.
- Details: Different spans of non-empty lines in the canonical solutions of HumanEval[^humaneval] are turned into a FIM task.
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
    * [ ] Line Level
    * [ ] Span Level
    * [x] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels


## 📘Reference

[^roberta]: [https://arxiv.org/pdf/1907.11692.pdf](https://arxiv.org/pdf/1907.11692.pdf)
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
