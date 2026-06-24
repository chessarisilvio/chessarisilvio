<p align="center">
  <h1>Silvio Chessari</h1>
  <p><b>LLM Inference · AI Infrastructure · Embedded Systems</b></p>
</p>

Infrastructure engineer focused on local LLM inference, speculative decoding research, and running large models on unsupported GPU architectures. Building end-to-end AI stacks — from CUDA-level workarounds to production dashboards.

---

## Stack

| Domain | Technologies |
|---|---|
| LLM Inference | llama.cpp, GGUF, EXL2, speculative decoding, EAGLE, MTP, MoE routing |
| GPU Compute | NVIDIA Tesla P40 (sm_61), RTX 3050, CUDA compatibility workarounds, VRAM optimization |
| AI Infrastructure | Ollama, llama-stack, Node.js gateways, systemd services, automated watchdogs |
| Automation | Bash pipelines, Python orchestration, cron/Telegram alerting, benchmark automation |
| Embedded | ESP32, Arduino R4 WiFi, MQTT, Tailscale, HID, OLED/LCD displays |
| Tools | C++, Python, Flask, OpenCV, CMake, Git |

---

## LLM Research

- [auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) — Automated pipeline: download LLM checkpoints, benchmark on P40/3050, evaluate Q4_K_M vs Q5_K_S, produce production-ready GGUF with Obsidian vault updates.
- [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) — Toolchain for Qwen3_5MoeForC architecture fix, EXL2 conversion, mixed quantization, and validation benchmarks. Core C++ with Python CLI wrapper.
- [benchmark-4-agent-wrappers-on-qwen3627b-llamacpp](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp) — Comparative benchmark of Pi, OpenCode, Hermes, and Qwen-Code agent wrappers on Qwen3.6-27B Q4 via llama.cpp. Latency, VRAM, and output quality on orbital simulation prompts.
- [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) — Video input support for llama.cpp: CMake integration, video capture stubs, Python demo script for webcam/file-to-LLM inference.
- [nex2-mini-phase-twin-30b-lowvram-gguf-model](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model) — Low-VRAM GGUF model optimized for sub-24GB GPU deployment.
- [noema-atlas-rete-p2p-per-modelli-llm](https://github.com/chessarisilvio/noema-atlas-rete-p2p-per-modelli-llm) — P2P network for sharing LLM models across nodes.
- [secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault) — Encrypted archive for LLM conversation contexts and retrieval chains.

## AI Infrastructure

- [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) — Local monitoring dashboard (:9190): GPU panels, service health, AGENDA.md, sub-task worker, unified security scanner, public/personal idea feeds.
- [openclaw](https://github.com/chessarisilvio/openclaw) — Ollama gateway service built on Node.js.
- [automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) — Advanced watchdog for llama-stack: process monitoring, VRAM/token-rate anomaly detection, Telegram alerts, systemd auto-restart.
- [sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf) — Automated GGUF benchmarking on P40 and RTX 3050 with auto-generated reports.

## Tools & Automation

- [bot-short](https://github.com/chessarisilvio/bot-short) — Telegram bot for AI graphics: C++ core, SVG generation pipeline.
- [reddit-monitor](https://github.com/chessarisilvio/reddit-monitor) — Subreddit AI/tech monitor → AGENDA.md idea generation, 3-hour timer loop.
- [megatool](https://github.com/chessarisilvio/megatool) — OSINT toolkit: C++ core, Flask web app (:7788), AI photo analysis module.
- [videostudio](https://github.com/chessarisilvio/videostudio) — Spot AI from photos: LLM storyboard generation + Higgsfield clip compositing, prompt library, backend on :9195.
- [bias-personalizzato-per-whisper-locale](https://github.com/chessarisilvio/bias-personalizzato-per-whisper-locale) — Custom bias module for local Whisper: JSON/TSV bias loading, optional LLM-based contextual correction via GGUF.

## Embedded & Hardware

- [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) — Physical dashboard: Arduino R4 WiFi + LCD showing P40/3050 status (VRAM, tok/s, uptime), ESP32 voice commands, MQTT/Tailscale integration with OpenClaw gateway.
- [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) — ESP32-based physical AI model selector: rotary encoder navigation, OLED feedback, HID/OpenClaw command dispatch.
- [controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) — Proactive thermal fan controller on ESP32 with sensor array.
- [digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd) — HID-based LCD temperature display (Thermalright).
- [pipeline-grafiche-silvioprint](https://github.com/chessarisilvio/pipeline-grafiche-silvioprint) — Geometric warp pipeline (OpenCV, no generative AI) for applying graphics to real motorcycle photos.

---

<p align="center"><img src="https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=default&hide_title=true" height="165"> <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=chessarisilvio&layout=compact&theme=default&hide_title=true" height="165"></p>