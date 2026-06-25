<h1 align="center">🧠 Silvio Chessari</h1>
<p align="center">
  <strong>ML Systems Researcher & AI Infrastructure Engineer</strong><br>
Speculative decoding, MoE routing, and LLM inference on unsupported GPUs.<br>
Building end-to-end AI stacks from llama.cpp patches to ESP32 hardware controllers.
</p>

## 🛠 Technical Stack

| Domain | Technologies |
|---|---|
| LLM Inference | llama.cpp, GGUF, EXL2, speculative decoding, MTP, EAGLE, MoE expert routing, Qwen3, Whisper |
| GPU Compute | NVIDIA Tesla P40 (sm_61, 24 GB), RTX 3050, CUDA version workarounds, VRAM-optimized quant stacks |
| Quantization | Q4_K_M, Q5_K_S, mixed-precision EXL2, automated GGUF pipelines |
| Automation | systemd timers, watchdog daemons, Telegram bots, cron-orchestrated benchmarking |
| Embedded | ESP32, Arduino R4 WiFi, MQTT, Tailscale, HID, OLED/SSD1306, thermal sensors, rotary encoders |
| Backend | Python, C++, Node.js, Flask, Ollama gateway, CMake |
| DevOps | GitHub Pages auto-deploy, OSINT toolchain, EXIF/GPS offline geocoding |

## 🔬 LLM Inference & Research

[automated-gguf-benchmarking-pipeline](https://github.com/chessarisilvio/automated-gguf-benchmarking-pipeline) — Automated pipeline: download new LLM checkpoints, benchmark GGUF variants (Q4_K_M / Q5_K_S) on Tesla P40 and RTX 3050, auto-generate production-ready GGUF files with Obsidian vault docs updated.

[benchmark-agent-wrappers-qwen3627b-llamacpp](https://github.com/chessarisilvio/benchmark-agent-wrappers-qwen3627b-llamacpp) — Comparative benchmark of four agent wrappers (Pi, OpenCode, Hermes, Qwen-Code) on Qwen3.6-27B via llama.cpp; measures latency, VRAM draw, and output quality on orbital-simulation prompts.

[automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) — Toolchain automating Qwen3_5MoeForC architecture fix, EXL2 checkpoint conversion, mixed-precision quantization, and validation benchmarks; C++ core with Python CLI orchestration.

[add-video-input-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-to-llamacpp-mtmd) — Adds video input support to llama.cpp (mtmd): webcam/file frame acquisition piped to LLM inference via CMake `LLAMA_VIDEO_INPUT` flag and Python demo script.

[auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) — Automated GGUF quantization pipeline: downloads checkpoints, runs rapid benchmarks on P40/3050, evaluates optimal quantization cutpoints, ships ready-to-serve GGUFs.

[nex2-mini-phase-twin-30b-lowvram-gguf-model](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model) — Low-VRAM 30B parameter GGUF model optimized for sub-24 GB GPU deployment with phase-twin architecture.

[whisper-custom-bias-local](https://github.com/chessarisilvio/whisper-custom-bias-local) — Custom bias injection for locally-run Whisper; targets Italian language transcription gaps with domain-specific vocabulary weighting.

## 🏗 AI Infrastructure

[ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) — Local monitoring dashboard on `:9190`: GPU telemetry, systemd services, sprint/agenda panels, unified security scanner, task worker; AGENDA.md aggregates ideas from 35B local model.

[openclaw](https://github.com/chessarisilvio/openclaw) — Ollama API gateway on Node.js; central model-serving bus connecting dashboards, agents, and embedded controllers.

[automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) — Advanced watchdog for `llama-stack` service: monitors process state, VRAM footprint, tok/s; triggers systemd restarts and Telegram anomaly alerts.

[secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault) — Encrypted local archive for LLM session contexts, prompts, and retrieval-augmented grounding data.

[bot-short](https://github.com/chessarisilvio/bot-short) — Telegram AI graphics bot; generates SVG pipelines from LLM prompts, renders and delivers in-chat.

[silvioprint](https://github.com/chessarisilvio/silvioprint) — Telegram content-delivery bot backed by systemd service; manages scheduled posts, image queues, and subscriber lists.

[silvioPrint-webshop](https://github.com/chessarisilvio/silvioPrint-webshop) — Static e-commerce site (HTML/CSS/JS) for motorcycle graphic kits; no framework, zero dependencies.

[pipeline-frame-interpolation-offline-mockup](https://github.com/chessarisilvio/pipeline-frame-interpolation-offline-mockup) — Geometric warp pipeline (OpenCV) applying motorcycle graphics to real photos without generative AI; perspective-correct, batch-mode.

[megatool](https://github.com/chessarisilvio/megatool) — OSINT suite in C++ with Flask web UI on `:7788`; returns AI-analyzed photo intelligence with offline EXIF/GPS extraction.

[modulo-offline-exifgps-geotagging-per-megatool](https://github.com/chessarisilvio/modulo-offline-exifgps-geotagging-per-megatool) — Offline EXIF/GPS metadata extraction + reverse geocoding using local geographic databases; no external API calls.

[reddit-monitor](https://github.com/chessarisilvio/reddit-monitor) — Subreddit tracker (AI/tech) on a 3-hour timer; scrapes posts, generates candidate ideas into AGENDA.md.

[videostudio](https://github.com/chessarisilvio/videostudio) — Storyboard generation from photos via LLM + Higgsfield clip recombination; served on `:9195` with prompt library backend.

## ⚙️ Tools & Automation

[systemd-html-minify-github-pages](https://github.com/chessarisilvio/systemd-html-minify-github-pages) — systemd timer triggering HTML minification (comments, whitespace, inline CSS/JS) and automatic GitHub Pages deploy; zero-touch static site updates.

## 📡 Embedded & Hardware

[ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) — Physical dashboard: Arduino R4 WiFi + LCD shows P40/3050 status (VRAM, tok/s, uptime); ESP32 handles voice commands via MQTT/Tailscale bound to OpenClaw gateway.

[ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) — ESP32-based hardware model selector: rotary encoder navigation, OLED SSD1306 feedback, HID/keyboard emulation switching local LLM models through OpenClaw.

[controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) — Proactive thermal fan controller on ESP32; PID-driven PWM from multi-zone sensor array with predictive ramp-up.

[thermalright-lcd-hid](https://github.com/chessarisilvio/thermalright-lcd-hid) — Thermalright LCD temperature display driven by HID reports; real-time GPU thermals on physical panel.

---

<p align="center"><img src="https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=default&hide_title=true" height="165"> <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=chessarisilvio&layout=compact&theme=default&hide_title=true" height="165"></p>