---
title: 'Revealing Compiler Heuristics through Automated Discovery and Optimization'
collection: publications
permalink: /publication/2024_cgo_heureka
excerpt: 'We present Heureka, a tool to automatically discover heuristic functions in compiler source code.'
date: 2024-02-19
venue: 'CGO'
citation: 'TBD'
---

# Abstract

Tuning compiler heuristics and parameters is well known to improve optimization outcomes dramatically. Prior works have tuned command line flags and a few expert identified heuristics. However, there are an unknown number of heuristics buried, unmarked and unexposed inside the compiler as a consequence of decades of development without auto-tuning being foremost in the minds of developers. Many may not even have been considered heuristics by the developers who wrote them. The result is that auto-tuning search and machine learning can optimize only a tiny fraction of what could be possible if all heuristics were available to tune. Manually discovering all of these heuristics hidden among millions of lines of code and exposing them to auto-tuning tools is a Herculean task that is simply not practical. What is needed is a method of automatically finding these heuristics to extract every last drop of potential optimization. In this work, we propose Heureka, a framework that automat ically identifies potential heuristics in the compiler that are highly profitable optimization targets and then automatically finds available tuning parameters for those heuristics with minimal human involvement. Our work is based on the following key insight: When modifying the output of a heuristic within an acceptable value range, the calling code using that output will still function correctly and produce semantically correct results. Building on that, we automatically manipulate the output of potential heuristic code in the compiler and decide using a Differential Testing approach if we found a heuristic or not. During output manipulation, we also explore acceptable value ranges of the targeted code. Heuristics identified in this way can then be tuned to optimize an objective function. We used Heureka to search for heuristics among eight thou sand functions from the LLVM optimization passes, which is about 2% of all available functions. We then use identified heuristics to tune the compilation of 38 applications from the NAS and Polybench benchmark suites. Compared to an -Oz baseline we reduce binary sizes by up to 11.6% considering single heuristics only and up to 19.5% when stacking the effects of multiple identified tuning targets and applying a random search with minimal search effort. Generalizing from existing analysis results, Heureka needs, on average, a little under an hour on a single machine to identify relevant heuristic targets for a previously unseen application.

# Resources

[![Paper Preprint]({{ site.url }}{{ site.baseurl }}/images/icon-pdf.png)]({{ site.url }}{{ site.baseurl }}/files/papers/cgo24_heureka_preprint.pdf)
