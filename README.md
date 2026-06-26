<h1 align="center">Silvio Chessari</h1>
<p align="center">
  LLM inference systems · self-hosted AI infrastructure · embedded & GPU compute
</p>

<!-- 🔧 -->

## Stack

| Domain | Technologies |
|---|---|
| LLM Inference | llama.cpp, GGUF, speculative decoding, EAGLE, MTP, MoE routing, ExLlamaV2 |
| Hardware | NVIDIA Tesla P40 (sm_61), RTX 3050 (sm_86), CUDA forward-port workarounds |
| AI Infra | Ollama, self-hosted gateways, LiteLLM alternatives, custom systemd watchdog |
| Languages | Python, Bash, C/C++, CMake |
| Embedded | ESP32, Arduino R4 WiFi, OLED/SSD1306, HID over MQTT, Tailscale |
| Tools | systemd/timers, Flask, Telegram bots, GitHub Pages CI |

## LLM Research

- [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) — Toolchain for architecture fix, EXL2 conversion, mixed quantization, and benchmark validation
- [auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) — Automated GGUF quantization pipeline with benchmark selection on P40 and RTX 3050
- [benchmark-4-agent-wrappers-on-qwen3627b-llamacpp](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp) — Comparative benchmark of four agent wrappers on Qwen3.6-27B via llama.cpp
- [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) — Video input support patch for llama.cpp (mtmd), webcam/file frame acquisition with Python bindings
- [sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf) — Automated GGUF benchmarking system generating reports on P40 and RTX 3050

## AI Infrastructure

- [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) — Local AI dashboard: GPU monitoring, AGENDA.md, security scanner, public/private idea pipeline
- [ai-gateway-in-prod-alternative-concrete-a-litellm](https://github.com/chessarisilvio/ai-gateway-in-prod-alternative-concrete-a-litellm) — Evaluation of 10 self-hosted AI gateway alternatives to LiteLLM optimized for consumer GPU stacks
- [automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) — Advanced systemd watchdog for llama-stack: VRAM monitoring, t/s telemetry, Telegram alerts, auto-restart
- [secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault) — Encrypted vault for storing and retrieving LLM conversation contexts
- [voice-dictate](https://github.com/chessarisilvio/voice-dictate) — Local voice dictation via Whisper turbo (GPU), Claude Code hotkey integration
- [openclaw](https://github.com/chessarisilvio/openclaw) — Ollama API gateway, Node.js multi-model proxy

## Tools & Automation

- [bot-short](https://github.com/chessarisilvio/bot-short) — Telegraph bot for AI graphics with SVG rendering pipeline
- [megatool](https://github.com/chessarisilvio/megatool) — OSINT suite: C++ core, Flask web app, AI photo analysis
- [modulo-offline-exifgps-geotagging-per-megatool](https://github.com/chessarisilvio/modulo-offline-exifgps-geotagging-per-megatool) — Offline EXIF/GPS extraction and reverse geocoding with local geographic databases
- [reddit-monitor](https://github.com/chessarisilvio/reddit-monitor) — Subreddit AI/tech monitor feeding ideas into AGENDA.md every 3 hours
- [silvioprint](https://github.com/chessarisilvio/silvioprint) — Automated content delivery bot via Telegram
- [silvioprint-sito-web](https://github.com/chessarisilvio/silvioprint-sito-web) — Static e-commerce site (HTML/CSS/JS) for motorcycle graphics kits
- [pipeline-grafiche-silviopprint](https://github.com/chessarisilvio/pipeline-grafiche-silvioprint) — Geometric warp pipeline converting motorcycle photos to editable SVG
- [automazione-systemd-timer-per-html-minificazione](https://github.com/chessarisilvio/automazione-systemd-timer-per-html-minificazione) — Automated HTML minification and GitHub Pages deployment via systemd timer
- [videostudio](https://github.com/chessarisilvio/videostudio) — Video generation web app: LLM storyboard creation with Higgsfield clip integration prompt library

## Embedded & Hardware

- [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) — Physical dashboard with Arduino R4 WiFi + ESP32: VRAM, tok/s, uptime display; vocal commands via MQTT/Tailscale to local AI gateway
- [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) — ESP32 physical model selector: rotary encoder navigation, OLED 1306 feedback, HID commands to OpenClaw gateway
- [controller-termico-esp32](https://github.com/chessarisilvio/controller-termico-esp32) — Proactive thermal fan controller on ESP32 with multi-sensor input
- [digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd) — HID-based temperature display on custom LCD panel

---

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=transparent&hide_title=true&count_private=true)

</div>