---
title: GraphCoder
author: coder
date: 2024-06-11 00:00:00 +0800
categories: [arxiv]
tags: [models]
math: true
---

- 📙Paper: [GraphCoder: Enhancing Repository-Level Code Completion via Code Context Graph-based Retrieval and Language Model](https://arxiv.org/abs/2406.07003)
- 📚Publisher: `arxiv`
- 🏠Author Affiliation: `Peking University`, `Chinese Academy of Sciences`, `Huawei`
- GitHub: [https://github.com/oceaneLIU/GraphCoder](https://github.com/oceaneLIU/GraphCoder)
- Contribution: 
    + An approach GraphCoder to enhance the effectiveness of retrieval by a coarse-to-fine process, which considers both structural and lexical context, as well as the dependence distance between the completion target and the context;
    + A graph-based representation CCG (code context graph) of source code to capture relevant long-distance context for predicting the semantics of code completion target instead of the widely adopted sequence-based one;
    + Extensive experiments upon 5 LLMs and across 8000 code completion tasks from 20 repositories demonstrate that GraphCoder achieves higher exact match values with reduced retrieval time and overhead in database storage space.