---
title: Beyond the Imitation Game | Quantifying and extrapolating the capabilities of language models
author: coder
date: 2022-06-09 00:00:00 +0800
categories: [arxiv]
tags: [benchmarks, metrics]
math: true
---

> Note that we only report the `nl2code` related parts.
{: .prompt-tip }

## 📙Proposed Benchmark

- Benchmark Name: `python programming challenge`[^bigbench]
- 📚Publisher/Date: `Arxiv/2022`
- 🔗URL: [https://github.com/google/BIG-bench/tree/main/bigbench/benchmark_tasks/python_programming_challenge](https://github.com/google/BIG-bench/tree/main/bigbench/benchmark_tasks/python_programming_challenge)
- Feature: This task tests the model's ability to solve coding challenges in python.
- Details: There are `32` total challenges in this task, categorized as very easy (`7`), easy (`14`), medium (`14`), and hard (`7`). Code that the model produces is compiled and run against test cases. Scores are computed for the number of solutions that compile and the accuracy of each solution across test cases.

  ```python
  # One example:
  Name: Binary addition
  Difficulty: Very Easy

  Example outputs:
  (2, 3) => 101
  (5, 12) => 10001
  (98, 99) => 11000101
  (459, 256) => 1011001011
  (1111, 111111) => 11011011001011110

  Prompt:
  # In this coding exercise, we write a python function which sum two positive integers and return the answer in binary. We do not use augmented assignment operations (+=, *=, etc.) for clarity.
  # The function 'binary_add' will take the arguments 'n1', an int and 'n2', an int. It will return a str.
  def binary_add(n1, n2):
  ```

- Supported Metric: `normalized prefered metric`
- Test Case： ✅
- 🔏Input (NL)
  + 🚩Language: `English`
  + 🌟Format
    * [ ] Code Context
    * [ ] Plain Natural Language
    * [x] Competition Problem
    * [ ] Code Comment
    * [ ] TODO
    * [ ] Pseudocode
    * [ ] Other Formats
  + 💈Description Granularity
    * [x] Why? (Background)
    * [x] What? (Requirement, Functionality, TODO)
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

## 🚩Proposed Metric

- Metric Name: `normalized prefered metric`
- Definition: Each BIG-bench task has a unique preferred metric, as well as high and low values for the task on this metric, as specified by the task authors. The low value indicates poor performance on the task, and the high value indicates excellent performance. When computing aggregate performance plots, we normalize the raw preferred score by subtracting the low score and normalizing the low to high score range to lie within 0–100.

  $$[normalized\quad prefered\quad metric]=100\times \frac{[raw\quad preferred\quad metric]-[low\quad score]}{[high\quad score]-[low\quad score]}$$
  
  Under this normalized preferred metric, tasks are calibrated so that a score of 0 corresponds to poor performance, and a score of 100 corresponds to very good performance. 


## 📘Reference

[^bigbench]: [https://github.com/google/BIG-bench](https://github.com/google/BIG-bench)
