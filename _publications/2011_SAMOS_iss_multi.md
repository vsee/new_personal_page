---
title: "Scalable Multi-Core Simulation Using Parallel Dynamic Binary Translation"
collection: publications
permalink: /publication/2011_SAMOS_iss_multi
excerpt: 'In this paper we develop a fast and scalable simulation methodology for multi-core platforms based on parallel and just-in-time dynamic binary translation.'
date: 2011-07-01
venue: 'IC-SAMOS'
citation: 'Oscar Almer, Igor Bo&#776;hm, Tobias J.K. Edler von Koch, 
Bjo&#776;rn Franke, Stephen Kyle, Volker Seeker, Christopher 
Thompson, and Nigel Topham. &quot;Scalable Multi-Core
Simulation Using Parallel Dynamic Binary Translation.&quot; Proceedings
of the 11th International Conference on Embedded Computer Systems:
Architectures, Modelling, and Simulation, Samos, Greece, July 2011.'
---

# Abstract

In recent years multi-core processors have seen broad adoption in application domains ranging from embedded systems through general-purpose computing to large-scale data centres. Simulation technology for multi-core systems, however, lags behind and does not provide the simulation speed required to effectively support design space exploration and parallel software development. While state-of-the-art instruction set simulators (ISS) for single-core machines reach or exceed the performance levels of speed-optimised silicon implementations of embedded processors, the same does not hold for multi-core simulators where large performance penalties are to be paid. In this paper we develop a fast and scalable simulation methodology for multi-core platforms based on parallel and just-in-time (JIT) dynamic binary translation (DBT). Our approach can model large-scale multi-core configurations, does not rely on prior profiling, instrumentation, or compilation, and works for all binaries targeting a state-of-the-art embedded multi-core platform implementing the ARCompact instruction set architecture (ISA). We have evaluated our parallel simulation methodology against the industry standard SPLASH-2 and EEMBC MULTIBENCH benchmarks and demonstrate simulation speeds up to 25,307 MIPS on a 32-core x86 host machine for as many as 2048 target processors whilst exhibiting minimal and near constant overhead.

# Resources

[![Paper]({{ site.url }}{{ site.baseurl }}/images/icon-pdf.png)]({{ site.url }}{{ site.baseurl }}/files/papers/2011_SAMOS_iss_multi.pdf)
**Paper**
