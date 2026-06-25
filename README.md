<h1 align="center">Silvio Chessari</h1>
<p align="center">
  <b>LLM inference researcher · AI infrastructure engineer · Embedded systems developer</b>
</p>

---

## 🛠️ Technical Stack

| Domain | Technologies |
|---|---|
| **LLM Inference** | llama.cpp, GGUF, EXL2, speculative decoding, EAGLE, MTP, MoE routing, quantization (Q4_K_M, Q5_K_S) |
| **GPU Compute** | CUDA workarounds for unsupported hardware (NVIDIA Tesla P40, RTX 3050), sm_61 compatibility, VRAM optimization |
| **AI Infrastructure** | Ollama, OpenClaw gateway, Hugging Face Hub, automated model benchmarking, EXL2 conversion pipelines |
| **Automation** | systemd services & timers, watchdog daemons, Telegram notification bots, bash orchestration |
| **Embedded** | ESP32, Arduino R4 WiFi, MQTT, Tailscale, HID devices, OLED/LCD displays, thermal sensing |
| **Languages & Tools** | Python, C++, C, Bash, CMake, Flutter, Flask, Node.js, OpenCV |

---

## 🔬 LLM Research & Inference

- **[auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf)** — Automated GGUF quantization of new LLM checkpoints with benchmark-driven calibration for P40 / RTX 3050
- **[automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline)** — C++/Python toolchain for architecture-level fixes on Qwen MoE models, EXL2 conversion, mixed quantization, and validation benchmarks
- **[benchmark-4-agent-wrappers-on-qwen3627b-llamacpp](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp)** — Comparative benchmark of four agent wrappers (Pi, OpenCode, Hermes, Qwen-Code) on Qwen3.6-27B quantized via llama.cpp
- **[add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd)** — Video input integration for llama.cpp with CMake flags and Python client for frame acquisition
- **[nex2-mini-phase-twin-30b-lowvram-gguf-model](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model)** — Low-VRAM GGUF model ready for deployment on consumer hardware
- **[benchmark-4-agent-wrappers-latency-vram](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-latency-vram)** — Latency, VRAM, and output quality profiling for agent wrappers on llama.cpp

---

## 🖥️ AI Infrastructure

- **[ai-dashboard](https://github.com/chessarisilvio/ai-dashboard)** — Local monitoring dashboard (port :9190) with GPU status, AGENDA system, task management, unified security scanner, and auto-generated ideation pipeline
- **[sistema-di-benchmarking-automatizzato-per-nuovi-mo](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-mo)** — Automated GGUF benchmarking system for new models running on Tesla P40 and RTX 3050 with automatic report generation
- **[openclaw](https://github.com/chessarisilvio/openclaw)** — Node.js Ollama gateway service for model routing and orchestration
- **[automazione-boot-watchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-boot-watchdog-ai-avanzato)** — Advanced systemd watchdog monitoring llama-stack with VRAM, token rate, anomaly detection, and Telegram alerting
- **[voice-dictate](https://github.com/chessarisilvio/voice-dictate)** — Local Whisper-based dictation system using Claude Code as a GPU-accelerated alternative to native voice mode, optimized on Italian benchmarks
- **[bias-personalizzato-per-whisper-locale](https://github.com/chessarisilvio/bias-personalizzato-per-whisper-locale)** — Custom bias configuration and fine-tuning for local Whisper transcription

---

## 🔧 Tools & Automation

- **[megatool](https://github.com/chessarisilvio/megatool)** — OSINT platform in C++ with Flask web app (port :7788), AI photo analysis, and offline EXIF/GPS geotagging module
- **[reddit-monitor](https://github.com/chessarisilvio/reddit-monitor)** — Automated subreddit scanner for AI/tech content piped into AGENDA idea generation with configurable loop interval
- **[automazione-systemd-timer-html-minification](https://github.com/chessarisilvio/automazione-systemd-timer-html-minification)** — systemd-timer-driven HTML minifier for automated static site updates and GitHub Pages deployments
- **[secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault)** — Encrypted archive system for managing and persisting LLM conversation contexts
- **[bot-short](https://github.com/chessarisilvio/bot-short)** — Telegram bot with AI-powered SVG graphics pipeline

---

## 🔌 Embedded & Hardware

- **[ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard)** — Hardware dashboard (Arduino R4 WiFi + ESP32) displaying P40/3050 VRAM, tok/s, uptime via MQTT over Tailscale
- **[ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller)** — ESP32-based physical model selector with rotary encoder, OLED feedback, HID interfacing, and OpenClaw gateway integration
- **[controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32)** — Proactive thermal fan controller on ESP32 with multi-sensor input
- **[digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd)** — Thermalright temperature display via USB HID and LCD output

---

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=transparent&hide_title=true&hide_border=true" />
</div>