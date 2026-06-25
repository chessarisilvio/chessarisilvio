<h1 align="center">Silvio Chessari</h1>
<p align="center">
  <b>LLM Inference Researcher · AI Infrastructure Engineer · Embedded Systems Developer</b><br>
  Running large language models on unsupported hardware. Building local AI infrastructure from scratch.<br>
  Speculative decoding, MoE routing, CUDA workarounds, ESP32 — production-grade work, zero cloud dependency.
</p>

## 🛠 Technical Stack

| Domain | Technologies |
|---|---|
| **LLM Inference** | llama.cpp, GGUF, EXL2, speculative decoding, EAGLE, MTP, MoE expert routing, Qwen3, Qwen3.6-27B |
| **GPU Compute** | Tesla P40 (sm_61, 24GB), RTX 3050 (8GB), CUDA forward-compat patches, VRAM-constrained quantization |
| **AI Infrastructure** | Ollama, LiteLLM alternatives, OpenClaw gateway, multi-model routing, prompt/response caching |
| **Embedded** | ESP32, Arduino R4 WiFi, MQTT, Tailscale, HID, OLED SSD1306, thermal/EXIF sensors |
| **Automation** | systemd timers, watchdog daemons, Telegram bots, Reddit monitors, HTML minification pipelines |
| **Languages** | Python, C/C++, Bash, JavaScript, CMake |
| **Tools** | Git, Docker, Flask, Node.js, llama.cpp server, llama-stack |

## 🔬 LLM Research

- [auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) — Automated pipeline: download checkpoints → benchmark on P40/3050 → evaluate Q4_K_M vs Q5_K_S → produce production GGUF with Obsidian vault doc updates.
- [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) — Toolchain fixing Qwen3_5MoeForC architecture, EXL2 conversion, mixed quantization, and benchmark validation. Core C++ with Python CLI orchestration.
- [benchmark-4-agent-wrappers-on-qwen3627b-llamacpp](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp) — Comparative benchmark of four agent wrappers running Qwen3.6-27B via llama.cpp on consumer/datacenter GPUs.
- [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) — Video input support for llama.cpp: CMake `LLAMA_VIDEO_INPUT` flag, webcam/file frame acquisition stubs, Python example script.
- [sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf) — Automated GGUF benchmarking on P40 and RTX 3050 with automatic report generation.
- [nex2-mini-phase-twin-30b-lowvram-gguf-model](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model) — Low-VRAM GGUF model package ready for deployment on memory-constrained GPUs.
- [secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault) — Encrypted archive for LLM conversation contexts and retrieval pipelines.

## 🖥 AI Infrastructure

- [ai-gateway-in-prod-alternative-concrete-a-litellm](https://github.com/chessarisilvio/ai-gateway-in-prod-alternative-concrete-a-litellm) — Evaluation of 10 LiteLLM alternatives for local AI gateway on P40+3050 hardware. Focus: intelligent routing, prompt/response caching, multi-model/multi-user, OpenAI-compatible API, Docker deploy.
- [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) — Local monitoring dashboard (`:9190`): GPU panels, service health, system metrics, AGENDA.md, sprint tracker, unified security scanner, public/personal idea feeds.
- [openclaw](https://github.com/chessarisilvio/openclaw) — Ollama gateway service built on Node.js for local LLM orchestration.
- [automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) — Advanced watchdog for `llama-stack`: process monitoring, VRAM tracking, token-rate anomaly detection, Telegram alerts, systemd auto-restart.

## ⚙️ Tools & Automation

- [voice-dictate](https://github.com/chessarisilvio/voice-dictate) — Local Whisper turbo dictation for Claude Code: hold Space → GPU transcription replacing integrated voice mode. Optimized for Italian.
- [reddit-monitor](https://github.com/chessarisilvio/reddit-monitor) — Subreddit AI/tech monitor → auto-populates AGENDA.md ideas, 3-hour timer cycle.
- [bot-short](https://github.com/chessarisilvio/bot-short) — Telegram bot for AI graphics: SVG generation pipeline.
- [megatool](https://github.com/chessarisilvio/megatool) — OSINT toolkit: C++ core + Flask web app (`:7788`) + AI photo analysis.
- [modulo-offline-exifgps-geotagging-per-megatool](https://github.com/chessarisilvio/modulo-offline-exifgps-geotagging-per-megatool) — Offline EXIF/GPS extraction + reverse geocoding with local geographic databases.
- [videostudio](https://github.com/chessarisilvio/videostudio) — Spot AI from photos (`:9195`): LLM storyboard generation + Higgsfield clip embedding + prompt library.
- [automazione-systemd-timer-per-html-minification](https://github.com/chessarisilvio/automazione-systemd-timer-per-html-minification) — Automated HTML minification + GitHub Pages deploy via systemd timer.

## 📡 Embedded & Hardware

- [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) — Physical dashboard: Arduino R4 WiFi + LCD showing P40/3050 status (VRAM, tok/s, uptime), ESP32 voice commands, MQTT/Tailscale integration with OpenClaw gateway.
- [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) — ESP32-based physical AI model selector: rotary encoder navigation, OLED SSD1306 feedback, HID/keyboard commands to local AI stack.
- [controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) — Proactive thermal fan controller on ESP32 with multi-sensor input.
- [digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd) — Thermalright LCD temperature display via HID interface.

---

<p align="center"><img src="https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=default&hide_title=true&count_private=true" /></p>