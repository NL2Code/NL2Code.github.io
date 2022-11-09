---
title: Analytical Papers of Code Generation
author: coder
date: 2022-01-01 00:00:00 +0800
categories: [other]
tags: [other]
math: true
---

| **Title** | **Analyzed Question** | **Affiliation** | **Publisher/Date** |
| :---- | :---------------- | :-------------- | :----------------- |
| [A Systematic Evaluation of Large Language Models of Code](https://dl.acm.org/doi/pdf/10.1145/3520312.3534862) | How to systematic evaluate large language model of code? | Carnegie Mellon University | ACM/2022 |
| [Exploring and Evaluating Personalized Models for Code Generation](https://arxiv.org/pdf/2208.13928.pdf) | The goal of our experimental design is to investigate whether custom models outperform the baseline model, leading to performance improvements in terms of intrinsic metrics (RQ1), as well as extrinsic task-specific metrics (RQ2). Next, we analyze and compare the different customization approaches in terms of training and compute costs (RQ3) as well as model size and required storage for deployment. | McGill University; Anthropic; Microsoft | FSE/2022 |
| [Memorization and Generalization in Neural Code Intelligence Models](https://arxiv.org/pdf/2106.08704.pdf) | The goal of this paper is to evaluate and compare the extent of memorization and generalization in neural code intelligence models. It aims to provide insights on how memorization may impact the learning behavior of neural models in code intelligence systems. | University of Houston; Carnegie Mellon University | 	Information and Software Technology/2022 |
| [To What Extent do Deep Learning-based Code Recommenders Generate Predictions by Cloning Code from the Training Set?](https://arxiv.org/pdf/2204.06894.pdf) | The goal of this study is to understand the extent to which DL-based code recommenders are prone to suggest code snippets being clones of instances present in the training set. | Università della Svizzera italiana | ACM/2022 |
| [Looking for a Handsome Carpenter! Debiasing GPT-3 Job Advertisements](https://arxiv.org/pdf/2205.11374.pdf) | Our goal is to generate job ads that are (1) unbiased, i.e., do not encourage or discourage application from one gender; and (2) realistic, i.e., of a quality comparable to human-generated ads. | University of Oxford | NAACL/2022 |
| [Large Language Models are Not Models of Natural Language: They are Corpus Models](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9794684) | We argue as a corollary that the term language model is misleading and propose the adoption of the working term corpus model instead, which better reflects the genesis and contents of the model. | University of Bergen | IEEE/2022	|
| [Neural Models for Automatic Program Repair vs. Human Developers](https://elib.uni-stuttgart.de/bitstream/11682/12293/1/master_thesis_dominik_huber.pdf) | RQ1: How do human developers and APR approaches compare in terms of repair performance? RQ2: Do the attention vectors extracted from APR approaches correlate to those of the human participants? RQ3: Is there a relationship between high human-model correlation and model repair performance? RQ4: What proportion of their attention do developers and models pay to the buggy line versus the surrounding context? RQ5: How much attention do developers and humans pay to different types of tokens? RQ6: What patterns are there in the behavior of human developers?| University of Stuttgart | Other/2022	|
| [AI Challenges for Society and Ethics](https://arxiv.org/pdf/2206.11068.pdf) | We begin by outlining some of the benefits and opportunities AI promises for society, before turning to some of the most concerning sources of harm and risk AI might pose. We then discuss the kinds of ethical and political challenges that arise in trying to balance these benefits and risks, before concluding with some recommendations for AI governance today. | University of Cambridge | The Oxford Handbook of AI Governance/2022	|
| [Exploring Length Generalization in Large Language Models](https://arxiv.org/pdf/2207.04901.pdf) | We study combinations of three kinds of techniques for LLMs: finetuning, few shot prompting (also referred to as in-context learning), and use of a scratchpad (also referred to as chain-of-thought), to understand the role of each method and the interplay among the three in length generalization. | Google Research | Arxiv/2022	|
| [A Case Study on Machine Learning for Synthesizing Benchmarks](https://sertel.github.io/files/synthetic_benchmarks_mapl_2019.pdf) | We have re-evaluated the use of machine learning in CLgen, a method for mining OpenCL kernels from Github and training a generative model from them to produce OpenCL benchmarks. | TU Dresden; University of Edinburgh | ACM MAPL/2019	|
| [Synthesizing Benchmarks for Predictive Modeling](https://www.research.manchester.ac.uk/portal/files/157727841/CGO17_Clgen.pdf) | Generating valid, executable program code is an ambitious and challenging goal for unsupervised machine learning. We employ state of the art deep language modeling techniques to achieve this task. | University of Edinburgh; Lancaster University | IEEE/2017	|
| [Choose Your Programming Copilot: A Comparison of the Program Synthesis Performance of GitHub Copilot and Genetic Programming](https://arxiv.org/pdf/2111.07875.pdf) | We evaluate GitHub Copilot on standard program synthesis benchmark problems and compare the achieved results with those from the genetic programming literature. In addition, we discuss the performance of both approaches. | Johannes Gutenberg University | ACM GECCO/2022	|
| [Asleep at the Keyboard? Assessing the Security of GitHub Copilot’s Code Contributions](https://arxiv.org/pdf/2108.09293.pdf?nylayout=pc) | We perform automatic and manual analysis of Copilot's software and hardware code completion behavior in response to "prompts" handcrafted to represent security-relevant scenarios and characterize the impact that patterns in the context can have on the AI’s code generation and confidence. We discuss implications for software and hardware designers, especially security novices, when using AI pair programming tools. This work is accompanied by the release of our repository of security-relevant scenarios. | New York University; University of Calgary | IEEE Symposium on Security and Privacy/2022	|
| [An empirical evaluation of GitHub copilot's code suggestions](https://dl.acm.org/doi/abs/10.1145/3524842.3528470) | In this paper, we perform an empirical study to evaluate the correctness and understandability of Copilot's suggested code. | University of Alberta | MSR/2022	|
| [Expectation vs. Experience: Evaluating the Usability of Code Generation Tools Powered by Large Language Models](https://tianyi-zhang.github.io/files/chi2022-lbw-copilot.pdf) | RQ1: How does using Copilot affect the programming experience? RQ2: How do users recognize errors in code generated by Copilot? RQ3: What coping mechanisms do users employ when they find errors in code generated by Copilot? RQ4: What are the obstacles and limitations that can prevent adoption of Copilot? | Harvard University; Purdue University | CHI EA/2022	|
| [Capturing Failures of Large Language Models via Human Cognitive Biases](https://arxiv.org/pdf/2202.12299.pdf) | Large language models generate complex, openended outputs: instead of outputting a single class, they can write summaries, generate dialogue, and produce working code. In order to study the reliability of these open-ended systems, we must understand not just when they fail, but also how they fail. | University of California | Arxiv/2022	|
| [An Extensive Study on Pre-trained Models for Program Understanding and Generation](https://lingming.cs.illinois.edu/publications/issta2022.pdf) | RQ1: How do pre-trained models perform for program understanding and generation tasks? RQ2: How do pre-trained models perform against non-pre-trained models? RQ3: Are the pre-trained models robust? | Southern University of Science and Technology; The Hong Kong Polytechnic University; Kwai Inc.; University of Illinois Urbana-Champaign | ISSTA/2022	|
|  |  |  | 	|
|  |  |  | 	|
|  |  |  | 	|
|  |  |  | 	|
|  |  |  | 	|
|  |  |  | 	|
|  |  |  | 	|
|  |  |  | 	|
|  |  |  | 	|
|  |  |  | 	|
|  |  |  | 	|
|  |  |  | 	|
|  |  |  | 	|
|  |  |  | 	|
|  |  |  | 	|
|  |  |  | 	|


