I make AI compute fast, efficient, and reliable, from the serving layer down to the hardware and the power behind it.

Senior Software Engineer on an inference data plane at an AI company (New York); previously AWS, on payments and IoT. Rust, C++, and distributed systems.

**Open to:** advising AI-infrastructure and payments startups, technical diligence for investors, and early conversations with founders. [ryan.j.hamby@gmail.com](mailto:ryan.j.hamby@gmail.com)

## Projects

- **[GPU Flight Recorder](https://github.com/RyanJHamby/distributed-gpu-training-flight-recorder)**: finds the straggling rank in distributed GPU training and explains why it is slow, by joining PyTorch NCCL collective timings with per-GPU NVML telemetry (Go, gRPC). Validated in simulation; real-GPU run next.
- **[FlowState](https://github.com/RyanJHamby/FlowState)**: Rust as-of join engine with zero-copy Arrow, Rayon-parallel merge scans, and streaming watermark joins.
- **[Order Book Engine](https://github.com/RyanJHamby/order-book-engine)**: C++20 matching engine; P50 0.21 µs, P99.9 3.1–3.2 µs on EC2 `c6i.large`, lock-free SPSC ingestion, slab memory pools.
- **[autopilot-kit](https://github.com/RyanJHamby/autopilot-kit)**: guardrails for coding agents working across my repos: reusable GitHub Actions workflows and stdlib scripts (guard, gate, handshake, automerge) that repos pin by commit SHA, with no tokens or network access in the scripts.

## Open Source Contributions

- **[vllm-project/vllm#48420](https://github.com/vllm-project/vllm/pull/48420)** (merged): fixed a `StopIteration` crash in Qwen3-Omni multimodal processing when a video has no audio track but `use_audio_in_video=True` is requested, plus two follow-on false-positive paths in processor caching ([write-up](https://ryanjhamby.substack.com/p/the-fix-for-a-qwen3-omni-crash-broke))
- **[firecracker-microvm/firecracker#6032](https://github.com/firecracker-microvm/firecracker/pull/6032)** (merged): fixed a VMM panic on ACPI device restore when `EventFd` creation fails
- **[firecracker-microvm/firecracker#6033](https://github.com/firecracker-microvm/firecracker/pull/6033)** (merged, docs): documented a DNS lookup delay caused by an IPv6 resolver stall

## Writing

I write up measured results, including the dead ends, on [Substack](https://ryanjhamby.substack.com) ([subscribe](https://ryanjhamby.substack.com/subscribe)).

- **[The fix for a Qwen3-Omni crash broke CI two ways](https://ryanjhamby.substack.com/p/the-fix-for-a-qwen3-omni-crash-broke)**: my first vLLM fix, the review that replaced it, and the two CI failures that followed
- **[Why I paused the site-control checker I built for PJM's interconnection queue](https://ryanjhamby.substack.com/p/why-i-paused-the-site-control-checker)**: the Zonevex postmortem, with the outreach result and what I would build instead

## Also built

- **[Macro Trading System](https://github.com/RyanJHamby/macro-factor-decomposition)**: PCA regime classification and Kelly sizing over FRED data (backtest being rerun with lagged signals)
- **[Equity Signal Engine](https://github.com/RyanJHamby/stock-screener)**: daily 3,800+ stock scanner, automated with GitHub Actions
