<div align="center">

# Yuchen He

**GPU / AI Systems · Systems Performance · Embedded / SoC**

M.S.E. Electrical Engineering @ University of Pennsylvania (2026–2028)

Building hardware-aware software from real measurements: multi-GPU inference, reliable serving, performance-oriented C++, and register-level systems.

`Python` · `Go` · `C/C++` · `CUDA/NCCL` · `Linux`

**Open to Summer 2027 internships in GPU/AI systems, embedded software, and hardware-aware performance engineering.**

[yuchenhe985.github.io](https://yuchenhe985.github.io) · [LinkedIn](https://www.linkedin.com/in/yuchenhe-) · [yuchenhe.work@outlook.com](mailto:yuchenhe.work@outlook.com)

</div>

## Selected systems work

| Project | Engineering focus | Evidence |
| --- | --- | --- |
| **[RadixGates](https://github.com/YuchenHe985/radixgates)** | Failure-tolerant Go gateway for multi-GPU LLM serving: prefix affinity, health-aware failover, circuit breaking, admission control, and OpenAI-compatible routing | **85.2% → 99.7%** clean completions during node-crash tests; **55 tests** under `go test -race`; real evaluation on **4× RTX 4090 and 4× A100** |
| **[llm-serving-eval-kit](https://github.com/YuchenHe985/llm-serving-eval-kit)** | GPU-memory sizing, topology interpretation, startup-log diagnosis, repeated benchmark matrices, and confounder-aware comparison | **11 failure signatures**, bootstrap intervals, cost/SLO reporting, and **39 unit/end-to-end tests** |
| **[cdc-chunker](https://github.com/YuchenHe985/cdc-chunker)** | C++17 Gear/Rabin content-defined chunking with streaming and bit-identical parallel output | About **2.0 GB/s** sequential and **7.4 GB/s** with 8 threads on Apple M1; **31 tests** plus **23/23 mutation checks** |
| **[llm-finetune-lab](https://github.com/YuchenHe985/llm-finetune-lab)** | Local text-to-SQL feasibility study: LoRA/DDP, execution-based evaluation, GGUF deployment, and guardrail analysis | **398 MB** Q4 model, **82.6%** execution accuracy, **1.76×** two-GPU training speedup; evidence-based human-in-the-loop release decision |

## Software and data engineering

| Project | Engineering focus | Evidence |
| --- | --- | --- |
| **[conference-ops](https://github.com/YuchenHe985/conference-ops)** | Spring Boot 3 + PostgreSQL 16 backend: row-locked seat allocation with a FIFO waitlist, exclusion constraints against double-booking, idempotent retries, optimistic locking, Flyway | **60** concurrent requests for **10** seats never oversell (the test fails when the lock is removed); **25** integration tests on real PostgreSQL |
| **[review-pipeline](https://github.com/YuchenHe985/review-pipeline)** | Python/DuckDB/Parquet pipeline: data contracts with quarantine, content-addressed idempotent stages, point-in-time features, leakage-safe evaluation | **494K** real reviews in about 45 s; a random split would overstate R² **4.6×**; top-decile helpful rate **2.13×** the base rate |

## Field notes

Four short notes on what a measurement taught me, on [my site](https://yuchenhe985.github.io/notes/):

- [A simulation can't see a cache](https://yuchenhe985.github.io/notes/simulation-cannot-see-a-cache/): my gateway's failure tests all passed, and a routing rule I had added still cut prefix-cache hits from 59.1% to 24.4% on real engines.
- [The wrong answers that raise no error](https://yuchenhe985.github.io/notes/wrong-answers-that-raise-no-error/): the 16.4% of a fine-tuned model's SQL that runs cleanly and returns the wrong rows.
- [Same weights, different dtype](https://yuchenhe985.github.io/notes/same-weights-different-dtype/): only 27.6% of a fine-tuned model's bytes match its base, and the encoding mattered more than the chunker.
- [Average chunk size isn't what an edit costs](https://yuchenhe985.github.io/notes/average-chunk-size-is-not-the-cost/): an edit is more likely to land in a big chunk, so the spread of chunk sizes matters as much as the average.

## What connects the projects

- **Measure before optimizing:** record topology, software versions, failure modes, repetitions, and uncertainty before attributing a result.
- **Design for failure:** make overload, node loss, partial streams, and invalid model output explicit instead of hiding them behind averages.
- **Follow the hardware:** connect routing, cache locality, communication topology, memory limits, and parallelism choices to observed behavior.

## Current direction

I am extending this systems work toward embedded and accelerator design through register-level firmware, FPGA/SoC architecture, and digital IC/VLSI coursework. My earlier engineering experience includes PySpark/Hive pipelines and data-quality checks for a regional logistics forecasting platform.
