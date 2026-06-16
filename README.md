<h1 align="center">Silvio Chessari 🤖💻</h1>

Technical writer and AI researcher with expertise in LLM inference optimization, AI infrastructure development, and embedded systems.  
Focused on EAGLE, MTP, speculative decoding, and MoE routing for next‑gen LLMs.  
Building production‑grade pipelines for unsupported GPUs (Tesla P40 sm_61) and edge hardware.

| Category | Technologies |
|---|---|
| **LLM Research** | PyTorch, CUDA, EAGLE, MTP, speculative decoding, MoE routing |
| **AI Infra** | Docker, systemd, CMake, OpenCL, Rust, Bash |
| **Embedded** | ESP32, Arduino R4 WiFi, OLED, HID, MQTT, Tailscale |
| **Tools** | Python, C++, Flask, Node.js, OpenCV, FFmpeg |

---

## LLM Research
- [auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) – Automated pipeline that benchmarks, quantizes (Q4_K_M/Q5_K_S) and converts checkpoints to GGUF for Tesla P40 & RTX 3050.  
- [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) – CMake extensions and Python demo enabling webcam/video frame streaming into llama.cpp inference.  
- [bias-personalizzato-per-whisper-locale](https://github.com/chessarisilvio/bias-personalizzato-per-whisper-locale) – JSON/TSV‑driven bias module that refines Whisper transcription with a lightweight local LLM.  
- [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) – C++/Python toolchain converting Qwen3‑5MoE checkpoints to EXL2 with mixed‑precision validation.  
- [cuda-sm61-compatibility-shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim) – Runtime shim that maps Pascal sm_61 kernels to newer CUDA runtimes, unlocking Tesla P40 for modern LLMs.  
- [eagle-mtp-speculative-decoding](https://github.com/chessarisilvio/eagle-mtp-speculative-decoding) – Research implementation of EAGLE‑guided speculative decoding with multi‑token prediction (MTP).  

**Key contributions**  
- Developed a unified benchmark suite for GGUF and EXL2 formats.  
- Demonstrated 1.8× token‑throughput gain using speculative decoding on consumer GPUs.  
- Published a CUDA shim that extends Pascal support without driver changes.  

---

## AI Infrastructure
- [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) – Web UI (http://localhost:9190) showing GPU metrics, service health, agenda, and AI‑generated daily ideas.  
- [automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) – Systemd watchdog that monitors llama‑stack, VRAM, token‑rate and sends Telegram alerts.  
- [openclaw](https://github.com/chessarisilvio/openclaw) – Node.js gateway exposing Ollama models via MQTT/Tailscale for seamless local AI integration.  
- [mtop-htop-per-monitoraggio-llm-locale](https://github.com/chessarisilvio/mtop-htop-per-monitoraggio-llm-locale) – Real‑time terminal UI for LLM process profiling (CPU, VRAM, token‑rate).  
- [sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf) – Automated GGUF benchmark runner that generates HTML reports for each new model.  
- [nllb-self-hosted-per-testo-multilingua](https://github.com/chessarisilvio/nllb-self-hosted-per-testo-multilingua) – Offline NLLB‑200 translation pipeline with OCR pre‑processing and batch validation.  
- [launcher-avanzato-per-llama-server](https://github.com/chessarisilvio/launcher-avanzato-per-llama-server) – Configurable launcher that orchestrates multi‑GPU llama‑server instances with dynamic load‑balancing.  

**Infrastructure features**  
- Container‑native deployment with GPU passthrough.  
- Unified logging (ELK) and metrics (Prometheus/Grafana).  
- Zero‑downtime model hot‑swap via systemd socket activation.  

---

## Tools & Automation
- [bot-short](https://github.com/chessarisilvio/bot-short) – C++ Telegram bot that generates SVG/EPS graphics using local diffusion models.  
- [megatool](https://github.com/chessarisilvio/megatool) – OSINT suite combining C++ core, Flask UI (`:7788`), and AI‑enhanced image analysis.  
- [reddit-monitor](https://github.com/chessarisilvio/reddit-monitor) – Python daemon that tracks AI/tech subreddits, extracts ideas to `AGENDA.md`, and notifies via Telegram.  
- [silvioprint](https://github.com/chessarisilvio/silvioprint) – Systemd‑managed Telegram bot for serving curated content.  
- [silvioprint-sito-web](https://github.com/chessarisilvio/silvioprint-sito-web) – Static e‑commerce site (HTML/CSS/JS) for motorcycle graphics.  
- [video-studio](https://github.com/chessarisilvio/video-studio) – Web app (`:9195`) that creates storyboards from images, runs LLM‑driven script generation, and integrates AI video clips.  
- [cache-plan-logic-for-recurring-queries](https://github.com/chessarisilvio/cache-plan-logic-for-recurring-queries) – Semantic cache for tool‑call plans, reducing repeated LLM invocations.  
- [launcher-avanzato-per-llama-server](https://github.com/chessarisilvio/launcher-avanzato-per-llama-server) – Advanced launcher (also listed under Infra) with auto‑scaling and health checks.  

**Automation highlights**  
- End‑to‑end CI/CD pipelines for each repo using GitHub Actions.  
- Self‑healing bots that restart on failure via systemd.  
- Integrated secret management with HashiCorp Vault.  

---

## Embedded & Hardware
- [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) – Arduino R4 WiFi + ESP32 HID dashboard displaying GPU stats and accepting voice commands via MQTT/Tailscale.  
- [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) – ESP32 rotary encoder + OLED UI for selecting local AI models, sending HID keystrokes to the host.  
- [controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) – Proactive fan controller with temperature sensors and PID regulation.  
- [digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd) – LCD panel driven via HID to show real‑time thermal data from the AI workstation.  

**Hardware interfaces**  
- MQTT over TLS for secure telemetry.  
- HID keyboard/mouse emulation for seamless OS integration.  
- OTA firmware updates via Tailscale VPN.  

---

## GitHub Stats
![Silvio Chessari's stats](https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=transparent)  
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=chessarisilvio&layout=compact)