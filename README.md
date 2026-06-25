<h1 align="center">Silvio Chessari</h1>
<p align="center">
  <b>LLM Inference Researcher · Self-Hosted AI Infrastructure · Embedded Systems</b><br>
  Optimizing speculative decoding on unsupported GPUs. Building AI tooling from scratch.<br>
  Tesla P40 whisperer. llama.cpp contributor. ESP32 tinkerer.
</p>

<br>

## Stack

| Layer | Details |
|-------|---------|
| **LLM Inference** | llama.cpp, ik_llama, BeeLLama (turbo3_tcq/sm_61), GGUF IQ4_XS, speculative decoding (EAGLE, MTP), MoE routing, EXL2 conversion |
| **Hardware** | NVIDIA Tesla P40 24GB (sm_61 Pascal), RTX 3050 8GB (sm_86), Intel i5-9400F, 20GB DDR4 |
| **Models** | Qwen3.6-35B-A3B (IQ4_XS, ctx 131k), Qwen3.5-9B (Q5_K_M), Qwen3.6-27B, custom GGUF quant pipeline |
| **Embedded** | ESP32, Arduino R4 WiFi, MQTT, Tailscale, HID, OLED/LCD displays |
| **Languages** | C/C++, Python, Bash, JavaScript |
| **Infra** | systemd services, Ollama gateway, Node.js, Flask, Tailscale mesh, Telegram bots |
| **OS** | Ubuntu 24.04 LTS |

<br>

## LLM Research

- [benchmark-4-agent-wrappers-on-qwen3627b-llamacpp](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp) — Comparative benchmark of 4 agent wrappers (Pi, OpenCode, Hermes, Qwen-Code) on Qwen3.6-27B Q4 via llama.cpp, measuring latency/VRAM on P40 and RTX 3050.
- [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) — Automated Qwen3_5MoeForC architecture fix, EXL2 conversion with mixed quantization, and validation benchmarks. C++ core + Python CLI.
- [auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) — Automated GGUF quantization pipeline: download checkpoints, benchmark on P40/3050, evaluate Q4_K_M vs Q5_K_S, produce production-ready GGUF files.
- [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) — Video input support for llama.cpp (mtmd): webcam/file frame acquisition piped to LLM inference. CMake integration + Python demo.
- [bias-personalizzato-per-whisper-locale](https://github.com/chessarisilvio/bias-personalizzato-per-whisper-locale) — Custom JSON/TSV bias module for Whisper + optional LLM-based contextual correction via local GGUF model.
- [secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault) — Encrypted local archive for LLM conversation contexts and retrieval chains.

<br>

## AI Infrastructure

- [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) — Local monitoring dashboard (port 9190): GPU telemetry, systemd services, AGENDA.md, automated idea generation from 35B model, unified security scanner.
- [openclaw](https://github.com/chessarisilvio/openclaw) — Ollama API gateway (Node.js): model routing, request proxying, local LLM orchestration.
- [automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) — Advanced watchdog for llama-stack: VRAM/token-rate monitoring, Telegram alerts, systemd auto-restart.
- [sistema-di-benchmarking-automatizzato-per-nuovi-mo](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-mo) — Automated GGUF benchmarking on P40 + RTX 3050 with auto-generated reports.
- [reddit-monitor](https://github.com/chessarisilvio/reddit-monitor) — Subreddit AI/tech monitor → AGENDA.md idea pipeline, 3h timer loop.

<br>

## Tools & Automation

- [megatool](https://github.com/chessarisilvio/megatool) — OSINT toolkit: C++ core + Flask web app (port 7788) + AI photo analysis.
- [modulo-offline-exifgps-geotagging-per-megatool](https://github.com/chessarisilvio/modulo-offline-exifgps-geotagging-per-megatool) — Offline EXIF/GPS extraction + reverse geocoding with local geographic databases.
- [videostudio](https://github.com/chessarisilvio/videostudio) — Spot AI generator from photos: LLM storyboard + Higgsfield clip composition, Flask backend (port 9195), prompt library.
- [pipeline-frame-interpolation-offline-per-mockup-s](https://github.com/chessarisilvio/pipeline-frame-interpolation-offline-per-mockup-s) — Offline frame interpolation (30→60fps) via Flowframes + FFmpeg, Python batch processing.
- [bot-short](https://github.com/chessarisilvio/bot-short) — Telegram bot for AI graphics: SVG pipeline, C++ backend.
- [silvioprint](https://github.com/chessarisilvio/silvioprint) — Telegram content bot (systemd service) + static e-commerce site for motorcycle graphics kits.
- [pipeline-grafiche-silvioprint](https://github.com/chessarisilvio/pipeline-grafiche-silvioprint) — OpenCV geometric warp (no generative AI) to apply graphics onto real motorcycle photos.

<br>

## Embedded & Hardware

- [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) — Physical dashboard: Arduino R4 WiFi + ESP32 + LCD showing P40/3050 status (VRAM, tok/s, uptime), voice commands via MQTT/Tailscale.
- [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) — ESP32 physical controller: rotary encoder + OLED SSD1306, HID/keyboard output to switch local AI models via OpenClaw gateway.
- [controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) — ESP32 proactive fan controller with thermal sensors.
- [digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd) — HID-based LCD temperature display (Thermalright).

<br>

<div align="center">

[![GitHub Stats](https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=dark&hide_title=true&count_private=true)](https://github.com/chessarisilvio)

</div>