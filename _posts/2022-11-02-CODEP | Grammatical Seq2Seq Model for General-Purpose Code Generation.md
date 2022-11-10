---
title: CODEP | Grammatical Seq2Seq Model for General-Purpose Code Generation
author: coder
date: 2022-11-02 00:00:00 +0800
categories: [arxiv]
tags: [methods]
math: true
image:
  path: /assets/imgs/example-parser.png
  width: 800
  height: 500
  alt: Examples of a parser parsing python code.
---

## 🌸Method

- 📙Title: [CODEP Grammatical Seq2Seq Model for General-Purpose Code Generation](https://arxiv.org/pdf/2211.00818.pdf)
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: Peking University
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
    * [x] Pre-train and Fine-tune
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
    * [x] Abstract Syntax Tree (AST)
    * [ ] Data/Control Flow (DF/CF)
    * [ ] Variable 
    * [ ] PL keywords
    * [ ] Code Comment
    * [x] Natural Language to Code Pairs
    * [ ] Jupyter Notebook
    * [ ] Programmatic Idioms
    * [ ] Code Sketches
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
  + CONALA[^conala]
  + DJANGO[^django]
  + MBPP[^mbpp]
- ✈️Relevant Model
  + [Tranx](https://nl2code.github.io/posts/Tranx-A-Transition-based-Neural-Abstract-Syntax-Parser-for-Semantic-Parsing-and-Code-Generation/)
  + [ML-Tranx](https://ojs.aaai.org/index.php/AAAI/article/download/17662/17469)
  + [Tranx-RL](https://arxiv.org/pdf/2106.00261)
  + [APT](https://nl2code.github.io/posts/Antecedent-Predictions-Are-Dominant-for-Tree-Based-Code-Generation/)
  + [BART](https://arxiv.org/pdf/1910.13461.pdf)
  + [CodeT5](https://arxiv.org/pdf/2109.00859.pdf)
  + [CodeGen](https://arxiv.org/pdf/2203.13474.pdf)
  + [InCoder](https://arxiv.org/pdf/2204.05999.pdf)
- 💕Contribution
  + We propose CODEP, a grammatical Seq2Seq code generation framework, which achieves significant improvements. To the best of our knowledge, we are the first to implement grammatical Seq2Seq models for general-purpose code generation successfully.
  + We propose a PDA module, which can be applied directly to Seq2Seq models without training to ensure that the generated code satisfies grammatical constraints.
  + We propose the state representation, state prediction task, and joint prediction for the decoder of CODEP. The first one enters additional valid information to CODEP. The second one enables CODEP to understand the workflow of the PDA module. The last one assists CODEP in avoiding the generation of code tokens of inappropriate PDA states.
  + Extensive experimental results also demonstrate the effectiveness of our proposed method, which outperforms the previous state-of-the-art methods on several benchmark datasets.

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
