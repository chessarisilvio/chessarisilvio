<h1 align="center">Silvio Chessari</h1>

<p align="center">
LLM inference researcher — speculative decoding, MoE routing, GGUF quantization on unsupported GPU hardware.
<br>
Self-built AI infrastructure on consumer/datacenter GPUs. Embedded & automation systems.
</p>

<table>
<tr>
<td width="33%" align="center"><strong>Languages</strong><br>C++ · Python · CUDA · Bash · SystemVerilog</td>
<td width="33%" align="center"><strong>Compute</strong><br>llama.cpp · Ollama · vLLM · EXL2 · GGUF</td>
<td width="33%" align="center"><strong>Embedded</strong><br>ESP32 · Arduino R4 WiFi · MQTT HID-dashboard · Tailscale</td>
</tr>
</table>

---

## LLM Research

- [benchmark-4-agent-wrappers-on-qwen3627b-llamacpp](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp) — Comparative benchmark of 4 agent wrappers on Qwen3.6‑27B via llama.cpp
- [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) — Webcam/video frame ingestion for llama.cpp multimodal inference (CMake patches + Python stub)
- [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) — Auto-fix Qwen3.5 MoE architecture, mixed-EXL2 conversion, validation benchmarks
- [auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) — Auto-download LLM checkpoints, benchmark Q4_K_M vs Q5_K_S on Tesla P40/RTX 3050, publish GGUF
- [sistema-di-benchmarking-automatizzato-per-nuovi-mo](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-mo) — Automated GGUF benchmarking suite for new models on P40 + RTX 3050 with automatic report generation

## AI Infrastructure

- [openclaw](https://github.com/chessarisilvio/openclaw) — Production AI gateway routing Ollama backends (Node.js), multi-model, multi-user
- [ai-gateway-in-prod-alternative-concrete-a-litellm](https://github.com/chessarisilvio/ai-gateway-in-prod-alternative-concrete-a-litellm) — Evaluated concrete LiteLLM alternatives for consumer GPU routing and prompt caching
- [automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) — systemd watchdog for llama-stack: VRAM monitoring, t/s anomaly detection, Telegram alerts, auto-restart
- [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) — Local monitoring dashboard (:9190): GPU stats, services, AGENDA.md, sub-task workers, unified security scanner
- [secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault) — Encrypted context archival system for LLM session continuity
- [nex2-mini-phase-twin-30b-lowvram-gguf-model](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model) — Low-VRAM GGUF model, production-ready quantized variant

## Tools & Automation

- [voice-dictate](https://github.com/chessarisilvio/voice-dictate) — Hold Space in Claude Code terminal → local Whisper turbo (GPU) transcription, replaces built-in voice mode
- [auto-vault-journal](https://github.com/chessarisilvio/auto-vault-journal) — Claude Code Stop-hook: auto-update Obsidian vault from session transcript (Sonnet + freellmapi, timer-based cleanup)
- [reddit-monitor](https://github.com/chessarisilvio/reddit-monitor) — Subreddit AI/tech scraper → AGENDA.md idea feed (3h systemd timer)
- [silvioprint-pipeline-contenuti](https://github.com/chessarisilvio/silvioprint-pipeline-contenuti) — Daily content pipeline + Telegram bot (systemd service)
- [videostudio](https://github.com/chessarisilvio/videostudio) — AI video studio (:9195): LLM storyboard → Higgsfield clips, prompt library
- [megatool](https://github.com/chessarisilvio/megatool) — OSINT suite: C++ core + Flask web app (:7788) + AI photo analysis
- [modulo-offline-exifgps-geotagging-per-megatool](https://github.com/chessarisilvio/modulo-offline-exifgps-geotagging-per-megatool) — Offline EXIF/GPS extraction + reverse geocoding via local geographic databases

## Embedded & Hardware

- [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) — Arduino R4 WiFi + ESP32 LCD dashboard: P40/3050 VRAM, tok/s, uptime via MQTT/Tailscale
- [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) — ESP32 rotary encoder + OLED: physical local-AI model selector, HID gateway integration
- [controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) — Proactive thermal fan controller with sensor feedback loop
- [digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd) — Thermalright LCD temperature display via HID interface

---

<p align="center"><img src="https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=default&hide_title=true&hide_border=true" /></p>