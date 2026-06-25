<h1 align="center">Silvio Chessari</h1>
<p align="center">
  <b>LLM Inference Researcher · AI Infrastructure Engineer · Embedded Systems Developer</b><br>
  Optimizing speculative decoding, MoE routing & GGUF inference on unsupported GPUs.<br>
  Building end-to-end AI stacks, automation pipelines, and hardware-interfaced embedded systems.
</p>

## 🛠 Technical Stack

| Domain | Technologies |
|---|---|
| **LLM Inference** | llama.cpp, GGUF, EXL2, speculative decoding, EAGLE, MTP, MoE routing, Qwen3, Ollama |
| **GPU Compute** | Tesla P40 (sm_61, 24 GB), RTX 3050 (8 GB), CUDA workarounds, VRAM-constrained inference |
| **AI Infrastructure** | LiteLLM alternatives, AI gateways, model routing, prompt/response caching, Docker |
| **Automation** | systemd timers, watchdog scripts, CI pipelines, Telegram bots, Reddit monitoring |
| **Embedded** | ESP32, Arduino R4 WiFi, MQTT, Tailscale, HID, OLED/EXIF/GPS geotagging |
| **Languages** | Python, C/C++, Bash, JavaScript |
| **Tools** | CMake, Flask, Node.js, Git, GitHub Pages, OSINT |

## 🔬 LLM Research

- [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) — Toolchain automating Qwen3_5MoeForC architecture fix, EXL2 conversion, mixed quantization, and benchmark validation.
- [auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) — Automated pipeline: download checkpoints → benchmark on P40/RTX 3050 → evaluate Q4_K_M vs Q5_K_S → produce production GGUF files.
- [benchmark-4-agent-wrappers-on-qwen3627b-llamacpp](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp) — Comparative benchmark of four agent wrappers on Qwen3.6-27B via llama.cpp.
- [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) — Video input support for llama.cpp: CMake integration, video frame stubs, Python demo script.
- [sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf) — Automated GGUF benchmarking on P40 and RTX 3050 with auto-generated reports.
- [nex2-mini-phase-twin-30b-lowvram-gguf-model](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model) — Low-VRAM GGUF model optimized for consumer/datacenter GPU deployment.
- [secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault) — Encrypted archive for persistent LLM context storage and retrieval.

## 🖥 AI Infrastructure

- [ai-gateway-in-prod-alternative-concrete-a-litellm](https://github.com/chessarisilvio/ai-gateway-in-prod-alternative-concrete-a-litellm) — Evaluation of 10 LiteLLM alternatives for local AI gateways on consumer NVIDIA hardware with OpenAI-compatible API.
- [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) — Local monitoring dashboard (:9190): GPU panels, services, AGENDA.md, worker sub-tasks, unified security scanner.
- [openclaw](https://github.com/chessarisilvio/openclaw) — Ollama gateway with Node.js orchestration for multi-model routing.
- [automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) — Advanced watchdog for llama-stack: VRAM monitoring, token-rate anomaly detection, Telegram alerts, systemd auto-restart.

## ⚙️ Tools & Automation

- [voice-dictate](https://github.com/chessarisilvio/voice-dictate) — Local Whisper turbo dictation for Claude Code via hold-to-speak, replacing integrated voice mode for Italian.
- [reddit-monitor](https://github.com/chessarisilvio/reddit-monitor) — Subreddit AI/tech monitor → AGENDA.md idea generation, 3-hour timer cycle.
- [megatool](https://github.com/chessarisilvio/megatool) — OSINT toolkit: C++ core, Flask web app (:7788), AI photo analysis pipeline.
- [modulo-offline-exifgps-geotagging-per-megatool](https://github.com/chessarisilvio/modulo-offline-exifgps-geotagging-per-megatool) — Offline EXIF/GPS extraction with local geographic database and reverse geocoding.
- [videostudio](https://github.com/chessarisilvio/videostudio) — Spot AI from photos: LLM storyboard generation + Higgsfield clip assembly, Flask backend (:9195).
- [automazione-systemd-timer-per-html-minification-gi](https://github.com/chessarisilvio/automazione-systemd-timer-per-html-minification-gi) — Automated HTML minification and GitHub Pages deployment via systemd timer.

## 📡 Embedded & Hardware

- [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) — Physical dashboard: Arduino R4 WiFi + LCD showing P40/3050 status (VRAM, tok/s, uptime), ESP32 voice commands via MQTT/Tailscale.
- [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) — ESP32-based physical AI model selector: rotary encoder navigation, OLED feedback, HID commands to OpenClaw gateway.
- [controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) — Proactive thermal fan controller on ESP32 with multi-sensor input.
- [digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd) — HID-driven LCD temperature display via Thermalright hardware interface.

---

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=default&hide_title=true&count_private=true" alt="GitHub Stats" />
</p>