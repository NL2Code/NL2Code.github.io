---
title: Shellcode_IA32 | A Dataset for Automatic Shellcode Generation
author: coder
date: 2021-04-27 00:00:00 +0800
categories: [ACL, NLP4Prog]
tags: [benchmarks]
math: true
image:
  path: /assets/imgs/shellcodeIA32.png
  width: 800
  height: 500
  alt: x86 assembly code used to spawn /bin/sh shell on Linux OS.
---

## 📙Proposed Benchmark

- Benchmark Name: `Shellcode_IA32`[^shellcode_ia32]
- 📚Publisher/Date: `ACL/2021`
- 🏠Author Affiliation: University of Naples Federico II; University of North Carolina at Charlotte
- 🔗URL: https://github.com/dessertlab/Shellcode_IA32
- Details: This dataset consists of `3,200` examples of instructions in assembly language for IA-32 (the 32-bit version of the x86 Intel Architecture) from publicly-available security exploits.

  ```bash
  Intent: jump short to the decode label if the contents of the al register is not equal to the contents of the cl register else jump to the shellcode label
  Multi-line Snippets: cmp al, cl \n jne short decode \n jmp shellcode

  Intent: jump to the label recv http request if the contents of the eax register is not zero else subtract the value 0x6 from the contents of the ecx register 
  Multi-line Snippets: test eax, eax \n jnz recv http request \n sub ecx, 0x6
  ```

- Supported Metric: `BLEU`; `Accuracy`
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
  + 🚩Language: `Shell`
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
    * [x] Line Level
    * [ ] Span Level
    * [ ] Function Level
    * [ ] Class Level
    * [ ] File Level
    * [ ] Repository Level
    * [ ] Other Levels

## 📘Reference

[^shellcode_ia32]: [https://aclanthology.org/2021.nlp4prog-1.7.pdf](https://aclanthology.org/2021.nlp4prog-1.7.pdf)
