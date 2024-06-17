---
title: ReflectionCoder
author: coder
date: 2024-05-27 00:00:00 +0800
categories: [arxiv]
tags: [models]
math: true
---

- 📙Paper: [ReflectionCoder Learning from Reflection Sequence for Enhanced One-off Code Generation](https://arxiv.org/pdf/2405.17057)
- 📚Publisher: `arxiv`
- 🏠Author Affiliation: `Shanghai Jiao Tong University`, `SenseTime Research`, `Shanghai Artificial Intelligence Laboratory`, `CUHK MMLab`, `CPII under InnoHK`
- GitHub: [https://github.com/SenseLLM/ReflectionCoder](https://github.com/SenseLLM/ReflectionCoder)
- Contributions:
    + We constructed a reflection sequence dataset, a two-round dialogue dataset composed of reflection sequence and code generation. The dataset can effectively guide code LLMs fine-tuning to obtain better one-off generation performance.
    + We proposed to leverage reflection sequences to guide the fine-tuning of code LLMs. On top of the idea, we propose two techniques to effectively utilize the reflection sequence data, namely reflection self-distillation and dynamically masked distillation.
    + Extensive experiments on HumanEval (+), MBPP (+), and MultiPl-E demonstrate the effectiveness of the proposed method on one-off code generation. ReflectionCoder-DeepSeek-Coder-33B reaches 82.9 (76.8) on HumanEval (+) and 84.1 (72.0) on MBPP (+), which is an on-par performance of GPT-3.5-Turbo and Claude-3-opus and surpasses early GPT-4.