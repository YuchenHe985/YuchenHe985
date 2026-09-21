<div align="center">

# Yuchen He

**GPU / AI Systems · Systems Performance · Embedded / SoC**

M.S.E. Electrical Engineering @ University of Pennsylvania (2026–2028)

Building hardware-aware software from real measurements: multi-GPU inference, reliable serving, performance-oriented C++, and register-level systems.

`Python` · `Go` · `C/C++` · `CUDA/NCCL` · `Linux`

**Open to Summer 2027 internships in GPU/AI systems, embedded software, and hardware-aware performance engineering.**

</div>

## Selected systems work

| Project | Engineering focus | Evidence |
| --- | --- | --- |
| **[RadixGates](https://github.com/YuchenHe985/radixgates)** | Failure-tolerant Go gateway for multi-GPU LLM serving: prefix affinity, health-aware failover, circuit breaking, admission control, and OpenAI-compatible routing | **85.2% → 99.7%** clean completions during node-crash tests; **53 tests** under `go test -race`; real evaluation on **4× RTX 4090 and 4× A100** |
| **[llm-serving-eval-kit](https://github.com/YuchenHe985/llm-serving-eval-kit)** | GPU-memory sizing, topology interpretation, startup-log diagnosis, repeated benchmark matrices, and confounder-aware comparison | **11 failure signatures**, bootstrap intervals, cost/SLO reporting, and **39 unit/end-to-end tests** |
| **[cdc-chunker](https://github.com/YuchenHe985/cdc-chunker)** | C++17 Gear/Rabin content-defined chunking with streaming and bit-identical parallel output | About **2.0 GB/s** sequential and **7.4 GB/s** with 8 threads on Apple M1; **31 tests** plus **23/23 mutation checks** |
| **[llm-finetune-lab](https://github.com/YuchenHe985/llm-finetune-lab)** | Local text-to-SQL feasibility study: LoRA/DDP, execution-based evaluation, GGUF deployment, and guardrail analysis | **398 MB** Q4 model, **82.6%** execution accuracy, **1.76×** two-GPU training speedup; evidence-based human-in-the-loop release decision |

## What connects the projects

- **Measure before optimizing:** record topology, software versions, failure modes, repetitions, and uncertainty before attributing a result.
- **Design for failure:** make overload, node loss, partial streams, and invalid model output explicit instead of hiding them behind averages.
- **Follow the hardware:** connect routing, cache locality, communication topology, memory limits, and parallelism choices to observed behavior.

## Current direction

I am extending this systems work toward embedded and accelerator design through register-level firmware, FPGA/SoC architecture, and digital IC/VLSI coursework. My earlier engineering experience includes PySpark/Hive pipelines and data-quality checks for a regional logistics forecasting platform.

**Contact:** [heyuchen@seas.upenn.edu](mailto:heyuchen@seas.upenn.edu)
