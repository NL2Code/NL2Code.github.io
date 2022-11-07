---
title: A Systematic Evaluation of Large Language Models of Code
author: coder
date: 2022-06-13 00:00:00 +0800
categories: [ACM]
tags: [methods, models]
math: true
pin: false
---

## 🌸Method

- 📙Title: [A Systematic Evaluation of Large Language Models of Code](https://dl.acm.org/doi/pdf/10.1145/3520312.3534862)
- 📚Publisher/Date: `ACM/2022`
- 🏠Author Affiliation: `Carnegie Mellon University`
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
- ✈️Base Model
  + CodeParrot[^codeparrot]
  + GPT-Neo[^gptneo]
  + Codex[^codex]
  + PolyCoder[^polycoder]
- 💕Contribution
  + We aim to do a systematic evaluation of the largest existing models: Codex, GPT-J, GPT-Neo, GPT-NeoX-20B, and CodeParrot, across various programming languages.
  + We release a new model, PolyCoder, with 2.7B parameters based on the GPT-2 architecture, that was trained on 249GB of code across 12 programming languages on a single machine[^polycoder]. 

## 🎃Proposed Model

- Model Name: `PolyCoder`
- Publisher/Date: `ACM/2021`
- Author Affiliation: `Carnegie Mellon University`
- Architecture: `Transformer-based neural networks (decoder)`
- Traing Corpus: `A lot of code files`
- Supported Natural Language: `English`
- Supported Programming Language: `Python`; `C`; `C#`; `C++`; `Go`; `Java`; `JavaScript`; `PHP`; `Ruby`; `Rust`; `Scala`; `TypeScript`
- Model Size: `160M`; `400M`; `2.7B`
- Public Item: `checkpoint`; `training data`; `inference code`
- 🔗URL: [https://github.com/VHellendoorn/Code-LMs](https://github.com/VHellendoorn/Code-LMs)

## 📘Reference

[^humaneval]: [https://github.com/openai/human-eval](https://github.com/openai/human-eval)
[^codeparrot]: [https://github.com/huggingface/transformers/tree/main/examples/research_projects/codeparrot](https://github.com/huggingface/transformers/tree/main/examples/research_projects/codeparrot)
[^gptneo]: [https://huggingface.co/docs/transformers/model_doc/gpt_neo](https://huggingface.co/docs/transformers/model_doc/gpt_neo)
[^codex]: [Evaluating Large Language Models Trained on Code](https://arxiv.org/abs/2107.03374)
[^polycoder]: [https://github.com/VHellendoorn/Code-LMs](https://github.com/VHellendoorn/Code-LMs)
