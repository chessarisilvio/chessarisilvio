# <h1 style="text-align:center;">🚀 Silvio Chessari – AI & Embedded Engineer</h1>

## 3‑line Technical Bio  
- Deep‑learning inference researcher focused on speculative decoding, MoE routing, and EAGLE‑style instruction tuning.  
- Creator of a self‑built AI stack that runs LLMs on unsupported consumer GPUs (Tesla P40 sm_61, RTX 3050) via custom CUDA shims and runtime patches.  
- Embedded systems specialist delivering hardware dashboards and real‑time thermal control on ESP32, Arduino R4, and HID peripherals.

## Compact Stack Table  

| Languages / Frameworks | Tools / Hardware |
|------------------------|------------------|
| C++, Python, Rust, Bash | NVIDIA P40 sm_61, RTX 3050, ESP32‑DevKit, Arduino R4 WiFi |
| CMake, OpenCV, Flask, Node.js | Tailscale, MQTT, OpenClaw, NVIDIA CUDA 12 |
| HuggingFace Transformers, llama.cpp | GGUF quantization, EXL2 conversion, Whisper‑local, MoE routing libraries |
| Docker, systemd, GitHub Actions | CI pipelines, watchdog scripts, telemetry dashboards |

## LLM Research  

- **[add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd)** – Integrates webcam/video frame capture into llama.cpp for real‑time multimodal inference.  
- **[auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf)** – Automates checkpoint download, GPU‑benchmarks on P40/RTX3050, and GGUF quantization tuning (Q4_K_M vs Q5_K_S).  
- **[automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline)** – C++/Python toolchain that converts Qwen models to EXL2, applies mixed‑precision quantization, and validates throughput.  
- **[bias-personalizzato-per-whisper-locale](https://github.com/chessarisilvio/bias-personalizzato-per-whisper-locale)** – Implements a JSON/TSV bias loader for Whisper, coupled with a local GGUF LLM for contextual post‑processing.  

## AI Infrastructure  

- **[sistema-di-benchmarking-automatizzato-per-nuovi-mo](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-mo)** – End‑to‑end benchmarking of new GGUF models on P40/RTX3050, auto‑generated performance reports.  
- **[automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato)** – Advanced watchdog for llama‑stack: monitors VRAM, token/s, and triggers Telegram alerts and systemd restarts.  
- **[openclaw](https://github.com/chessarisilvio/openclaw)** – Node.js gateway exposing Ollama locally over MQTT/Tailscale, enabling secure AI model invocation.  
- **[cuda-sm61-compatibility-shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim)** – CUDA compatibility layer that patches sm_61 binaries to run on newer CUDA toolchains, unlocking legacy Pascal GPUs for deep‑learning workloads.  

## Tools & Automation  

- **[ai-dashboard](https://github.com/chessarisilvio/ai-dashboard)** – Web UI (http://localhost:9190) visualizing GPU stats, services, and an agenda system with auto‑generated idea prompts.  
- **[reddit-monitor](https://github.com/chessarisilvio/reddit-monitor)** – Periodic crawler of tech subreddits, aggregates AI trends, and updates AGENDA.md.  
- **[silvioprint](https://github.com/chessarisilvio/silvioprint)** – Telegram bot that publishes curated graphic content from a static e‑commerce site.  
- **[megatool](https://github.com/chessarisilvio/megatool)** – C++ OSINT engine with Flask front‑end (port 7788) and AI‑powered photo analysis.  
- **[bot-short](https://github.com/chessarisilvio/bot-short)** – C++ Telegram bot that renders AI‑generated SVG/EPS graphics on demand.  

## Embedded & Hardware  

- **[ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard)** – Arduino R4 WiFi + ESP32 LCD panel displaying P40/RTX3050 metrics, voice‑controlled via MQTT/Tailscale.  
- **[ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller)** – ESP32‑based rotary encoder and OLED selector that issues HID commands to switch local LLM models.  
- **[controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32)** – Proactive fan control for ESP32‑powered enclosures using sensor‑driven PID loops.  
- **[digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd)** – HID temperature display on a 16×2 LCD, driven by microcontroller readings and local AI telemetry.  
- **[video-studio](https://github.com/chessarisilvio/video-studio)** – Web UI (port 9195) that stitches AI‑generated storyboard clips and embeds them into video sequences, leveraging a local LLM prompt library.  

---

### GitHub Stats  

![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=chessarisilvio&theme=radical&hide_border=true)  
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=chessarisilvio&langs_count=8&theme=radical&hide_border=true)  
![Repo Count](https://github-readme-stats.vercel.app/api?username=chessarisilvio&count_private=true&include_all_commits=true&show_icons=true&theme=radical)

---