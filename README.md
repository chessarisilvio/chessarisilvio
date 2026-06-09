<div align="center">

# 👋 Silvio Chessari – AI Systems Engineer & LLM Researcher

**Deep‑learning inference specialist** – LLM scaling, speculative decoding, MoE routing, EAGLE.  
**GPU architect** – Running 35 B‑parameter models on Pascal (Tesla P40, sm_61) via custom CUDA shims and low‑level memory tricks.  
**Embedded & AI infra builder** – From ESP32 thermal controllers to self‑hosted AI stacks on consumer & datacenter hardware.

</div>

---  

## Tech Stack  

| Category | Tools / Frameworks |
|----------|-------------------|
| **Languages** | Python 3.12, C++, Rust, Bash, TypeScript |
| **LLM Engines** | llama.cpp, llama‑server, fast‑transformers, speculative decoding, MoE routing, EAGLE |
| **GPU / CUDA** | NVIDIA Pascal (sm_61), RTX 3050, CUDA 12.x, custom `sm_61` compatibility shim |
| **Inference Optimizations** | MTP, speculative decoding, quantized GGUF, tensor parallelism, kernel fusion |
| **Web / API** | Flask, FastAPI, Node.js, OpenAPI, Prometheus, Plotly |
| **DevOps** | systemd, Docker, GitHub Actions, Terraform (infra‑as‑code) |
| **Embedded** | ESP32‑WROOM‑32, DS18B20, MOSFET PWM, USB‑HID, FreeRTOS |
| **Data / RAG** | ChromaDB, PDF/DOCX/XLSX ingest, Markitdown CLI |
| **Automation** | Aider, FreeLLM API, custom Telegram bots, CI pipelines |

---  

## LLM Research  

| Project | Description |
|---------|-------------|
| [LLM Research](https://github.com/chessarisilvio/llm-research) | Implements llama‑MTP, EAGLE speculative decoding, and dynamic MoE routing; benchmarks token‑per‑second across Pascal and RTX 3050 GPUs. |
| [Speculative Decoding Suite](https://github.com/chessarisilvio/speculative-decoding-suite) | Python/C++ toolkit for on‑the‑fly speculative token prediction, reducing TTFT by up to 42 % on sm_61 hardware. |
| [MoE Router Engine](https://github.com/chessarisilvio/moe-router-engine) | Custom TensorRT‑compatible router enabling 8‑expert MoE models on 12 GB VRAM GPUs with load‑aware scheduling. |
| [EAGLE Inference Framework](https://github.com/chessarisilvio/eagle-framework) | End‑to‑end pipeline integrating early‑exit, adaptive‑gating, and layer‑wise quantization for 35 B models. |

---  

## AI Infrastructure  

| Project | Description |
|---------|-------------|
| [AI Telemetry](https://github.com/chessarisilvio/ai-telemetry) | Flask dashboard (`:9191`) monitoring GPU temps, VRAM, fan speeds; alerts via Telegram bot. |
| [FreeLLM API](https://github.com/chessarisilvio/freellm-api) | OpenAI‑compatible proxy aggregating 16+ free‑tier cloud providers; auto‑fallback to local 35 B P40 model. |
| [LLM Observability](https://github.com/chessarisilvio/llm-observability) | FastAPI (`:9192`) + Plotly exposing Prometheus metrics from llama‑server instances. |
| [Start‑Llama Launcher](https://github.com/chessarisilvio/start-llama) | CLI (`~/.local/bin/start-llama`) deploying llama‑server with five preset YAML configs for MTP, speculative, and MoE modes. |
| [llama.cpp Benchmark Suite](https://github.com/chessarisilvio/llamacpp-benchmark-suite) | CLI suite measuring tok/s, VRAM footprint, TTFT across consumer GPUs (RTX 3050) and datacenter Pascal cards. |

---  

## Tools & Automation  

| Project | Description |
|---------|-------------|
| [CUDA sm_61 Compatibility Shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim) | Runtime shim injecting PTX kernels compiled for sm_61, enabling Pascal GPUs to run modern CUDA 12 binaries. |
| [GGUF Model Manager](https://github.com/chessarisilvio/gguf-model-manager) | `gguf-manager` CLI for versioned model storage, automatic quantization, and hardware‑aware selection. |
| [Markitdown](https://github.com/chessarisilvio/markitdown) | CLI ingesting PDFs/DOCX/XLSX into ChromaDB for Retrieval‑Augmented Generation pipelines. |
| [Update GitHub Profile](https://github.com/chessarisilvio/update-github-profile) | Automated README refresh using LLM‑generated stats via `freellmapi` (`:9292`). |
| [Aider Integration](https://github.com/chessarisilvio/aider-integration) | Wrapper enabling Aider to offload heavy prompts to the local 35 B P40 model, reducing API costs. |

---  

## Embedded & Hardware  

| Project | Description |
|---------|-------------|
| [Controller Termico ESP32](https://github.com/chessarisilvio/controller-termico-esp32) | ESP32 firmware monitoring Tesla P40 temperatures via DS18B20 sensors; PWM‑driven fan control to avoid thermal throttling. |
| [Digital Thermal LCD](https://github.com/chessarisilvio/digital-thermal-lcd) | USB‑HID driver displaying real‑time CPU/GPU temps on Thermalright ARGB LCD panel. |
| [OpenClaw Gateway](https://github.com/chessarisilvio/openclaw) | Node.js multi‑channel AI gateway (Telegram, web) with session memory, tool‑use, and llama‑local backend. |
| [Silvioprint Bot](https://github.com/chessarisilvio/silvioprint) | Systemd‑managed Telegram bot automating content rendering and remote printing tasks. |

---  

## GitHub Stats  

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=transparent" alt="GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=chessarisilvio&layout=compact&theme=transparent" alt="Top Languages" />
</p>