# Hi, I'm Yuchen He

M.S.E. Electrical Engineering student at the University of Pennsylvania (2026-2028). I work on
AI infrastructure and GPU systems: serving LLMs on multi-GPU machines, making that serving
reliable, and measuring it in a way you can trust, plus performance-oriented C++.

## Projects

| Project | What it is |
| --- | --- |
| [radixgates](https://github.com/YuchenHe985/radixgates) | Go gateway for multi-GPU LLM serving on SGLang, upgraded with prefix-affinity routing, health-aware failover, circuit breaking, admission control and a failure-injection benchmark against the original; includes my 4x RTX 4090 / 4x A100 evaluation. |
| [llm-serving-eval-kit](https://github.com/YuchenHe985/llm-serving-eval-kit) | Python toolkit for GPU procurement studies: memory / GPU-count sizing, startup-failure diagnosis, benchmark matrices with confidence intervals, and comparisons that flag confounded setups. |
| [cdc-chunker](https://github.com/YuchenHe985/cdc-chunker) | C++17 content-defined chunking library (Gear and Rabin) for deduplicating storage of large files: about 2 GB/s per core and 7.4 GB/s on 8 threads with output identical to the sequential chunker; checked against an independent reference implementation and a 23-bug injected-fault check. |

## Background

- Mentor-guided industry project on private LLM serving: evaluated SGLang on 4x RTX 4090 (PCIe) and 4x A100 (NVLink) in data, tensor and expert parallel modes and diagnosed CUDA, NCCL and memory failures.
- Built PySpark / Hive batch pipelines and data-quality checks for a logistics forecasting platform.
- Coursework this term: SoC architecture (FPGA), digital IC / VLSI (SRAM-based MAC accelerator), embedded systems.

**Languages:** Python, Go, C/C++, SQL &nbsp;|&nbsp; **Contact:** heyuchen@seas.upenn.edu
