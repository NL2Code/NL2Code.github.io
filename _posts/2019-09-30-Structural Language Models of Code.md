---
title: Structural Language Models of Code
author: coder
date: 2019-09-30 00:00:00 +0800
categories: [ICML]
tags: [methods, benchmarks, metrics]
math: true
image:
  path: /assets/imgs/StructuralLM.png
  width: 800
  height: 500
  alt: Examples from the Java (left) and C# (right) test sets.
---

## 🌸Method

- 📙Title: [Structural Language Models of Code]([https://arxiv.org/pdf/2107.03374.pdf](https://arxiv.org/pdf/1910.00577.pdf))
- 📚Publisher/Date: `ICML/2020`
- 🏠Author Affiliation: Technion, Israel; Tel Aviv University; Facebook AI Research
- 🔗URL: [https://github.com/tech-srl/slm-code-generation](https://github.com/tech-srl/slm-code-generation); [https://anycodegen.org/](https://anycodegen.org/)
- 🌐Neural Network (NN)
  + ⚒️Architecture
    * [ ] Feedforward NN (FNN)
    * [ ] Convolutional NN (CNN)
    * [ ] Recurrent NN (RNN)
    * [x] Long Short-Term Memory Neural Networks (LSTM)
    * [ ] Deep Belief Networks (DBN)
    * [ ] Variational Autoencoders (VAE)
    * [ ] Generative Adversarial Networks (GAN)
    * [ ] Diffussion
    * [x] Transformer-based Neural Networks including Encode and Decode
    * [ ] Other
  + ⚙️How to learn
    * [x] Supervised Transfer Learning
    * [ ] Unsupervised Transfer Learning
    * [ ] Reinforcement Learning (RL)
    * [ ] Multi-task Learning
    * [ ] Meta Learning
    * [ ] Contrastive Learning
    * [ ] Retrieved-based Learning
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
    * [ ] Google Code
    * [ ] Other Platform
- 🗂️Downstream Benchmark
  + Any-Code Completion#Java (see below)
  + Restricted Completion#C# (see below)
- 💕Contribution
  + We present a new approach that explicitly models the source and the target code as the same tree – structural language modeling (SLM).
  + Our model significantly outperforms both seq2seq and a variety of structured approaches in generating `Java` and `C#` code.
  + We release two datasets to evaluating our proposed approach.[^slm]

## 📙Proposed Benchmark#1

- Benchmark Name: `Any-Code Completion#Java`
- 📚Publisher/Date: `ICML/2020`
- 🏠Author Affiliation: Technion, Israel; Tel Aviv University; Facebook AI Research
- 🔗URL: [https://github.com/tech-srl/slm-code-generation](https://github.com/tech-srl/slm-code-generation)
- Sub-benchmark
  * Code2Seq[^code2seq]
- Details: We take the Java-small dataset of Alon et al. (2019a)[^code2seq], which is a re-split of the dataset of Allamanis et al. (2016)[^can-essc]. It contains 11 GitHub projects, broken down into a single method per example, and split to train/dev/test by project to reduce code overlap. This dataset was found to contain the least code duplication by Allamanis (2019)[^allamanis]. We create any-code completion examples by selecting every expression larger than a single AST node as the target, using the remainder of the method as the context. We remove methods containing the word “test” in their body or file name, and omit 10% of the examples by filtering out methods longer than 20 lines to avoid configurations, initializations, and auto-generated code. To make the task even harder, we remove examples where the target appears as-is in the context. Ultimately, this dataset contains `1.3M/10k/20k` train/dev/test examples.
- Supported Metric: `acc@k`; `tree@k`
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
  + 🚩Language: `Java`
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
    * [ ] Line Level
    * [x] Span Level
    * [ ] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 📙Proposed Benchmark#2

- Benchmark Name: `Restricted Completion#C#`
- 📚Publisher/Date: `ICML/2020`
- 🏠Author Affiliation: Technion, Israel; Tel Aviv University; Facebook AI Research
- 🔗URL: [https://github.com/tech-srl/slm-code-generation](https://github.com/tech-srl/slm-code-generation)
- Details: We use the code of Brockschmidt et al. (2019)[^gcmg] which filters out examples where the targets contain non-primitive types or user-defined functions. We extract the exact same types of limited expressions. Since the dataset of Brockschmidt et al. (2019)[^gcmg] is not publicly available, we consulted with Brockschmidt et al. directly and extracted examples from the raw dataset of Allamanis et al. (2018)[^lrpg] using their “unseen projects test” set. This dataset contains `30` GitHub projects broken down to one method per example. This dataset contains `16k/8k/3k` train/dev/test examples.
- Supported Metric: `acc@k`; `tree@k`
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
  + 🚩Language: `C#`
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
    * [ ] Line Level
    * [x] Span Level
    * [ ] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 🚩Proposed Metric

- Metric Name: `tree@k`
- Definition: It counts a prediction as correct if the entire tree structures, ignoring leaf values, are identical. For example, $x > 1$ and $y > 2$ would not count as identical in exact match, but would count as "tree-match identical" because both express that an identifier is greater than an integer (`NAME` > `INT`). The `tree@k` metric is interesting because it allows us to tease apart the model's syntactic errors from incorrect subtoken predictions.

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
[^slm]: [https://github.com/tech-srl/slm-code-generation](https://github.com/tech-srl/slm-code-generation)
[^allamanis]: [https://arxiv.org/pdf/1812.06469.pdf](https://arxiv.org/pdf/1812.06469.pdf)
[^can-essc]: [http://proceedings.mlr.press/v48/allamanis16.pdf](http://proceedings.mlr.press/v48/allamanis16.pdf)
[^code2seq]: [https://arxiv.org/pdf/1808.01400.pdf](https://arxiv.org/pdf/1808.01400.pdf)
[^lrpg]: [https://arxiv.org/pdf/1711.00740.pdf](https://arxiv.org/pdf/1711.00740.pdf)
[^gcmg]: [https://arxiv.org/pdf/1805.08490.pdf](https://arxiv.org/pdf/1805.08490.pdf)
