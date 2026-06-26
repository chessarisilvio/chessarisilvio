<h1 align="center">Silvio Chessari</h1>
<p align="center">
  AI/ML Engineer · LLM Inference Researcher · Self-Hosted AI Infrastructure · Embedded Systems
</p>
<p align="center">
  Optimizing LLM inference on unsupported hardware · speculative decoding · MoE routing · CUDA workarounds · ESP32/Arduino
</p>

## Stack

| Domain | Technologies |
|---|---|
| LLM Inference | llama.cpp, GGUF, EXL2, speculative decoding, EAGLE, MTP, MoE routing, Qwen3, llama-server |
| Hardware | NVIDIA Tesla P40 (sm_61, 24 GB VRAM), RTX 3050 (8 GB VRAM), CUDA version workarounds |
| AI Infrastructure | Ollama, OpenClaw gateway, LiteLLM alternatives, Docker, systemd, Tailscale |
| Languages | Python, C/C++, Bash, CMake |
| Embedded | ESP32, Arduino R4 WiFi, MQTT, HID, OLED SSD1306 |
| Automation | systemd timers/hooks, Telegram bots, Obsidian vault tooling |

## LLM Research

- [auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) — Automated pipeline: download checkpoints → benchmark on P40/RTX3050 → evaluate Q4_K_M vs Q5_K_S → produce production GGUF files with vault doc updates.
- [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) — Toolchain for Qwen3_5MoeForC architecture fix, EXL2 conversion, mixed quantization, and benchmark validation. Core C++ with Python CLI wrapper.
- [benchmark-4-agent-wrappers-on-qwen3627b-llamacpp](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp) — Comparative benchmark of four agent wrappers serving Qwen3.6-27B via llama.cpp.
- [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) — Video input support for llama.cpp: CMake integration, video frame stubs, Python demo script for webcam/file-to-server inference.
- [nex2-mini-phase-twin-30b-lowvram-gguf-model](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model) — Low-VRAM GGUF model optimized for sub-24GB deployments, ready to use.
- [sistema-di-benchmarking-automatizzato-per-nuovi-modelli](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-modelli) — Automated GGUF benchmarking on P40 and RTX3050 with auto-generated reports.
- [secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault) — Encrypted archive for persistent LLM context storage and retrieval.

## AI Infrastructure

- [ai-gateway-in-prod-alternative-concrete-a-litellm](https://github.com/chessarisilvio/ai-gateway-in-prod-alternative-concrete-a-litellm) — Analysis of 10 LiteLLM alternatives for local AI gateways on consumer NVIDIA hardware (P40 + RTX3050, 20GB RAM), with focus on intelligent routing, prompt/response caching, multi-model support, OpenAI-compatible API.
- [openclaw](https://github.com/chessarisilvio/openclaw) — Ollama gateway service, Node.js, production deployment.
- [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) — Local monitoring dashboard (:9190): GPU panels, services, system health, AGENDA.md, worker sub-tasks, unified security scanner, public/personal idea tracking.
- [automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) — Advanced watchdog for llama-stack: process monitoring, VRAM tracking, token-per-second anomaly detection, Telegram alerts, systemd auto-restart.

## Tools & Automation

- [auto-vault-journal](https://github.com/chessarisilvio/auto-vault-journal) — Automatic Obsidian vault updater triggered by Claude Code Stop hook; extracts session title, user requests, modified files via JSONL transcript; Sonnet for vault files, freellmapi for narrative journal; 72h cleanup timer.
- [voice-dictate](https://github.com/chessarisilvio/voice-dictate) — Local Whisper turbo GPU dictation for Claude Code: hold Space in terminal, replaces built-in voice mode with improved Italian recognition.
- [reddit-monitor](https://github.com/chessarisilvio/reddit-monitor) — Subreddit AI/tech monitor → auto-populates AGENDA.md ideas, 3-hour timer cycle.
- [megatool](https://github.com/chessarisilvio/megatool) — OSINT toolkit: C++ core + Flask web app (:7788) + AI photo analysis pipeline.
- [modulo-offline-exifgps-geotagging-per-megatool](https://github.com/chessarisilvio/modulo-offline-exifgps-geotagging-per-megatool) — Offline EXIF/GPS metadata extraction with local geographic database for reverse geocoding.
- [bot-short](https://github.com/chessarisilvio/bot-short) — Telegram bot for AI graphics: SVG generation pipeline.
- [silvioprint](https://github.com/chessarisilvio/silvioprint) — systemd service bot for Telegram content distribution.

## Embedded & Hardware

- [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) — Physical dashboard: Arduino R4 WiFi + LCD showing P40/3050 status (VRAM, tok/s, uptime), ESP32 voice commands, MQTT/Tailscale integration with OpenClaw gateway.
- [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) — ESP32-based physical AI model selector: rotary encoder navigation, OLED SSD1306 feedback, HID/keyboard commands to local AI stack.
- [controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) — Proactive thermal fan controller on ESP32 with sensor array.
- [digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd) — Thermalright LCD temperature display via HID interface.

---

<p align="center"><img src="https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=default&hide_title=true&count_private=true" /></p>