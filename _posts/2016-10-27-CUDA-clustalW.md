---
layout: post
title: CUDA-clustalW
description: >
    A sequence alignment tool
modified: 2016-10-27
category: [High Performance Computing]
tags: [projects, GPGPU, CUDA, bioinformatics]
---

  In computational biology, sequence alignment is of priority concern and many methods have been developed to solve sequence alignment-related problems for biological applicatons.
ClustalW is a progressive multiple sequence alignment tool to align a set of sequences by repeatedly aligning pairs of sequences and previously generated alignments. Several algorithms or tools 
have been ported on GPUs with CUDA in computational biology, such as MUMmerGPU, CUDA-MEME, CUDA-BLASTP, and etc. Liu et al. proposed a tool MSA-CUDA to parallelize all three stages 
of ClustalW v2.0.9 processing pipeline by using inter-task parallelization. CUDA ClustalW v1.0 is a GPU version of ClustalW v2.0.11 which is implemented by using intra-task parallelization and 
Synchronous Diagonal Multiple Threads type. Several optimization methods were designed to improve the performance of CUDA ClustalW v1.0. From the experimental results, the CUDA ClustalW 
v1.0 can achieve about 22x speedups for 1000 sequences with length of 1532 in the distance matrix calculation step by comparing to ClustalW v2.0.11 on single-GPU. For the overall execution time, 
the CUDA ClustalW v1.0 can achieve about 33x speedups by comparing to ClustalW v2.0.11 on two-GPUs.


## Version 1.0.0 (March 2013) 

* Linux x86 64-bit
* CPU/GPU coprocess
* Support Multiple GPUs
* NVIDIA CUDA support
* Base on clustalW 2.0


		

### Papers
 * Journal
   * Che-Lun Hung, `Yu-Shiang Lin`, Chun-Yuan Lin, Yeh-Ching Chung, Yi-Fang Chung, “CUDA ClustalW: An efficient parallel algorithm for progressive multiple sequence alignment on Multi-GPUs”, CBAC: 58-62 (2015).




[GitHub link](https://github.com/coldfunction/CUDA-clustalW)