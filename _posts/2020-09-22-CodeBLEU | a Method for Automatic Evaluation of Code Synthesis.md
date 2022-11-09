---
title: CodeBLEU | a Method for Automatic Evaluation of Code Synthesis
author: coder
date: 2020-09-22 00:00:00 +0800
categories: [arxiv]
tags: [metrics]
math: true
image:
  path: /assets/imgs/codebleu.png
  width: 800
  height: 500
  alt: The proposed CodeBLEU, a weighted syntactic and semantic BLEU for code synthesis evaluation, consists of the original BLEU, the weighted n-gram match, the syntactic AST match, and the semantic data-flow match.
---

## 🚩Proposed Metric

- Metric Name: `CodeBLEU`
- Definition: It defines as the weighted combination of four parts: $CodeBLEU=\alpha \cdot BLEU+\beta \cdot BLEU_{weight} + \gamma \cdot Match_{ast} + \delta \cdot Match_{df}$. where BLEU is calculated by standard BLEU, $BLEU_{weight}$ is the weighted n-gram match, obtained by comparing the hypothesis code and the reference code tokens with different weights, $Match_{ast}$ is the syntactic AST match, exploring the syntactic information of code, and $Match_{df}$ is the semantic dataflow match, considering the semantic similarity between the hypothesis and the reference.  The weighted ngram match and the syntactic AST match are used to measure grammatical correctness, and the semantic data-flow match is used to calculate logic correctness.
- 😄Merits and 😒Demeritsa
  + The difference in CodeBLEU metric is reliable. CodeBLEU is capable to differentiate code synthesis systems.
  + CodeBLEU is reliable, and its variance is within a reasonable range.
  + CodeBLEU is more correlated with human evaluation scores than traditional BLEU scores on all the three tasks, and more correlated than Acc on the two tasks.
