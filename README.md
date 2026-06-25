<h1 align="center">Silvio Chessari</h1>
<p align="center">
  LLM inference researcher · Self-hosted AI infrastructure · Embedded systems engineer
</p>
<p align="center">
  Pushing speculative decoding, MoE routing, and consumer GPU workarounds on unsupported silicon — Tesla P40 (sm_61) and beyond.
</p>

## Stack

| Domain | Technologies |
|---|---|
| LLM Inference | llama.cpp, GGUF, EXL2, speculative decoding, EAGLE, MTP, MoE routing, Qwen3, llama-stack |
| Compute | NVIDIA Tesla P40 24GB (sm_61), RTX 3050 8GB, CUDA forward-compat workarounds, 20GB system RAM |
| AI Gateway | OpenClaw (Node.js), Ollama, LiteLLM alternatives, Docker, API OpenAI-compatible |
| Automation | systemd timers/watchdogs, Bash pipelines, Python orchestration, Telegram bots |
| Embedded | ESP32, Arduino R4 WiFi, MQTT, Tailscale, HID, OLED SSD1306, thermal/EXIF-GPS modules |
| Tools | C++, Python, Flask, CMake, OSINT pipelines, web dashboards |

## LLM Research

- [auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) — Automated pipeline: download new LLM checkpoints, benchmark on P40/3050, evaluate optimal GGUF quant point (Q4_K_M vs Q5_K_S), produce production-ready GGUF with Obsidian vault doc updates.
- [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) — Toolchain fixing Qwen3_5MoeForC architecture, converting checkpoints to EXL2 with mixed quantization, generating validation benchmarks. Core C++ with Python CLI wrapper.
- [benchmark-4-agent-wrappers-on-qwen3627b-llamacpp](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp) — Comparative benchmark of four agent wrappers on Qwen3.6-27B via llama.cpp.
- [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) — Video input support for llama.cpp: CMake integration, video capture stubs, Python demo script for webcam/file-to-LLM inference.
- [sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf) — Automated GGUF benchmarking on P40 and RTX 3050 with auto-generated reports.
- [nex2-mini-phase-twin-30b-lowvram-gguf-model](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model) — Low-VRAM GGUF model optimized for sub-24GB deployments, ready to use.
- [secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault) — Encrypted archive for LLM conversation contexts and retrieval chains.

## AI Infrastructure

- [ai-gateway-in-prod-alternative-concrete-a-litellm](https://github.com/chessarisilvio/ai-gateway-in-prod-alternative-concrete-a-litellm) — Evaluation of 10 LiteLLM alternatives for local AI gateway on consumer NVIDIA hardware; focus on intelligent routing, prompt/response caching, multi-model/multi-user support, OpenAI-compatible API, Docker deploy.
- [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) — Local monitoring dashboard (:9190): GPU panels, service health, system metrics, AGENDA.md, sprint tracker, unified security scanner, public/personal idea board.
- [automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) — Advanced watchdog for llama-stack: process monitoring, VRAM tracking, token-rate anomaly detection, Telegram alerts, systemd auto-restart.
- [openclaw](https://github.com/chessarisilvio/openclaw) — Ollama gateway on Node.js; core routing layer for local AI stack.
- [voice-dictate](https://github.com/chessarisilvio/voice-dictate) — Local Whisper turbo GPU dictation for Claude Code; hold Space in terminal, replaces built-in voice mode with improved Italian support.

## Tools & Automation

- [megatool](https://github.com/chessarisilvio/megatool) — OSINT suite: C++ core, Flask web app (:7788), AI photo analysis pipeline.
- [modulo-offline-exifgps-geotagging-per-megatool](https://github.com/chessarisilvio/modulo-offline-exifgps-geotagging-per-megatool) — Offline EXIF/GPS extraction + reverse geocoding with local geographic databases.
- [reddit-monitor](https://github.com/chessarisilvio/reddit-monitor) — Subreddit AI/tech monitor → auto-populates AGENDA.md ideas, 3-hour timer cycle.
- [bot-short](https://github.com/chessarisilvio/bot-short) — Telegram bot for AI graphics, SVG generation pipeline.
- [silvioprint](https://github.com/chessarisilvio/silvioprint) — Telegram content bot, systemd service.
- [pipeline-grafiche-silvioprint](https://github.com/chessarisilvio/pipeline-grafiche-silvioprint) — Geometric warp pipeline: motorcycle graphics split-to-photo workflow.
- [videostudio](https://github.com/chessarisilvio/videostudio) — Spot AI from photos (:9195): LLM storyboard generation + Higgsfield clip embedding, prompt library.
- [automazione-systemd-timer-per-html-minification-gi](https://github.com/chessarisilvio/automazione-systemd-timer-per-html-minification-gi) — Automated HTML minification + GitHub Pages deploy via systemd timer.

## Embedded & Hardware

- [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) — Physical dashboard: Arduino R4 WiFi + LCD showing P40/3050 status (VRAM, tok/s, uptime), ESP32 voice commands, MQTT/Tailscale integration with OpenClaw gateway.
- [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) — ESP32-based physical AI model selector: rotary encoder navigation, OLED SSD1306 feedback, HID/keyboard output to local AI gateway.
- [controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) — Proactive thermal fan controller on ESP32 with sensor array.
- [digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd) — Thermalright LCD temperature display via HID interface.

---

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=default&hide_title=false&count_private=true)

</div>