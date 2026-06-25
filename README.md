<h1 align="center">Silvio Chessari</h1>
<p align="center">AI/LLM infrastructure engineer. Local-first inference on consumer and datacenter GPUs. Building toolchains that make LLMs run where they shouldn't.</p>
<p align="center">Tesla P40 · RTX 3050 · CUDA workarounds · llama.cpp · GGUF · llama.cpp MoE</p>

---

## Stack

| Domain | Technologies |
|---|---|
| LLM Inference | llama.cpp, GGUF, EXL2, MoE routing, LlamaStack |
| GPU Compute | CUDA (sm_61 Pascal), PTX-level workarounds, mixed-precision quantization |
| LLM Research | EAGLE, MTP, speculative decoding, MoE, quantization-aware inference |
| Languages | Python, C++, C (CUDA kernels), Bash |
| Infrastructure | systemd, MQTT, Tailscale, Docker, Ollama, OpenClaw |
| Hardware/Embedded | ESP32, Arduino R4 WiFi, HID, OLED SSD1306, rotary encoders |
| Vision/ML | OpenCV, YOLO, Whisper (finetuned), AI upscaling pipelines |

---

## 🔬 LLM Research

| | |
|---|---|
| [EAGLE/MTP Speculative Decoding](https://github.com/chessarisilvio/eagle-mtp-speculative-decoding) | Research and implementation of EAGLE and MTP speculative decoding strategies for accelerating LLM inference on consumer GPUs, with benchmarks against standard autoregressive generation. |
| [GGUF Auto-Quantization Pipeline](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) | Automated pipeline that downloads new LLM checkpoints, benchmarks quantization points (Q4_K_M vs Q5_K_S) on local hardware (P40 / RTX 3050), and produces production-ready GGUF files with vault documentation updates. |
| [Automated EXL2 Conversion & Validation](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) | Toolchain automating architecture fixes for Qwen3 MoE checkpoints, EXL2 format conversion, mixed-quantization application, and validation benchmarks. Core C++ with Python CLI orchestration. |
| [Video Input for llama.cpp (mtmd)](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) | Adds native video input to llama.cpp — frame capture from webcam/video files, integration with the mtmd server endpoint, CMake option `LLAMA_VIDEO_INPUT`, and Python demo script. |
| [Benchmark: 4 Agent Wrappers on Qwen3.6-27B](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp) | Comparative benchmark of Pi, OpenCode, Hermes, and Qwen-Code agent wrappers on Qwen3.6-27B Q4 via llama.cpp, measuring latency, VRAM consumption, and output quality on orbital simulation prompts. |
| [Nex2 Mini Phase Twin 30B low-VRAM GGUF](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model) | Optimized low-VRAM GGUF model package ready for deployment on sub-24GB GPUs. |
| [GGUF Benchmarking Suite](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-mo) | Automated GGUF benchmarking harness for Tesla P40 and RTX 3050 with automatic report generation. |

---

## 🖥️ AI Infrastructure

| | |
|---|---|
| [OpenClaw — Ollama Gateway](https://github.com/chessarisilvio/openclaw) | Node.js gateway bridging Ollama with local orchestration layers; API routing, model lifecycle management, and health monitoring. |
| [AI Dashboard + AGENDA](https://github.com/chessarisilvio/ai-dashboard) | Local web dashboard (`:9190`) for GPU monitoring, systemd services, AGENDA.md task tracking, sprint status, and automated security scanning. 35B local model generates ideas daily. |
| [Secure LLM Context Vault](https://github.com/chessarisilvio/secure-llm-context-vault) | Encrypted archival system for LLM conversation contexts — persistent retrieval without plaintext exposure of sensitive prompt data. |
| [Voice Dictate for Claude Code](https://github.com/chessarisilvio/voice-dictate) | Hold-to-talk Whisper turbo (GPU-accelerated) replacing Claude Code's built-in voice mode; Italian-optimized for the local P40 pipeline. |
| [Advanced AI Boot/Watchdog](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzado) | systemd watchdog for llama-stack monitoring process health, VRAM usage, and token-rate; Telegram anomaly alerts with automatic service restart. |
| [Reddit AI/tech Monitor](https://github.com/chessarisilvio/reddit-monitor) | Subreddit crawler feeding AI/tech ideas into AGENDA.md on a 3-hour cycle. |

---

## 🔧 Tools & Automation

| | |
|---|---|
| [Custom Whisper Bias](https://github.com/chessarisilvio/bias-personalizzato-per-whisper-locale) | Custom transcription bias profiles for local Whisper — domain-specific terminology and Italian dialect handling to reduce WER. |

---

## ⚡ Embedded & Hardware

| | |
|---|---|
| [AI Home Assistant HID Dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) | Physical LCD dashboard (Arduino R4 WiFi + ESP32) displaying real-time P40/3050 VRAM, tok/s, and uptime via MQTT over Tailscale; voice command passthrough. |
| [AI Model Selector Controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) | ESP32-based hardware controller with rotary encoder, OLED SSD1306, and HID/keyboard output for selecting and launching local AI models physically. |
| [Proactive ESP32 Thermal Controller](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) | ESP32-driven fan control with proactive thermal management based on multi-sensor readings. |

---

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=default&hide_title=false&count_private=true)

</div>