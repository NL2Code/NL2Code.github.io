---
title: Training and Evaluating a Jupyter Notebook Data Science Assistant
author: coder
date: 2022-01-30 00:00:00 +0800
categories: [AAAI]
tags: [methods, models]
math: true
---

## 🌸Method

- 📙Title: [Training and Evaluating a Jupyter Notebook Data Science Assistant](https://arxiv.org/pdf/2201.12901.pdf)
- 📚Publisher/Date: `AAAI/2022`
- 🏠Author Affiliation: Microsoft
- 🔗URL: [https://github.com/microsoft/DataScienceProblems](https://github.com/microsoft/DataScienceProblems)
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
    * [ ] Code Files
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
    * [x] Jupyter Notebook
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
  + HumanEval[^humaneval]
  + MBPP[^mbpp]
- ✈️Relevant Model
  + Codex[^codex]
  + PyMT5[^pymt5]
- 💕Contribution
  + We introduce a new evaluation called Data Science Problems (DSP), a curated set of pedagogical Python notebooks and data contexts containing rich Markdown descriptions of problems, solutions, and unit tests, which uses the teaching tool `nbgrader`[^nbgrader] to automatically evaluate model hypotheses.
  + We introduce a new 'code-infilling' pre-training objective, similar to span-mask pre-training and the method-feature-filling objective of PyMT5[^pymt5], wherein each cell in each notebook is considered a target in one example, and the source is the neighboring cells with a control code indicating which cell type to produce and where it should be inserted. The resulting model trained by this objective is called JuPyT5 – Jupyter Python Text-to-text Transfer Transformer.
  + While we do not follow the trend of exploring model size, we focus on evaluating a model size with more modest deployment cost by training and evaluating one model size of 350M parameters (300M non-embedding parameters). We evaluate this model size trained on the cell-infilling objective for our new DSP metric, showing it can solve 78% of the DSP tasks given 100 sampled attempts. We find similarly that model performance improves with larger number of samples, and more context cells improves the model performance. Surprisingly, training the model with the ability to look ahead a single cell doubles the performance on DSP compared to a 3-cell look-back baseline. Showing the model unit tests also improves performance, and interestingly, the model learns to adapt the solutions to previous problems on a subsequent problem.
  + We also evaluate JuPyT5 on HumanEval and MBPP. JuPyT5 can beat a much larger 68B parameter model at MBPP with a modest 300M parameters, but was also explicitly trained only on code domain sources. While large models are very impressive general-learners from diverse data sources, it is still much more economical to focus a model training on a task domain. JuPyT5 was outperformed by a similar-sized Codex model on HumanEval, but we were able to partially close the gap by adapting HumanEval docstrings to look more like Markdown. We conclude naturally that smaller models are more formatting-sensitive.

## 🎃Proposed Model

- Model Name: `JuPyT5`
- 📚Publisher/Date: `AAAI/2022`
- 🏠Author Affiliation: Microsoft
- Architecture: `Transformer-based neural networks (encoder-decoder)`
- Pre-Traing Corpus: `A lot of Jupyter Notebooks from GitHub`
- Supported Natural Language: `English`
- Supported Programming Language: `Python`
- Model Size: `350M`
- Public Item: `training data`
- 🔗URL: [https://github.com/microsoft/DataScienceProblems](https://github.com/microsoft/DataScienceProblems)

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
[^pymt5]: [https://nl2code.github.io/posts/PyMT5-multi-mode-translation-of-natural-language-and-Python-code-with-transformers](https://nl2code.github.io/posts/PyMT5-multi-mode-translation-of-natural-language-and-Python-code-with-transformers)
[^nbgrader]: [https://nbgrader.readthedocs.io/en/stable](https://nbgrader.readthedocs.io/en/stable)
