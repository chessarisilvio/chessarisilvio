<h1 align="center">Silvio Chessari</h1>
<p align="center">
  Independent AI engineer — LLM inference research, speculative decoding (EAGLE/MTP/MoE routing), CUDA kernels on unsupported GPUs, self-built AI infrastructure & embedded HID controllers.
</p>

---

## Stack

| Domain | Tools |
|--------|-------|
| LLM Inference | llama.cpp, Ollama, vLLM, speculative decoding (EAGLE, MTP), GGUF quantization |
| GPUs | NVIDIA Tesla P40 (sm_61, 24 GB VRAM), RTX 3050 (8 GB), CUDA workarounds on legacy arch |
| Languages | Python, C++, Kotlin, Bash, TypeScript |
| Infrastructure | Proxmox VE, Docker, systemd, Tailscale, MQTT |
| Embedded | ESP32, Arduino R4 WiFi, OLED/HID, MQTT telemetry |

---

## Projects

### LLM Research & Inference

- **[llm-inference-research](https://github.com/chessarisilvio/llm-inference-research)** — Research repo: EAGLE speculative decoding, MoE routing, CUDA kernel optimization for llama.cpp
- **[dflash-kernel-attention-p40](https://github.com/chessarisilvio/dflash-kernel-attention-p40)** — Optimized Flash-Attention kernel for Tesla P40 (sm_61) in llama.cpp, working around compute capability limitations
- **[auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf)** — Automated GGUF quantization pipeline: benchmark new checkpoints on P40 + RTX 3050, select optimal Q-point (Q4_K_M / Q5_K_S), generate production-ready models
- **[benchmark-agent-wrappers-qwen36-27b](https://github.com/chessarisilvio/benchmark-agent-wrappers-qwen36-27b)** — Comparative benchmark of 4 AI agent wrappers on Qwen3.6-27B via llama.cpp
- **[automated-exl2-conversion-validation](https://github.com/chessarisilvio/automated-exl2-conversion-validation)** — Toolchain: fix Qwen3_5MoeForC architecture bugs, convert to EXL2, apply mixed quantization, validate with automated benchmarks
- **[auto-vault-journal](https://github.com/chessarisilvio/auto-vault-journal)** — Obsidian vault auto-updater triggered by Claude Code Stop hook; Sonnet for structured files, freellmapi for narrative journal entries
- **[voice-dictate](https://github.com/chessarisilvio/voice-dictate)** — Local Whisper turbo dictation for Claude Code (hold Space in terminal) — replaces built-in voice mode, optimized for Italian

### AI Infrastructure & Orchestration

- **[openclaw-ai-gateway](https://github.com/chessarisilvio/openclaw-ai-gateway)** — Self-hosted Ollama gateway (Node.js); routing, caching, multi-model/multi-user API layer for local LLM stack
- **[ai-gateway-prod-alternatives](https://github.com/chessarisilvio/ai-gateway-prod-alternatives)** — Technical analysis of 10 production-grade alternatives to LiteLLM, evaluated for consumer GPU constraints (P40 24GB + RTX 3050 8GB, 20GB RAM)
- **[ai-dashboard](https://github.com/chessarisilvio/ai-dashboard)** — Local monitoring dashboard (:9190): GPU/VRAM/tok-s panels, systemd services overview, unified security scanner, AGENDA.md integration
- **[automazione-bootwatchdog-ai](https://github.com/chessarisilvio/automazione-bootwatchdog-ai)** — Watchdog for llama-stack: monitors VRAM & token-rate, auto-restart via systemd, Telegram anomaly notifications
- **[secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault)** — Secure archive for LLM conversation contexts with encrypted storage
- **[reddit-monitor-ai-ideas](https://github.com/chessarisilvio/reddit-monitor-ai-ideas)** — Automated AI/tech subreddit monitor → filtered ideas to AGENDA.md via 3h systemd timer
- **[megatool](https://github.com/chessarisilvio/megatool)** — OSINT toolkit: C++ core + Flask web app (:7788) + AI photo analysis pipeline
  - **[offline-exifgps-geotagging](https://github.com/chessarisilvio/offline-exifgps-geotagging)** — Offline EXIF/GPS extraction with local reverse geocoding database

### Tools & Automation

- **[benchmark-gguf-p40-rtx3050](https://github.com/chessarisilvio/benchmark-gguf-p40-rtx3050)** — Automated GGUF benchmarking on Tesla P40 + RTX 3050 with auto-generated performance reports
- **[ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard)** — Physical dashboard: Arduino R4 WiFi + ESP32 + OLED, MQTT/Tailscale, displays P40/3050 VRAM/tok-s/uptime, voice control via ESP32
- **[ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller)** — ESP32 hardware controller: rotary encoder + OLED for local AI model selection, outputs via HID or OpenClaw gateway

### Embedded & Hardware

- **[controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32)** — Proactive thermal fan controller (ESP32) with predictive PID using temperature sensors
- **[thermalright-lcd-hid](https://github.com/chessarisilvio/thermalright-lcd-hid)** — Custom HID LCD driver for Thermalright display showing real-time temperatures
- **[videostudio-ai-spot](https://github.com/chessarisilvio/videostudio-ai-spot)** — Spot AI generator (:9195): LLM storyboard → Higgsfield video clips, prompt library, HTML/TypeScript frontend + Python backend
- **[bot-short-telegram-ai](https://github.com/chessarisilvio/bot-short-telegram-ai)** — Telegram AI graphic bot with SVG generation pipeline

---

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=default&hide_title=true&hide_border=true&card_width=500)

</div>