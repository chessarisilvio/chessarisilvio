<p align="center">
  <h1 align="center">Silvio Chessari</h1>
  <h3 align="center">⚡ AI Infrastructure • LLM Research • Embedded Systems 🤖</h3>
</p>

Specializes in maximizing LLM inference efficiency on heterogeneous hardware (Tesla P40/RTX) through speculative decoding and CUDA workarounds. Researches MoE routing, EAGLE/MTP techniques, and self-hosted AI stacks. Develops embedded interfaces (ESP32/Arduino) and automation pipelines bridging physical hardware with generative models.

| **Domain** | **Stack & Tools** |
| :--- | :--- |
| **LLM Inference** | llama.cpp, GGUF, EXL2, Speculative Decoding, Qwen3.5 MoE |
| **Systems** | CUDA, Docker, Bash, Python (FastAPI/Flask), Node.js |
| **Hardware** | NVIDIA Tesla P40 (sm_61), RTX 3050, Arduino R4, ESP32 |
| **Ops** | Systemd, Tailscale, MQTT, Nginx, GitHub Actions |

---

### LLM Research & Inference

[Nex2 Mini Phase Twin 30B](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model) — Low-VRAM GGUF model optimization designed for high-performance inference on constrained consumer GPUs.

[Automated EXL2 Conversion Pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) — C++/Python toolchain implementing Qwen3_5 MoE architecture fixes, mixed-precision quantization, and validation benchmarking.

[Benchmark 4 Agent Wrappers on Qwen3.6](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp) — Comparative latency and VRAM analysis of agent wrappers (Pi, OpenCode, Hermes) running on llama.cpp.

---

### AI Infrastructure

[Automated GGUF Benchmarking System](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-mo) — Automated evaluation pipeline generating performance reports for models running on Tesla P40 and RTX 3050.

[OpenClaw Gateway](https://github.com/chessarisilvio/openclaw) — Node.js-based Ollama gateway integrating MQTT/Tailscale for secure remote access to local LLM services.

[AI Dashboard](https://github.com/chessarisilvio/ai-dashboard) — Web-based monitoring solution tracking GPU VRAM, token-per-second throughput, service health, and active sprint agendas.

---