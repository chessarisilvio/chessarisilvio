<h1 align="center">Silvio Chessari</h1>
<p align="center">
  <b>LLM Inference Researcher · AI Infrastructure Engineer · Embedded Systems Developer</b>
</p>
<p align="center">
  Optimizing inference on unsupported hardware. Building local AI stacks from silicon up.
</p>

---

## 🛠 Technical Stack

| Domain | Technologies |
|---|---|
| **LLM Inference** | llama.cpp, GGUF, EXL2, speculative decoding, EAGLE, MTP, MoE routing |
| **GPU Compute** | Tesla P40 (sm_61, 24GB), RTX 3050 (8GB), CUDA workarounds, VRAM-constrained inference |
| **AI Infrastructure** | Ollama, LiteLLM alternatives, OpenClaw gateway, multi-model routing, prompt caching |
| **Embedded** | ESP32, Arduino R4 WiFi, MQTT, Tailscale, HID, OLED/SSD1306, thermal control |
| **Automation** | systemd timers, Claude Code hooks, Telegram bots, Python/Bash pipelines |
| **OSINT & Tools** | C++17, Flask, Node.js, reverse geocoding, EXIF/GPS extraction |

---

## 🔬 LLM Research

- [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) — Toolchain for Qwen3_5MoeForC architecture fix, EXL2 conversion, mixed quantization, and benchmark validation.
- [auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) — Automated GGUF quantization pipeline: download checkpoints, benchmark on P40/3050, select optimal Q4_K_M vs Q5_K_S, update vault docs.
- [benchmark-4-agent-wrappers-on-qwen3627b-llamacpp](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp) — Comparative benchmark of four agent wrappers on Qwen3.6-27B via llama.cpp.
- [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) — Video input support for llama.cpp: webcam/file frame acquisition, CMake integration, Python demo.
- [sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf) — Automated GGUF benchmarking on P40 and RTX 3050 with auto-generated reports.
- [nex2-mini-phase-twin-30b-lowvram-gguf-model](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model) — Low-VRAM GGUF model optimized for 24GB consumer/datacenter GPUs.

## 🖥 AI Infrastructure

- [ai-gateway-in-prod-alternative-concrete-a-litellm](https://github.com/chessarisilvio/ai-gateway-in-prod-alternative-concrete-a-litellm) — Analysis of 10 LiteLLM alternatives for local AI gateways on consumer NVIDIA hardware with OpenAI-compatible API.
- [openclaw](https://github.com/chessarisilvio/openclaw) — Ollama gateway with Node.js orchestration for multi-model local serving.
- [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) — Local monitoring dashboard (:9190): GPU panels, services, AGENDA.md, security scanner, idea generator.
- [automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) — Advanced watchdog for llama-stack: VRAM/token-rate monitoring, Telegram alerts, systemd auto-restart.
- [secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault) — Encrypted archive for LLM conversation contexts and retrieval.

## ⚙️ Tools & Automation

- [auto-vault-journal](https://github.com/chessarisilvio/auto-vault-journal) — Claude Code Stop hook: auto-updates Obsidian vault via Sonnet, narrative journal via freellmapi, 72h cleanup timer.
- [voice-dictate](https://github.com/chessarisilvio/voice-dictate) — Local Whisper turbo GPU dictation for Claude Code terminal (hold Space), replacing integrated voice mode.
- [reddit-monitor](https://github.com/chessarisilvio/reddit-monitor) — Subreddit AI/tech monitor → AGENDA.md idea pipeline, 3h timer.
- [megatool](https://github.com/chessarisilvio/megatool) — OSINT suite: C++ core + Flask web app (:7788) + AI photo analysis.
- [modulo-offline-exifgps-geotagging-per-megatool](https://github.com/chessarisilvio/modulo-offline-exifgps-geotagging-per-megatool) — Offline EXIF/GPS extraction with local geographic database and reverse geocoding.
- [videostudio](https://github.com/chessarisilvio/videostudio) — Spot AI from photos: LLM storyboard generation + Higgsfield clip compositing, Flask backend (:9195).

## 📡 Embedded & Hardware

- [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) — Arduino R4 WiFi + ESP32 hardware dashboard: P40/3050 status (VRAM, tok/s, uptime), voice commands via MQTT/Tailscale.
- [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) — ESP32 physical controller: rotary encoder + OLED SSD1306 + HID for local AI model selection via OpenClaw gateway.
- [controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) — Proactive thermal fan control on ESP32 with sensor feedback loop.
- [digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd) — Thermalright LCD temperature display via HID interface.

---

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=default&hide_title=true&count_private=true)

</div>