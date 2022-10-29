---
title: Language to Code | Learning Semantic Parsers for If-This-Then-That Recipes
author: coder
date: 2015-05-12 00:00:00 +0800
categories: [ACL]
tags: [benchmarks]
math: true
image:
  path: /assets/imgs/DSL.png
  width: 800
  height: 500
  alt: Example recipe with description, with nodes corresponding to (a) Channels, (b) Functions, and (c) Parameters indicated with specific boxes. Note how some of the fields in braces, such as OccurredAt, depend on the trigger.
---

## 📙Proposed Benchmark

- Benchmark Name: `IFTTT corpus`
- 📚Publisher/Date: `ACL/2015`
- 🏠Author Affiliation: Microsoft Research; UT Austin
- 🔗URL: [http://research.microsoft.com/lang2code](http://research.microsoft.com/lang2code)
- Details: As of January 2015, we found `114,408` recipes[^recipes] on [http://ifttt.com](http://ifttt.com). Among the available recipes we encountered a total of `160` channels. In total, we found `552` trigger functions from `128` of those channels, and `229` action functions from `99` channels, for a total of `781` functions. Each recipe includes a number of pieces of information: description, note, author, number of uses, etc. `99.98%` of the entries have a description, and `35%` contain a note. Based on availability, we focused primarily on the description, though there are cases where the note is a more explicit representation of program intent.
- Supported Metric: `exact match`; `balanced F-measure`; `accuracy`
- Test Case: ❌
- 🔏Input (NL)
  + 🚩Language: `English`
  + 🌟Format
    * [ ] Code Context
    * [x] Plain Natural Language
    * [ ] Competition Problem
    * [ ] Code Comment
    * [ ] TODO
    * [ ] Pseudocode
    * [ ] Other Formats
  + 💈Description Granularity
    * [ ] Why? (Background)
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
  + 🚩Language: Domain Specific Language (DSL) `recipes`[^recipes]
  + ⛺Domain
    * [x] General
    * [ ] Data Analysis and Manipulation
    * [ ] Plotting
    * [ ] Mathematical
    * [ ] Chemical
    * [ ] Educational
    * [ ] Other Domains
  + 👑Library
    * [ ] Build-in Library
    * [ ] Public Library
    * [ ] Private Library
    * [ ] Other Libraries
  + 🎯Level
  	* [ ] Token Level
    * [ ] Line Level
    * [ ] Span Level
    * [ ] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [x] Other Levels

## 📘Reference

[^roberta]: [https://arxiv.org/pdf/1907.11692.pdf%5C](https://arxiv.org/pdf/1907.11692.pdf%5C)
[^codexglue]: [https://microsoft.github.io/CodeXGLUE](https://microsoft.github.io/CodeXGLUE)
[^mbpp]: [https://huggingface.co/datasets/Muennighoff/mbpp](https://huggingface.co/datasets/Muennighoff/mbpp)
[^codeforce]: [https://codeforces.com](https://codeforces.com)
[^codecontests]: [https://github.com/deepmind/code_contests](https://github.com/deepmind/code_contests)
[^apps]: [https://github.com/hendrycks/apps](https://github.com/hendrycks/apps)
[^humaneval]: [https://github.com/openai/human-eval](https://github.com/openai/human-eval)
[^gptneo]: [https://huggingface.co/docs/transformers/model_doc/gpt_neo](https://huggingface.co/docs/transformers/model_doc/gpt_neo)
[^codebert]: [https://github.com/microsoft/CodeBERT](https://github.com/microsoft/CodeBERT)
[^plbart]: [https://github.com/wasiahmad/PLBART](https://github.com/wasiahmad/PLBART)
[^codet5]: [https://github.com/salesforce/CodeT5](https://github.com/salesforce/CodeT5)
[^codeparrot]: [https://huggingface.co/codeparrot/codeparrot](https://huggingface.co/codeparrot/codeparrot)
[^polycoder]: [https://github.com/VHellendoorn/Code-LMs](https://github.com/VHellendoorn/Code-LMs)
[^gptj]: [https://huggingface.co/EleutherAI/gpt-j-6B](https://huggingface.co/EleutherAI/gpt-j-6B)
[^codegen]: [https://github.com/salesforce/CodeGen](https://github.com/salesforce/CodeGen)
[^gptneox]: [https://github.com/EleutherAI/gpt-neox](https://github.com/EleutherAI/gpt-neox)
[^lamda]: [https://blog.google/technology/ai/lamda](https://blog.google/technology/ai/lamda)
[^alphacode]: [https://www.deepmind.com/blog/competitive-programming-with-alphacode](https://www.deepmind.com/blog/competitive-programming-with-alphacode)
[^codex]: [https://arxiv.org/pdf/2107.03374.pdf](https://arxiv.org/pdf/2107.03374.pdf)
[^incoder]: [https://github.com/dpfried/incoder/blob/main/README.md](https://github.com/dpfried/incoder/blob/main/README.md)
[^codesearchnet]: [https://github.com/github/CodeSearchNet](https://github.com/github/CodeSearchNet)
[^spider]: [https://arxiv.org/pdf/1809.08887.pdf](https://arxiv.org/pdf/1809.08887.pdf)
[^nl2bash]: [https://aclanthology.org/L18-1491](https://aclanthology.org/L18-1491)
[^github-code]: [https://huggingface.co/datasets/lvwerra/github-code](https://huggingface.co/datasets/lvwerra/github-code)
[^gpt2]: [https://huggingface.co/gpt2](https://huggingface.co/gpt2)
[^gpt3]: [https://nl2code.github.io/posts/GPT-3-Language-Models-are-Few-Shot-Learners](https://nl2code.github.io/posts/GPT-3-Language-Models-are-Few-Shot-Learners)
[^django]: [https://github.com/odashi/ase15-django-dataset](https://github.com/odashi/ase15-django-dataset)
[^mtg-hs]: [https://github.com/deepmind/card2code](https://github.com/deepmind/card2code)
[^bigbench]: [https://github.com/google/BIG-bench](https://github.com/google/BIG-bench)
[^concode]: [https://github.com/sriniiyer/concode](https://github.com/sriniiyer/concode)
[^recipes]: Naturally-occurring programs are called "recipes".
