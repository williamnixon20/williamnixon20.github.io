---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

[Download the PDF version]({{ base_path }}/files/William_CV.pdf)

Computer Science Ph.D. student at the University of Chicago researching efficient systems for
caching, storage, memory management, and LLM serving.

Education
======
* Ph.D. in Computer Science, University of Chicago, Sep 2025 – Present
  * GPA: 4.00
  * Advisors: Prof. Haryadi S. Gunawi and Prof. Juncheng Yang (Harvard)
* B.S. in Computer Science, Bandung Institute of Technology, Jul 2021 – Jul 2025
  * GPA: 3.95

Publications
======
* Haocheng Xia, **William Nixon**, Bintang Dwi Marthen, Pranav Bhandari, Juncheng Yang.
  "Learning-Augmented Heuristics: Simple yet Smart, Robust and Interpretable Cache Eviction."
  *USENIX Symposium on Operating Systems Design and Implementation (OSDI)*, 2026.
* Ray A. O. Sinurat, **William Nixon**, Philip Carns, ... Haryadi S. Gunawi, Hariharan Devarajan.
  "GLANCED-IO: Taming I/O Optimization for Deep Learning at Scale."
  *ACM International Symposium on High-Performance Parallel and Distributed Computing (HPDC)*, 2026.
* Ray A. O. Sinurat, **William Nixon**, Haryadi S. Gunawi, Nikoli Dryden, Hariharan Devarajan.
  "HORATIO: Bridging Management and Analysis of Traces at Scale."
  *International Conference on Scientific and Statistical Database Management (SSDBM)*, 2026.
* Samuel Cahyawijaya, Holy Lovenia, Joel Ruben Antony Moniz, ... **William Nixon**, ... Peerat Limkonchotiwat.
  "Crowdsource, Crawl, or Generate? Creating SEA-VL, a Multicultural Vision-Language Dataset for Southeast Asia."
  *Annual Meeting of the Association for Computational Linguistics (ACL)*, 2025.
* Holy Lovenia, Rahmad Mahendra, Salsabil Maulana Akbar, ... **William Nixon**, ... Samuel Cahyawijaya.
  "SEACrowd: A Multilingual Multimodal Data Hub and Benchmark Suite for Southeast Asian Languages."
  *Conference on Empirical Methods in Natural Language Processing (EMNLP)*, 2024.

Preprints
======
* **William Nixon**, Muxin Tian, Yunjia Zheng, Haryadi S. Gunawi, Juncheng Yang.
  "From Requests to Sessions: A Large-Scale Characterization of Human-Driven Agentic Workloads."
  In submission, 2026.
* **William Nixon**, Jon Durbin, Florian Standhartinger, Haryadi S. Gunawi, Juncheng Yang.
  "A Year in LLM Serving: Workload Evolution, Caching and Load-Balancing."
  In submission, 2026. [arXiv](https://arxiv.org/abs/2608.13573)
* Hongshu Yan, Yunjia Zheng, **William Nixon**, Yazhuo Zhang, Pranav Bhandari, Haryadi S. Gunawi, Ana Klimovic, Juncheng Yang.
  "Demystifying and Optimizing Slab Rebalance in Memory Caches."
  In submission, 2026.

Research experience
======
* **Caching and Memory Management**, Sep 2025 – Present
  * *Learning-Augmented Heuristics, LAH (OSDI'26)*: uses ML to make simple cache heuristics adaptive by
    automatically tuning their parameters, outperforming more complex ML-based cache policies with
    negligible runtime overhead; improves cache efficiency by 26% over S3-FIFO and 8% over prior state of the art.
  * *Adaptive Slab Rebalancing (preprint)*: improves memory allocation in slab-based caches by stabilizing
    noisy rebalance signals and preventing unnecessary slab movements; production deployment reduces DRAM
    misses by 20% and CPU utilization by up to 5%.
  * Implemented S4-FIFO and Adaptive-Marginal-Hits in C++/CacheLib and worked with Meta engineers to deploy
    and evaluate them in production.

* **LLM Serving and Agentic Workloads**, Jul 2026 – Present
  * *Agentic Workload Analysis (preprint)*: analyzes 1.2M production requests, 205B input tokens, and 12K
    coding-agent sessions across 13 agent frameworks; characterizes tool execution, context growth, and
    KV-cache reuse, and releases the largest production agentic trace with tool- and block-level information to date.
  * *A Year in LLM Serving (preprint)*: analyzes and releases a year-long production trace of 6.1B LLM requests
    across 9K+ models, the largest public LLM serving dataset to date, enabling large-scale studies of workload
    evolution, prefix caching, and request routing.
  * Led both projects: built the analysis pipeline for TBs of production requests and the event-driven simulator
    for cache eviction and request routing, and maintain the open-source trace and benchmark repositories.

* **Deep Learning I/O and Trace Analysis**, Mar 2025 – Jul 2026
  * *GLANCED-IO (HPDC'26)*: optimizes I/O bottlenecks in large-scale weather-forecasting workloads by tuning I/O
    and data configurations through GPU-free proxy applications, improving training performance by up to 1.57x
    while avoiding expensive GPU runs during tuning. In collaboration with Lawrence Livermore National Laboratory (LLNL).
  * *HORATIO (SSDBM'26)*: develops an out-of-place index for gzip-compressed JSONL traces emitted by scientific
    applications, enabling fast queries directly over compressed data without format conversion and with minimal
    additional storage; up to 83x faster analysis. In collaboration with LLNL.

Open-source contributions
======
* **Google Summer of Code (GSoC)**, Open Source Research Experience (OSRE), UC Santa Cruz OSPO, Sep 2023 – Mar 2025
  * Built an extensible benchmark for concept drift in ML-for-systems workloads, comparing three online adaptation
    algorithms against retraining across four datasets with mentors from Argonne National Laboratory.
  * Integrated Matchmaker, DriftSurf, and AUE into ML-based caching and storage systems, including GL-Cache and
    LinnOS, reducing cache misses by up to 5%.
  * Released open-source implementations, experiment results, and a reproducible Chameleon Cloud artifact.

* **SEACrowd**, Contributor and Community Reviewer, Jul 2023 – Sep 2024
  * Implemented Hugging Face dataset loaders for under-resourced Southeast Asian languages as part of the
    SEACrowd open-data and benchmark ecosystem published at EMNLP'24.
  * Reviewed 50+ community contributions for loader correctness, dataset metadata, and interface compatibility.

Industry experience
======
* **Backend Developer**, Bukit Vista Hospitality Services, Mar 2022 – Dec 2022
  * Built the backend for an in-house multi-property availability calendar, contributing to API design, database
    modeling, implementation, and deployment on AWS.
  * Automated finance and HR workflows previously handled manually, reducing processing time by up to 90%.
  * Technologies: Node.js, Python, AWS.

Teaching
======
* CMSC 23000: Operating Systems, University of Chicago — Aut 2025, 2026
* CMSC 33200: Topics in Operating Systems, University of Chicago — Spr 2026
* CMSC 14400: Systems Programming II, University of Chicago — Win 2026

Skills
======
* **Languages**: C, C++, Python, Go, Java, JavaScript, SQL, Bash/Shell
* **ML & parallel computing**: PyTorch, TensorFlow, CUDA, MPI, OpenMP, SLURM
* **Systems & data**: CacheLib, Redis, Apache Spark, Pandas, PyArrow/Parquet, RabbitMQ, PostgreSQL
* **Infrastructure & cloud**: Linux, Git, Docker, Kubernetes, AWS, Google Cloud, Chameleon Cloud
