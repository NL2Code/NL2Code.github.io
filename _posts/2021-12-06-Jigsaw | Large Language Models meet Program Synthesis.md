---
title: Jigsaw | Large Language Models meet Program Synthesis
author: coder
date: 2021-12-06 00:00:00 +0800
categories: [ACM, ICSE]
tags: [methods, benchmarks]
math: true
image:
  path: /assets/imgs/jigsaw.png
  width: 800
  height: 500
  alt: Architecture of Jigsaw.
---

## 🌸Method

- 📙Title: [Jigsaw Large Language Models meet Program Synthesis](https://arxiv.org/pdf/2112.02969.pdf)
- 📚Publisher/Date: `ICSE/2021`
- 🏠Author Affiliation: Microsoft Research; Standford University
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
    * [x] In-context Learning
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
    * [x] Executable
    * [ ] Dynamic/Statical PL
    * [ ] Procedure/Object/Aspect Orient PL
    * [ ] Other Characteristics
  + 🪵Resource
    * [x] Code Files
    * [x] Test Cases
    * [ ] Repositories
    * [x] Warnings, Errors, Bugs and Debug Infos
    * [ ] API Document
    * [ ] Official Tutorial
    * [x] Abstract Syntax Tree (AST)
    * [ ] Data/Control Flow (DF/CF)
    * [x] Variable
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
  + PandasEval1[^pandaseval12]
  + PandasEval2[^pandaseval12]
- ✈️Relevant Model
  + GPT-3[^gpt3]
  + Codex[^codex]
- 💕Contribution
  + We present an architecture to perform code synthesis by augmenting black-box PTLMs with program analysis and synthesis-based techniques and multi-modal specifications. We have implemented the architecture in a tool called Jigsaw. We have developed a Jupyter notebook extension that allows users to interact with the system seamlessly.
  + We characterize common classes of errors made by PTLMs, namely, reference errors, argument errors, and semantic errors. Motivated by these errors, we have designed program analysis and synthesis techniques in Jigsaw to fix such errors in code snippets produced by PTLMs. We have also designed techniques to learn from user feedback and improve with usage.
  + We have created two Pandas datasets with multi-modal specifications (provided in the supplementary material, and to be released for community use). Using two state-of-the-art PTLMs, we show that Jigsaw yields significantly higher accuracy compared to baselines on the two datasets.

## 📙Proposed Benchmark

- Benchmark Name: `PandasEval1`; `PandasEval2`
- 📚Publisher/Date: `ICSE/2021`
- 🏠Author Affiliation: Microsoft Research; Standford University
- 🔗URL: [https://github.com/microsoft/JigsawDataset](https://github.com/microsoft/JigsawDataset)
- Details: 
  + `PandasEval1` consists of `68` Python Pandas tasks. Each task can be solved using a single line of code by composing at most `2-3` Pandas functions; sometimes followed by assigning variables. This dataset was created by authors of this paper by going through queries in online forums like StackOverflow.
  + `PandasEval2`consists of `21` Pandas tasks; each task can be solved by composing at most `2-3` Pandas functions, possibly followed by assigning variables, as in the PandasEval1 dataset. We posed these tasks as illustrations, in a hackathon we conducted with `25` users over `2` different sessions.
- Supported Metric: `mean accuracy`; `std. deviation`
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
    * [ ] General
    * [x] Data Analysis and Manipulation
    * [x] Plotting
    * [ ] Mathematical
    * [ ] Chemical
    * [ ] Educational
    * [ ] Other Domains
  + 👑Library
    * [ ] Build-in Library
    * [x] Public Library
    * [ ] Private Library
  + 🎯Level
  	* [ ] Token Level
    * [x] Line Level
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
[^pandaseval12]: [https://github.com/microsoft/JigsawDataset](https://github.com/microsoft/JigsawDataset)
