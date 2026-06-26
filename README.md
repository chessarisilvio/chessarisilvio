<h1 align="center">Silvio Chessari</h1>
<p align="center">
  AI infrastructure engineer & LLM systems researcher. Building local inference stacks on consumer/datacenter GPUs, embedded hardware, and automated pipelines.
</p>

## 🛠️ Stack

| Domain | Technologies |
|---|---|
| **LLM Inference** | llama.cpp, GGUF, EXL2, speculative decoding, MTP, MoE routing, Ollama |
| **GPU Compute** | Tesla P40 (sm_61), RTX 3050 (sm_86), CUDA workarounds, VRAM-constrained optimization |
| **Languages** | Python, C/C++, Bash, JavaScript |
| **Infra & Ops** | systemd, Docker, Tailscale, MQTT, Node.js, Flask, GitHub Pages CI |
| **Embedded** | ESP32, Arduino R4 WiFi, HID, OLED (SSD1306), MQTT |
| **Tools** | Whisper turbo, Qwen, LiteLLM alternatives, llama-stack, voice coding |

## 📁 Projects

### LLM Research

- [auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) — Automated pipeline: download LLM checkpoints → benchmark on P40/3050 → select best GGUF quant point (Q4_K_M / Q5_K_S) → produce production-ready GGUF + Obsidian docs.
- [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) — Toolchain fixing Qwen3_5MoeForC arch → automated EXL2 conversion → mixed quantization → benchmark validation via C++ core + Python CLI wrapper.
- [benchmark-4-agent-wrappers-on-qwen3627b-llamacpp](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp) — Comparative benchmark of 4 agent wrappers running Qwen3.6-27B on llama.cpp.
- [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) — Video input support for llama.cpp (mtmd): CMake option `LLAMA_VIDEO_INPUT`, webcam/frame capture stubs, Python example script.
- [secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault) — Encrypted archive for LLM conversation contexts; secure retrieval and storage.
- [nex2-mini-phase-twin-30b-lowvram-gguf-model](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model) — Low-VRAM 30B parameter GGUF model optimized for 24GB/8GB deployments.

### AI Infrastructure

- [ai-gateway-in-prod-alternative-concrete-a-litellm](https://github.com/chessarisilvio/ai-gateway-in-prod-alternative-concrete-a-litellm) — Production AI gateway for consumer GPUs: analyzed 10 LiteLLM alternatives; prompt/response caching, multi-model routing, OpenAI-compatible API, Docker deploy on P40+3050.
- [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) — Local monitoring dashboard (`:9190`): GPU stats, services, system health, sprint board, unified security scan, personal AI ideas pipeline.
- [automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) — Advanced watchdog for llama-stack: process/VRAM/tps monitoring, Telegram anomaly alerts, systemd auto-restart.

### Tools & Automation

- [voice-dictate](https://github.com/chessarisilvio/voice-dictate) — Hold Space in Claude Code → local Whisper turbo GPU transcription, replacing built-in voice mode for improved Italian accuracy.
- [reddit-monitor](https://github.com/chessarisilvio/reddit-monitor) — Subreddit monitor (AI/tech) → auto-populates AGENDA.md with trending ideas on a 3h timer.
- [openclaw](https://github.com/chessarisilvio/openclaw) — Ollama API gateway in Node.js for local LLM orchestration.
- [megatool](https://github.com/chessarisilvio/megatool) — OSINT suite in C++ with Flask web app (`:7788`) and AI photo analysis.
- [modulo-offline-exifgps-geotagging-per-megatool](https://github.com/chessarisilvio/modulo-offline-exifgps-geotagging-per-megatool) — Offline EXIF/GPS extraction + reverse geocoding with local geographic databases.

### Embedded & Hardware

- [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) — Physical dashboard: Arduino R4 WiFi + LCD showing P40/3050 status (VRAM, tok/s, uptime), ESP32 voice commands via MQTT/Tailscale.
- [controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) — Proactive thermal controller on ESP32: sensor-driven fan curve logic with predictive adjustments.
- [digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd) — Thermalright temperature LCD display via HID interface.
- [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) — ESP32 physical model selector: rotary encoder + OLED SSD1306 + HID commands to switch local AI models.