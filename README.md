<h1 align="center">Silvio Chessari</h1>

<p align="center">
  LLM inference researcher · Self-built AI infrastructure · Embedded systems
</p>

<p align="center">
  Running speculative decoding research on unsupported GPUs. Building local AI stacks from scratch. Bridging embedded hardware with LLM pipelines.
</p>

---

## Stack

| Domain | Technologies |
|---|---|
| LLM Inference | llama.cpp, GGUF quantization, speculative decoding, EAGLE/MTP, MoE routing, EXL2 |
| GPU Compute | NVIDIA Tesla P40 (sm_61, 24GB VRAM), RTX 3050 (8GB VRAM), CUDA workarounds for unsupported architectures |
| AI Infrastructure | Ollama, LiteLLM alternatives, custom gateways, prompt/response caching, multi-model routing |
| Embedded | ESP32, Arduino R4 WiFi, HID devices, MQTT, Tailscale, OLED/LCD displays |
| Automation | systemd timers, bash pipelines, Python orchestration, Telegram notifications |
| Languages | C++, Python, Bash, CMake |

---

## LLM Research

- [dflash-kernel-attention-p40-llamacpp](https://github.com/chessarisilvio/dflash-kernel-attention-p40-llamacpp) — Custom attention kernel optimized for Tesla P40 (sm_61) inside llama.cpp, bypassing CUDA compute capability limitations
- [benchmark-4-agent-wrappers-qwen3627b-llamacpp](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-qwen3627b-llamacpp) — Comparative benchmark of four agent wrappers on Qwen3.6-27B via llama.cpp
- [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) — Automated EXL2 conversion with Qwen3_5MoeForC architecture fix, mixed quantization, and validation benchmarks
- [auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) — Automated GGUF quantization pipeline: download checkpoints, benchmark Q4_K_M vs Q5_K_S on P40/3050, select optimal quantization
- [benchmarking-automatizzato-gguf](https://github.com/chessarisilvio/benchmarking-automatizzato-gguf) — Automated GGUF benchmarking on P40 and RTX 3050 with automatic report generation
- [nex2-mini-phase-twin-30b-lowvram-gguf](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf) — Low-VRAM GGUF model optimized for 24GB consumer/datacenter GPUs
- [add-video-input-support-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-llamacpp-mtmd) — Video input support for llama.cpp via mtmd: webcam/file frame acquisition for multimodal inference
- [ai-gateway-prod-alternative-litellm](https://github.com/chessarisilvio/ai-gateway-prod-alternative-litellm) — Analysis of concrete LiteLLM alternatives for local AI gateways on consumer NVIDIA hardware

## AI Infrastructure

- [openclaw](https://github.com/chessarisilvio/openclaw) — Ollama gateway with Node.js, multi-model routing, and API compatibility layer
- [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) — Local monitoring dashboard (:9190): GPU status, services, AGENDA.md, worker sub-tasks, unified security scanner
- [secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault) — Encrypted archive for LLM context management and retrieval
- [boot-watchdog-ai-avanzato](https://github.com/chessarisilvio/boot-watchdog-ai-avanzato) — Advanced watchdog for llama-stack: VRAM monitoring, token-rate anomaly detection, Telegram alerts, systemd auto-restart
- [reddit-monitor](https://github.com/chessarisilvio/reddit-monitor) — Subreddit AI/tech monitor feeding ideas into AGENDA.md on 3h timer
- [voice-dictate](https://github.com/chessarisilvio/voice-dictate) — Local Whisper turbo dictation for Claude Code via hold-to-talk (replaces built-in voice mode for Italian)

## Tools & Automation

- [auto-vault-journal](https://github.com/chessarisilvio/auto-vault-journal) — Automatic Obsidian vault updater triggered by Claude Code Stop hook: Sonnet for vault files, freellmapi for narrative journal, 72h cleanup timer
- [megatool](https://github.com/chessarisilvio/megatool) — OSINT toolkit in C++ with Flask web app (:7788) and AI photo analysis
- [modulo-offline-exifgps-geotagging](https://github.com/chessarisilvio/modulo-offline-exifgps-geotagging) — Offline EXIF/GPS extraction with local reverse geocoding database
- [videostudio](https://github.com/chessarisilvio/videostudio) — Spot AI from photos: LLM storyboard generation + Higgsfield clip assembly (:9195)
- [bot-short](https://github.com/chessarisilvio/bot-short) — Telegram bot for AI graphics generation with SVG pipeline
- [systemd-timer-html-minification](https://github.com/chessarisilvio/systemd-timer-html-minification) — Automated HTML minification and GitHub Pages deployment via systemd timers

## Embedded & Hardware

- [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) — Physical dashboard with Arduino R4 WiFi + LCD showing P40/3050 status (VRAM, tok/s, uptime), ESP32 voice commands via MQTT/Tailscale
- [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) — ESP32 rotary encoder + OLED for local AI model selection, HID/OpenClaw integration
- [controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) — Proactive thermal fan controller with ESP32 and sensor array
- [digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd) — HID-based LCD temperature display for Thermalright coolers

---

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=default&hide_title=true&hide_border=true" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=chessarisilvio&layout=compact&hide_title=true&hide_border=true" />
</p>