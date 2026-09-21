# Hi, I'm Yuchen He

M.S.E. Electrical Engineering student at the University of Pennsylvania (2026-2028). I build
hardware-aware systems software: multi-GPU LLM serving, failure-tolerant gateways, reproducible
performance evaluation, and performance-oriented C++. I am also developing embedded/SoC depth
through register-level firmware, FPGA architecture, and digital-design work.

## Projects

| Project | What it is |
| --- | --- |
| [radixgates](https://github.com/YuchenHe985/radixgates) | Go reference gateway for multi-GPU LLM serving on SGLang: prefix-affinity routing, health-aware failover, circuit breaking, bounded admission, failure injection, and tests against real llama.cpp workers; includes my 4x RTX 4090 / 4x A100 evaluation. |
| [llm-serving-eval-kit](https://github.com/YuchenHe985/llm-serving-eval-kit) | Standard-library Python toolkit for memory/GPU-count sizing, startup-failure diagnosis, reproducible benchmark matrices, and comparison reports that surface confounded setups instead of over-claiming them. |
| [llm-finetune-lab](https://github.com/YuchenHe985/llm-finetune-lab) | On-device text-to-SQL feasibility study: LoRA with PyTorch DDP, execution-based evaluation, quantized llama.cpp deployment, and an evidence-based recommendation to keep a person in the loop. |
| [cdc-chunker](https://github.com/YuchenHe985/cdc-chunker) | C++17 Gear and Rabin content-defined chunking library: about 2 GB/s sequential and 7.4 GB/s with 8 threads on an Apple M1, bit-identical parallel output, 31 tests, independent-reference checks, sanitizers, and a 23/23 mutation check. |

## Background

- Mentor-guided industry project on private LLM serving: evaluated SGLang on 4x RTX 4090 (PCIe) and 4x A100 (NVLink) in data, tensor and expert parallel modes and diagnosed CUDA, NCCL and memory failures.
- Built PySpark / Hive batch pipelines and data-quality checks for a logistics forecasting platform.
- Coursework this term: SoC architecture (FPGA), digital IC / VLSI (SRAM-based MAC accelerator), embedded systems.

**Languages:** Python, Go, C/C++, SQL &nbsp;|&nbsp; **Contact:** heyuchen@seas.upenn.edu
