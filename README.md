<h1 align="center">Silvio Chessari</h1>
<p align="center">
  <b>LLM Inference Researcher · Self-Hosted AI Infrastructure · Embedded Systems</b>
</p>
<p align="center">
  Optimizing speculative decoding on unsupported GPUs · Running MoE models on 24GB consumer VRAM · Building end-to-end local AI pipelines
</p>

---

## Stack

| Domain | Technologies |
|---|---|
| LLM Inference | llama.cpp, GGUF quantization, EAGLE, MTP, speculative decoding, MoE routing, EXL2 |
| GPU Compute | NVIDIA Tesla P40 (sm_61, 24GB), RTX 3050 (8GB), CUDA version workarounds, VRAM-constrained serving |
| AI Infrastructure | Ollama, OpenClaw gateway, LiteLLM alternatives, multi-model routing, prompt/response caching |
| Automation | systemd timers, Claude Code hooks, bash pipelines, Telegram bots, scheduled benchmarking |
| Embedded | ESP32, Arduino R4 WiFi, MQTT, Tailscale, HID, OLED/SSD1306, thermal sensing |
| Backend | Python, C++, Flask, Node.js, Docker, CMake |
| OSINT & Tools | C++ toolchains, offline EXIF/GPS extraction, reverse geocoding |

---

## LLM Research

- [auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) — Automated pipeline: download checkpoints → benchmark on P40/3050 → evaluate Q4_K_M vs Q5_K_S → produce production GGUF with Obsidian vault doc updates.
- [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) — Toolchain for Qwen3_5MoeForC architecture fix, EXL2 conversion, mixed quantization, and validation benchmarks. Core C++ with Python CLI orchestration.
- [benchmark-4-agent-wrappers-on-qwen3627b-llamacpp](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp) — Comparative benchmark of four agent wrappers serving Qwen3.6-27B via llama.cpp.
- [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) — CMake integration and video input stubs for llama.cpp: webcam/file frame acquisition for multimodal LLM inference.
- [nex2-mini-phase-twin-30b-lowvram-gguf-model](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model) — Low-VRAM GGUF model optimized for sub-24GB deployments, ready-to-use.
- [sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf) — Automated GGUF benchmarking on P40 and RTX 3050 with auto-generated reports.

## AI Infrastructure

- [ai-gateway-in-prod-alternative-concrete-a-litellm](https://github.com/chessarisilvio/ai-gateway-in-prod-alternative-concrete-a-litellm) — Analysis of 10 LiteLLM alternatives for local AI gateways on consumer NVIDIA hardware (P40 + RTX 3050, 20GB RAM): routing, caching, multi-model, OpenAI-compatible API, Docker deploy.
- [openclaw](https://github.com/chessarisilvio/openclaw) — Ollama gateway with Node.js orchestration for local model serving.
- [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) — Local monitoring dashboard (:9190): GPU panels, service health, AGENDA.md, worker sub-tasks, unified security scanner, public/personal idea tracking.
- [automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) — Advanced watchdog for llama-stack: process monitoring, VRAM/token-rate anomaly detection, Telegram alerts, systemd auto-restart.
- [secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault) — Encrypted archive for LLM conversation contexts and retrieval-safe storage.

## Tools & Automation

- [auto-vault-journal](https://github.com/chessarisilvio/auto-vault-journal) — Automatic Obsidian vault updater triggered by Claude Code Stop hook: extracts session transcripts, titles, modified files; uses Sonnet for structured vault entries and freellmapi for narrative journals; 72h cleanup timer.
- [voice-dictate](https://github.com/chessarisilvio/voice-dictate) — Local Whisper turbo GPU dictation for Claude Code: hold Space → transcribe → inject into terminal. Replaces built-in voice mode with better Italian support.
- [reddit-monitor](https://github.com/chessarisilvio/reddit-monitor) — Subreddit AI/tech monitor → auto-populates AGENDA.md ideas, 3h timer cycle.
- [megatool](https://github.com/chessarisilvio/megatool) — OSINT suite: C++ core + Flask web app (:7788) + AI photo analysis pipeline.
- [modulo-offline-exifgps-geotagging-per-megatool](https://github.com/chessarisilvio/modulo-offline-exifgps-geotagging-per-megatool) — Offline EXIF/GPS metadata extraction with local geographic database for reverse geocoding.
- [videostudio](https://github.com/chessarisilvio/videostudio) — Spot AI from photos: LLM storyboard generation + Higgsfield clip compositing, Flask backend (:9195), prompt library.
- [bot-short](https://github.com/chessarisilvio/bot-short) — Telegram bot for AI graphics with SVG pipeline generation.

## Embedded & Hardware

- [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) — Physical dashboard: Arduino R4 WiFi + LCD showing P40/3050 status (VRAM, tok/s, uptime), ESP32 voice commands, MQTT over Tailscale integration with OpenClaw gateway.
- [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) — ESP32-based hardware controller: rotary encoder navigation, OLED SSD1306 feedback, HID/keyboard output for local AI model selection.
- [controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) — Proactive thermal fan controller on ESP32 with sensor array.
- [digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd) — Thermalright LCD temperature display via HID interface.

---

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=transparent&hide_title=true&count_private=true)

</div>