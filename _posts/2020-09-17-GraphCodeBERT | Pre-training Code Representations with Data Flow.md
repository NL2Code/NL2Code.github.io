---
title: GraphCodeBERT | Pre-training Code Representations with Data Flow
author: coder
date: 2020-09-17 00:00:00 +0800
categories: [ICLR]
tags: [models]
math: true
image:
  path: /assets/imgs/GraphCodeBERT.png
  width: 800
  height: 400
  alt: An illustration about GraphCodeBERT pre-training.
---

> Note that we only report the `nl2code` related parts, the paper do not have any `nl2code` related downstream tasks, and the proposed model is focusing code understanding and can not be used directly for code generation.
{: .prompt-tip }

## 🎃Proposed Model

- Model Name: `GraphCodeBERT`[^graphcodebert]
- 📚Publisher/Date: `ICLR/2021`
- 🏠Author Affiliation: Sun Yat-sen University; Beihang University; Peking University; Harbin Institute of Technology; Microsoft Research Asia; Microsoft Devdiv; Microsoft STCA
- Architecture: `Transformer-based neural networks (encoder)`
- Pre-Traing Corpus: `A lot of code files` on GitHub
- Fine-tuning Corpus: The corpus of downstream task about evaluating code understanding
- Supported Natural Language: `English`
- Supported Programming Language: `Go`; `Java`; `JavaScript`; `PHP`; `Python`; `Ruby`
- Model Size: `125M`
- Public Item: `checkpoint`; `inference code`
- 🔗URL: [https://github.com/microsoft/CodeBERT/tree/master/GraphCodeBERT](https://github.com/microsoft/CodeBERT/tree/master/GraphCodeBERT)

## 📘Reference

[^graphcodebert]: [https://arxiv.org/pdf/2009.08366.pdf](https://arxiv.org/pdf/2009.08366.pdf)
