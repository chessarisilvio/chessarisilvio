- [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) C++/Python toolchain for Qwen3_5MoeForC architecture fixes and mixed-precision EXL2 conversion.
   - [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) CMake and C++ patches enabling webcam/video frame capture for multimodal llama.cpp inference.

   *(Section 2: AI Infrastructure)*
   ### 🖥️ AI Infrastructure & Gateway Systems
   - [ai-gateway-in-prod-alternative-concrete-a-litellm](https://github.com/chessarisilvio/ai-gateway-in-prod-alternative-concrete-a-litellm) Analysis and deployment of OpenAI-compatible routing gateways optimized for 24GB/8GB VRAM constraints.
   - [openclaw](https://github.com/chessarisilvio/openclaw) Node.js Ollama gateway and local AI service orchestrator.
   - [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) Real-time monitoring dashboard (`:9190`) tracking GPU metrics, token throughput, and automated AGENDA.md generation.
   - [secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault) Encrypted local storage architecture for managing LLM context windows and prompt templates.

   *(Section 3: Tools & Automation)*
   ### 🛠️ Tools & Automation
   - [auto-vault-journal](https://github.com/chessarisilvio/auto-vault-journal) Obsidian vault synchronization system triggered by Claude Code `Stop` hooks with async transcript parsing.
   - [voice-dictate](https://github.com/chessarisilvio/voice-dictate) Local Whisper `turbo` GPU integration for terminal-based voice input, bypassing native voice mode limitations.
   - [reddit-monitor](https://github.com/chessarisilvio/reddit-monitor) Automated AI/tech subreddit scraper feeding structured ideas into AGENDA.md via 3h systemd timers.
   - [automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) Systemd-based watchdog monitoring llama-stack process health, VRAM allocation, and tok/s rates with Telegram alerts.

   *(Section 4: Embedded & Hardware)*
   ### 📡 Embedded & Hardware Integration
   - [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) Arduino R4 WiFi + ESP32 HID controller displaying P40/3050 telemetry via MQTT/Tailscale.
   - [controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) Proactive thermal management firmware with dynamic fan curve adjustment and sensor fusion.
   - [digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd) HID-based LCD display driver for real-time thermalright temperature monitoring.
   - [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) ESP32 rotary encoder interface for local model switching with OLED feedback and HID command injection.

   *(GitHub Stats)*
   <div align="center">
   ![GitHub Stats](https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=dark&hide_border=true&count_private=true)
   </div>

4.  **Check Constraints:**
   - Output ONLY final README.md? Yes.
   - English, technical, precise, no fluff? Yes.
   - Show real technical depth (EAGLE/MTP, P40 sm_61, etc.)? Yes, integrated into bio and stack.
   - Structure: centered header → 3-line bio → compact stack table → 4 sections → stats? Yes.
   - Projects: `[name](url)` + 1-line desc? Yes.
   - Slugs derived from names? Yes.
   - Max 2 emojis total (header only)? I used 🔬 and ⚙️ in the header. I need to remove any other emojis. I used `🔍`, `🖥️`, `🛠️`, `📡` in section headers. I must remove those to strictly follow "Max 2 emojis total (header only)".
   - 90-120 lines total? Let's count.
     Header: 3
     Bio: 3
     Table: 6
     Section 1: 5
     Section 2: 5
     Section 3: 5
     Section 4: 5
     Stats: 3
     Total ~35 lines. I need to expand slightly to hit 90-120, or add more projects/details while keeping it tight. I'll add a few more vault projects to fill it out and ensure line count is in range. I'll also format it carefully.
     Let's count lines precisely and adjust to hit 90-120.
     I will add more projects from the vault to each section to reach ~95 lines.
     Vault projects available: `sistema-di-benchmarking-automatizzato-per-nuovi-mo`, `nex2-mini-phase-twin-30b-lowvram-gguf-model`, `bot-short`, `megatool`, `modulo-offline-exifgps-geotagging-per-megatool`, `videostudio`, `web-access-layer-per-agenti-ai-locali`, `automazione-systemd-timer-per-html-minification-gi`.
     I'll distribute them across sections.
     Let's draft carefully and count lines.

   *Revised Draft (Mental Line Count Check):*
   <div align="center">
   <h1>🔬 Silvio Chessari ⚙️</h1>
   </div>

   AI infrastructure engineer specializing in local LLM inference, speculative decoding, and heterogeneous GPU acceleration. Architect of self-hosted AI stacks running quantized MoE and dense models on unsupported datacenter silicon (Tesla P40 sm_61) and consumer RTX hardware. Embedded systems developer bridging microcontrollers, MQTT, and real-time telemetry for autonomous AI workstations.

   | Domain | Stack |
   |--------|-------|
   | **LLM Inference** | llama.cpp (MTP/EAGLE), GGUF/EXL2, CUDA 12.x,