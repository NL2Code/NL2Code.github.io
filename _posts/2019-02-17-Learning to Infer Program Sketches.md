---
title: Learning to Infer Program Sketches
author: coder
date: 2019-02-17 00:00:00 +0800
categories: [ICML]
tags: [methods]
math: true
image:
  path: /assets/imgs/infer-sketch.png
  width: 800
  height: 500
  alt: Schematic overview of our model.
---

## 🌸Method

- 📙Title: [Learning to Infer Program Sketches](https://arxiv.org/pdf/1902.06349.pdf)
- 📚Publisher/Date: `ICML/2019`
- 🏠Author Affiliation: MIT Brain and Cognitive Sciences; MIT CSAIL; MIT-IBM AI Lab; Center for Brains, Minds and Machines (CBMM)
- 🔗URL: `None`
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
    * [ ] Prompt Design
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
    * [ ] Warnings, Errors, Bugs, Debug and Compilable Infos
    * [ ] API Document
    * [ ] Official Tutorial
    * [ ] Abstract Syntax Tree (AST)
    * [ ] Data/Control Flow (DF/CF)
    * [ ] Variable 
    * [ ] PL keywords
    * [ ] Code Comment
    * [ ] Natural Language to Code Pairs
    * [ ] Jupyter Notebook
    * [ ] Programmatic Idioms
    * [x] Code Sketches
    * [ ] Other Resources
  + 🚀Platform&Tool
    * [x] GitHub
    * [ ] Gitee
    * [ ] StackOverFlow
    * [ ] CodeForces
    * [ ] LeetCode
    * [ ] Google Code
    * [ ] Modulo Static Analysis Tool
    * [ ] Other Platform
- 🗂️Downstream Benchmark
  + Algolisp[^algolisp]
- 💕Contribution
  + We develop a novel neuro-symbolic program synthesis system, which writes programs from input-output examples and natural language specification by learning a suitable intermediate sketch representation between a neural network sketch generator and a symbolic synthesizer.
  + We introduce a novel training objective, which we used to train our system to find suitable sketch representations without explicit supervision.
  + We validate our system by demonstrating our results in two programming-by-example domains, list processing problems and string transformation problems, and achieve state-of-the-art performance on the AlgoLisp English-to-code test dataset.

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
[^conala]: [https://conala-corpus.github.io](https://conala-corpus.github.io)
[^algolisp]: [Neural Program Search Solving Programming Tasks from Description and Examples](https://arxiv.org/pdf/1802.04335.pdf)
