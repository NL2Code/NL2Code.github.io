---
title: A Dataset and Benchmark for Automatically Answering and Generating Machine Learning Final Exams
author: coder
date: 2022-06-11 00:00:00 +0800
categories: [arxiv]
tags: [benchmarks]
math: true
image:
  path: /assets/imgs/MIT.png
  width: 600
  height: 500
  alt: 500 MIT students taking the final exam in Introduction to Machine Learning in Fall 2021.
---

## 📙Proposed Benchmark

- Benchmark Name: `MLFinalsQ`[^mlfinalsq]
- 📚Publisher/Date: `Arxiv/2022`
- 🏠Author Affiliation: MIT; Columbia University
- 🔗URL: [https://github.com/idrori/mlfinalsQ](https://github.com/idrori/mlfinalsQ)
- Feature: We provide a new dataset and benchmark of questions from eight MIT Introduction to Machine Learning final exams between Fall 2017 and Spring 2022 and provide code for automatically answering these questions and generating new questions.
- Details: We present a new dataset of `496` questions from the eight most recent final exams of MIT’s Introduction to Machine Learning course. The dataset spans questions on the 12 machine learning topics covered in the course: (1) regression, (2) classifiers, (3) logistic regression, (4) features, (5) loss functions, (6) neural networks, (7) convolutional neural networks (CNNs), (8) Markov decision processes (MDPs), (9) recurrent neural networks (RNNs), (10) reinforcement learning, (11) clustering, and (12) decision trees.

![Window shadow](/assets/imgs/MIT-1.png){: .shadow width="300" height="400" .w-75 }
_The number of questions and parts in the final for each topic of Introduction to Machine Learning._

- Supported Metric: `grade score`
- Test Case: ❌
- 🔏Input (NL)
  + 🚩Language: `English`
  + 🌟Format
    * [ ] Code Context
    * [x] Plain Natural Language (Machine learning exam questions)
    * [ ] Competition Problem
    * [ ] Code Comment
    * [ ] TODO
    * [ ] Pseudocode
    * [ ] Other Formats
  + 💈Description Granularity
    * [x] Why? (Background)
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
    * [ ] Data Analysis and Manipulation
    * [ ] Plotting
    * [ ] Mathematical
    * [ ] Chemical
    * [x] Educational
    * [ ] Other Domains
  + 👑Library
    * [x] Build-in Library
    * [x] Public Library
    * [ ] Private Library
    * [ ] Other Libraries
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

[^mlfinalsq]: [https://arxiv.org/pdf/2206.05442v2.pdf](https://arxiv.org/pdf/2206.05442v2.pdf)
