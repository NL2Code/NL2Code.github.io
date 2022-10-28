---
title: Plotcoder | Hierarchical decoding for synthesizing visualization code in programmatic context
author: coder
date: 2021-03-01 00:00:00 +0800
categories: [ACL]
tags: [methods, models, benchmarks, metrics]
math: true
pin: false
---

## 🌸Method

- 📙Title: [PlotCoder: Hierarchical Decoding for Synthesizing Visualization Code in Programmatic Context](https://aclanthology.org/2021.acl-long.169.pdf)
- 📚Publisher/Date: `ACL/2021`
- 🏠Author Affiliation: `UC Berkeley`
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
    * [ ] Code Files
    * [ ] Test Cases
    * [x] Jupyter Notebooks
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
  + JuiCe[^juice]
- ✈️Base Model
  + RoBERTa-base
  + BERT-base
- 💕Contribution
  + We introduce PlotCoder, a new hierarchical encoder-decoder architecture that models both the code context and the input utterance. We use PlotCoder to first determine the template of the visualization code, followed by predicting the data to be plotted.
  + We use Jupyter notebooks to train PlotCoder. On a comprehensive set of test samples from those notebooks, we show that PlotCoder correctly predicts the plot type of about 70% samples, and synthesizes the correct programs for 35% samples, performing 34.5% better than the baseline[^plotcoder].

## 📚Proposed Benchmark

- Benchmark Name: `JuiCe`
- Publisher/Date: `ACL/2021`
- Author Affiliation: `UC Berkeley`
- Note: The benchmark used in this paper is adapted from [the original JuiCe paper](https://arxiv.org/abs/1910.02216).
- 🔗URL: [https://github.com/rajasagashe/juice](https://github.com/rajasagashe/juice)
- Feature: JuiCe provides refined human-curated data, open-domain code, and an order of magnitude more training data.
- Details: we present JuiCe, a corpus of `1.5` million examples with a curated test set of `3.7K` instances based on online programming assignments.
- Supported Metric: `plot type accuracy`; `plot data accuracy`; `program accuracy`
- Test Case： ❌
- 🔏Input (NL)
  + 🚩Language: `English`
  + 🌟Format
    * [ ] Code Context
    * [x] Plain Natural Language
    * [x] Code Snippet
    * [ ] Competition Problem
    * [ ] Code Comment
    * [ ] TODO
    * [ ] Pseudocode
    * [ ] Other Formats
  + 💈Description Granularity
    * [ ] Why? (Background)
    * [x] What? (Requirement, TODO)
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
    * [x] Public Library
    * [ ] Private Library
  + 🎯Level
  	* [ ] Token Level
    * [x] Line Level
    * [ ] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 🚩Proposed Metric

- Metric Name: `plot type accuracy`
- Definition: To compute this metric, we categorize all plots into several types, and a prediction is correct when it belongs to the same type as the ground truth. In particular, we consider the following categories: (1) scatter plots (e.g., generated by `plt.scatter`); (2) histograms (e.g., generated by `plt.hist`); (3) pie charts (e.g., generated by `plt.pie`); (4) a scatterplot overlaid by a line (e.g., generated by `sns.lmplot`); (5) a plot including a kernel density estimate (e.g., plots generated by `sns.distplot` or `sns.kdeplot`); and (6) others, which are mostly plots generated by `plt.plot`.

- Metric Name: `plot data accuracy`
- Definition: This metric measures whether the predicted program selects the same data to plot as the ground truth. Unless otherwise specified, the ordering of variables must match the ground truth as well, i.e., swapping the data used to plot `x` and `y` axes result in different plots.

- Metric Name: `program accuracy`
- Definition: We consider a predicted program to be correct if both the plot type and plotted data are correct. We do not evaluate the correctness of other plot attributes because they are mostly unspecified.

## 📘Reference

[^juice]: [https://github.com/rajasagashe/juice](https://github.com/rajasagashe/juice)
[^plotcoder]: [https://github.com/jungyhuk/plotcoder](https://github.com/jungyhuk/plotcoder)
