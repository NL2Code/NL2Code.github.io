---
title: WizardCoder
author: coder
date: 2023-06-14 00:00:00 +0800
categories: [arxiv]
tags: [models]
math: true
pin: false
---

- 📙Paper: [WizardCoder: Empowering Code Large Language Models with Evol-Instruct](https://arxiv.org/abs/2306.08568.pdf)
- 📚Publisher: `arxiv`
- 🏠Author Affiliation: `Microsoft`
- 🔑Public: ✅
- 🌐Architecture
  + [ ] Encoder-Decoder
  + [x] Decoder-Only
- 📏Model Size
  + `15B`, `34B`
- 🍉Evol-Instruct
  + Streamlined the evolutionary instructions by removing deepening, complicating input, and In-Breadth Evolving.
  + Simplified the form of evolutionary prompts by unifying the evolutionary prompt template.
  + Addressing the specific characteristics of the code domain, we added two evolutionary instructions: code debugging and code time-space complexity constraints.
- 🌐Huggingface
  + https://huggingface.co/WizardLM/WizardCoder-15B-V1.0
  + https://huggingface.co/WizardLM/WizardCoder-Python-34B-V1.0
