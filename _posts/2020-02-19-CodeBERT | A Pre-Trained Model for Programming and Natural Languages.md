---
title: CodeBERT | A Pre-Trained Model for Programming and Natural Languages
author: coder
date: 2020-02-19 00:00:00 +0800
categories: [EMNLP, Findings]
tags: [models]
math: true
image:
  path: /assets/imgs/CodeBERT.png
  width: 800
  height: 500
  alt: An illustration about the replaced token detection objective.
---

> Note that we only report the `nl2code` related parts, the paper do not have any `nl2code` related downstream tasks, and the proposed model is focusing code understanding and can not be used directly for code generation.
{: .prompt-tip }

## 🎃Proposed Model

- Model Name: `CodeBERT`[^codebert]
- 📚Publisher/Date: `EMNLP/2020`
- 🏠Author Affiliation: Harbin Institute of Technology; Sun Yat-sen University; Microsoft Research Asia; Microsoft Search Technology Center Asia
- Architecture: `Transformer-based neural networks (encoder)`
- Pre-Traing Corpus: `A lot of code files` on GitHub
- Fine-tuning Corpus: The corpus of downstream task about evaluating code understanding
- Supported Natural Language: `English`
- Supported Programming Language: `Go`; `Java`; `JavaScript`; `PHP`; `Python`; `Ruby`
- Model Size: `125M`
- Public Item: `checkpoint`; `inference code`
- 🔗URL: [https://github.com/microsoft/CodeBERT](https://github.com/microsoft/CodeBERT)

## 📘Reference

[^codebert]: https://arxiv.org/pdf/2002.08155.pdf
