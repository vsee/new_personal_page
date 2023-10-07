---
title: "Large Language Models for Compiler Optimization"
collection: publications
permalink: /publication/2023_arxiv_llm_compiler
excerpt: 'We explore the novel application of Large Language Models to code optimization.'
date: 2023-10-11
venue: 'arXiv'
citation: 'Cummins, Chris, Volker Seeker, Dejan Grubisic, Mostafa Elhoushi, Youwei Liang, Baptiste Roziere, Jonas Gehring, et al. “Large Language Models for Compiler Optimization.” arXiv, September 11, 2023. https://doi.org/10.48550/arXiv.2309.07062.'
---

# Abstract

We explore the novel application of Large Language Models to code optimization. We present a 7B-parameter transformer model trained from scratch to optimize LLVM assembly for code size. The model takes as input unoptimized assembly and outputs a list of compiler options to best optimize the program. Crucially, during training, we ask the model to predict the instruction counts before and after optimization, and the optimized code itself. These auxiliary learning tasks significantly improve the optimization performance of the model and improve the model's depth of understanding.
We evaluate on a large suite of test programs. Our approach achieves a 3.0% improvement in reducing instruction counts over the compiler, outperforming two state-of-the-art baselines that require thousands of compilations. Furthermore, the model shows surprisingly strong code reasoning abilities, generating compilable code 91% of the time and perfectly emulating the output of the compiler 70% of the time.
of migratable kernels.

# Resources

[Paper](https://arxiv.org/abs/2309.07062)
