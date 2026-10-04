I make AI compute fast, efficient, and reliable, from the serving layer down to the hardware and the power behind it.

Software engineer at AWS (New York). Rust, C++, and distributed systems.

## Projects

- **[GPU Flight Recorder](https://github.com/RyanJHamby/distributed-gpu-training-flight-recorder)**: finds the straggling rank in distributed GPU training and explains why it is slow, by joining PyTorch NCCL collective timings with per-GPU NVML telemetry (Go, gRPC). Validated in simulation; real-GPU run next.
- **[FlowState](https://github.com/RyanJHamby/FlowState)**: Rust as-of join engine with zero-copy Arrow, Rayon-parallel merge scans, and streaming watermark joins.
- **[Order Book Engine](https://github.com/RyanJHamby/order-book-engine)**: C++20 matching engine; P50 0.21 µs, P99.9 3.1–3.2 µs on EC2 `c6i.large`, lock-free SPSC ingestion, slab memory pools.

## Open Source Contributions

- **[vllm-project/vllm#48420](https://github.com/vllm-project/vllm/pull/48420)** (merged): fixed a `StopIteration` crash in Qwen3-Omni multimodal processing when a video has no audio track but `use_audio_in_video=True` is requested, plus two follow-on false-positive paths in processor caching
- **[firecracker-microvm/firecracker#6032](https://github.com/firecracker-microvm/firecracker/pull/6032)** (merged): fixed a VMM panic on ACPI device restore when `EventFd` creation fails
- **[firecracker-microvm/firecracker#6033](https://github.com/firecracker-microvm/firecracker/pull/6033)** (merged, docs): documented a DNS lookup delay caused by an IPv6 resolver stall

## Also built

- **[Macro Trading System](https://github.com/RyanJHamby/macro-factor-decomposition)**: PCA regime classification, Kelly sizing, VaR monitoring over an 18-year FRED backtest
- **[Equity Signal Engine](https://github.com/RyanJHamby/stock-screener)**: daily 3,800+ stock scanner, automated with GitHub Actions
