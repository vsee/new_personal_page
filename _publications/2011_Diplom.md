---
title: "Design and Implementation of an Efficient Instruction Set Simulator for an Embedded Multi-Core Architecture"
collection: publications
permalink: /publication/2011_diplom
excerpt: 'This thesis develops the concepts required for efficient multi-core just-in-time dynamic binary translation and demonstrates its feasibility and high simulation performance through an implementation in the ARCSIM simulator platform.'
date: 2011-05-01
citation: 'Volker Seeker. Design and Implementation of an Efficient Instruction Set Simulator for an Embedded Multi-Core Architecture. Diploma Thesis. Programmierung Eingebetteter Systeme, Technische Universit&auml;t Berlin, 2011.'
---

# Abstract

In recent years multi-core processors have become ubiquitous in many domains ranging from embedded systems through general-purpose computing to large-scale data centers. The design of future parallel computers requires fast and observable simulation of target architectures running realistic workloads. Aiming for this goal, a large number of parallel instruction set simulators (I SS) for parallel systems have been developed. With different simulation strategies all those approaches try to bridge the gap between detailed architectural observability and performance. However, up until now state-of-the-art simulation technology was not capable to provide the simulation speed required to efficiently support design space exploration and parallel software development. This thesis develops the concepts required for efficient multi-core just-in-time (JIT) dynamic binary translation (DBT) and demonstrates its feasibility and high simulation performance through an implementation in the ARCSIM simulator platform. ARCSIM is capable of simulating large-scale multi-core configurations with hundreds or even thousands of cores. It does not rely on prior profiling, instrumentation or compilation and works for all multi-threaded binaries implementing the PTHREAD interface and targeting a state-of-the-art embedded multi-core platform implementing the ARCOMPACT instruction set architecture (ISA). The simulator has been evaluated against two standard benchmark suites, EEMBC MULTIBENCH and SPLASH-2, and is able to achieve speed ups up to 25,307 million instructions per second (MIPS) on a 32-core x86 host machine for as many as 2048 simulated cores while maintaining near-optimal scalability. The results demonstrate that ARCSIM is even able to outperform an FPGA architecture used as a physical reference system on a per core basis.

# Supervision

* [Prof. Dr. Sabine Glesner](http://www.tu-berlin.de/?id=glesner)
* [Dr. Bj&ouml;rn Franke](https://blog.inf.ed.ac.uk/bfranke/)
* Dirk Tetzlaff

This work was partially funded by the Network of Excellence on Embedded Systems Design [ArtistDesign](http://www.artist-embedded.org/artist/-Home-Page-.html).

# Resources

[![Thesis]({{ site.url }}{{ site.baseurl }}/images/icon-pdf.png)]({{ site.url }}{{ site.baseurl }}/files/papers/2011_thesis.pdf)
**Thesis**
