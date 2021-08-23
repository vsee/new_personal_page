---
title: "Device-Hopping: Transparent Mid-Kernel Runtime Switching for Heterogeneous Systems"
collection: publications
permalink: /publication/2021_TACO_device_hopping
excerpt: 'This paper presents a study to make CPU + GPU systems more flexible with respect to switching between cores in the middle of kernel execution.'
date: 2021-08-23
venue: 'TACO'
citation: 'Metzger, P, Seeker, V, Fensch, C & Cole, M 2021, Device-Hopping: Transparent Mid-Kernel Runtime Switching for Heterogeneous Systems, ACM Transactions on Architecture and Code Optimization.'
---

# Abstract

Existing OS techniques for homogeneous many-core systems make it simple for single and multithreaded
applications to migrate between cores. Heterogeneous systems do not benefit so fully from this flexibility, and applications that cannot migrate in mid-execution may lose potential performance. The situation is particularly challenging when a switch of language runtime would be desirable in conjunction with a migration. We present a case study in making heterogeneous CPU + GPU systems more flexible in this respect. Our technique for fine-grained application migration, allows switches between OpenMP, OpenCL, and CUDA execution, in conjunction with migrations from GPU to CPU, and CPU to GPU. To achieve this, we subdivide iteration spaces into slices, and consider migration on a slice-by-slice basis. We show that slice sizes can be learned offline by machine learning models. To further improve performance, memory transfers are made migration-aware. The complexity of the migration capability is hidden from programmers behind a high-level programming model. We present a detailed evaluation of our mid-kernel migration mechanism with the First Come, First Served scheduling policy. We compare our technique in a focused evaluation scenario against idealized kernel-by-kernel scheduling, which is typical for current systems, and makes perfect kernel to device scheduling decisions, but cannot migrate kernels mid-execution. Models show that up to 1.33× speedup can be achieved over these systems by adding fine-grained migration. Our experimental results with all nine applicable SHOC and Rodinia benchmarks achieve speedups of up to 1.30× (1.08× on average) over an implementation of a perfect but kernel-migration incapable scheduler when migrated to a faster device. Our mechanism and slice size choices introduce an average slowdown of only 2.44% if kernels never migrate. Lastly, our programming model reduces the code size by at least 88% if compared to manual implementations
of migratable kernels.

# Resources

[Paper](https://www.research.ed.ac.uk/en/publications/device-hopping-transparent-mid-kernel-runtime-switching-for-heter)
