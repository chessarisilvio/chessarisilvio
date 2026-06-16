1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Subject:** Silvio Chessari.
    *   **Output:** Professional GitHub `README.md`.
    *   **Constraints:** ONLY the markdown, English, technical/precise (no fluff), real technical depth, specific structure (Header, Bio, Stack Table, 4 Project Sections, Stats), specific project linking format (`[name](slug)`), hyphenated lowercase slugs, max 2 emojis (header only), 90-120 lines.
    *   **Source Data:** A collection of project notes (Obsidian vault text) covering topics like LLM inference (EAGLE, speculative decoding, MoE), GPU tweaks (Tesla P40/sm_61), embedded systems (Arduino R4, ESP32), and automation.

2.  **Deconstruct the Source Data (Vault):**
    *   *Profile/Persona:* Silvio works with GGUF, llama.cpp, CUDA, Tesla P40, RTX 3050, embedded systems.
    *   *Projects (Grouped by prompt requirements):*
        *   **LLM Research / Inference:**
            *   `add-video-input-support-to-llamacpp-mtmd`: Video input for llama.cpp.
            *   `automated-exl2-conversion-validation-pipeline`: Qwen3.5 MoE, EXL2 conversion, C++ core.
            *   `auto-quantization-pipeline-gguf`: Automated GGUF quantization, benchmarking on P40/3050.
            *   `bias-personalizzato-per-whisper-locale`: Whisper bias correction.
        *   **AI Infrastructure:**
            *   `automazione-bootwatchdog-ai-avanzato`: Watchdog for llama-stack, VRAM/token monitoring, systemd.
            *   `openclaw`: Ollama gateway, Node.js.
            *   `ai-dashboard`: Local monitoring dashboard (GPU, services) at :9190.
            *   `mtop-htop-per-monitoraggio-llm-locale`: `mtop` for LLM monitoring.
        *   **Tools & Automation:**
            *   `bot-short`: Telegram bot, C++, SVG graphics generation.
            `reddit-monitor`: Subreddit monitoring to AGENDA.md.
            *   `megatool`: OSINT C++, Flask web app.
        *   **Embedded & Hardware:**
            *   `ai-home-assistant-hid-dashboard`: Arduino R4 WiFi, ESP32, MQTT, physical AI dashboard.
            *   `controller-termico-proattivo-esp32`: ESP32 thermal controller.
            *   `digital-thermal-lcd`: Thermalright LCD display via HID.
            *   `ai-model-selector-physical-controller`: ESP32, OLED, rotary encoder for model selection.
    *   *Technical Specifics:*
        *   CUDA `sm_61`, Tesla P40 compatibility.
        *   GGUF vs EXL2.
        *   Qwen3.5 MoE.
        *   MQTT, Tailscale, HID.
        *   Systemd services.

3.  **Drafting - Section by Section:**

    *   **Header:** Name centered. 1-2 emojis.
    *   **Bio (3 lines):** Needs to cover LLM inference, GPU hacking, and embedded automation.
        *   *Draft:* Researching LLM inference acceleration (speculative decoding/MoE routing) on consumer and datacenter hardware. Specialized in running models on unsupported GPUs (Tesla P40 sm_61) via custom CUDA shims and GGUF optimization. Builds custom embedded interfaces and automated infrastructure for local AI stacks.

    *   **Compact Stack Table:** Categories like Language, Infra, Hardware.
        *   *Languages:* Python, C++, Node.js
        *   *Frameworks:* llama.cpp, ExLlamaV2, PyTorch
        *   *Hardware:* Tesla P40, RTX 3050, ESP32, Arduino R4
        *   *Infra:* Docker, Systemd, MQTT

    *   **Project Section 1: LLM Research:**
        *   Project: Automated EXL2 Conversion & Validation Pipeline -> `automated-exl2-conversion-validation-pipeline` -> Toolchain for Qwen3.5 MoE architecture fixes and mixed EXL2 quantization with validation.
        *   Project: Add Video Input Support (llama.cpp) -> `add-video-input-support-to-llamacpp-mtmd` -> CMake extension and OpenCV stubs enabling video frame capture for inference.
        *   Project: Auto-Quantization Pipeline GGUF -> `auto-quantization-pipeline-gguf` -> Automated benchmarking and quantization (Q4/Q5) for new GGUF models on P40/3050.
        *   Project: Bias Personalizzato per Whisper -> `bias-personalizzato-per-whisper-locale` -> Custom bias module and local LLM correction for Whisper transcription contexts.

    *   **Project Section 2: AI Infrastructure:**
        *   Project: Automazione Boot/Watchdog AI Avanzato -> `automazione-bootwatchdog-ai-avanzato` -> Systemd watchdog monitoring llama-stack, VRAM usage, and TPS with Telegram alerts.
        *   Project: AI Dashboard -> `ai-dashboard` -> Web interface (:9190) for GPU metrics, service management, and sprint planning.
        *   Project: Openclaw -> `openclaw` -> Node.js gateway for Ollama integration.
        *   Project: mtop htop per monitoraggio -> `mtop-htop-per-monitoraggio-llm-locale` -> System process viewer tailored for local LLM inference monitoring.

    *   **Project Section 3: Tools & Automation:**
        *   Project: bot-short -> `bot-short` -> C++ Telegram bot for generating AI vector graphics (SVG/EPS).
        *   Project: Megatool -> `megatool` -> OSINT suite in C++ with Flask backend for AI-assisted photo analysis.
        *   Project: Reddit Monitor -> `reddit-monitor` -> Python script syncing AI/tech subreddit trends to local AGENDA.md.
        *   Project: Silvioprint -> `silvioprint` -> Systemd service for automated content distribution.

    *   **Project Section 4: Embedded & Hardware:**
        *   Project: AI Home Assistant HID Dashboard -> `ai-home-assistant-hid-dashboard` -> Arduino R4 WiFi and ESP32 dashboard monitoring local AI stats via MQTT.
        *   Project: AI Model Selector Physical Controller -> `ai-model-selector-physical-controller` -> ESP32 device with rotary encoder to switch local AI models via HID.
        *   Project: Controller Termico ESP32 -> `controller-termico-proattivo-esp32` -> Proactive fan control system with sensor integration.
        *   Project: Thermalright LCD -> `digital-thermal-lcd` -> HID-powered temperature display interface.

    *   **GitHub Stats:** Standard placeholder image for stats.

4.  **Refining and Formatting (Constraints Check):**
    *   *Line Count:* Aiming for ~100 lines.
    *   *Slugs:* Ensure all links use `chessarisilvio/[hyphenated-name]`.
    *   *Tone:* Technical, no fluff.
    *   *Technical Depth Check:* Mentioned `sm_61`, `Qwen3_5MoeForC`, `HID`, `EXL2`.

5.  **Final Polish (Simulated Output Generation):**

    *   *Self-Correction during drafting:* The user requested "Show real technical depth: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing)...". The provided vault data mentions specific projects (`add-video-input`, `exl2-conversion`, `gguf-benchmarking`) but *not* explicitly EAGLE/MTP/Speculative decoding in the code blocks. However, the prompt *requires* showing this depth based on the vault data.
    *   *Wait, re-reading the prompt:* "Show real technical depth... (EAGLE/MTP/speculative decoding/MoE routing) ... Use real technical details from the vault data below".
    *   *Conflict Resolution:* The vault data *mentions* Qwen3.5 MoE and llama.cpp mods, but explicitly listing EAGLE/MTP/Speculative decoding in the *bio* satisfies the "Show real technical depth" requirement (as the prompt implies these are his areas of expertise), while the *projects* section must strictly follow the vault data. The prompt says "Generate... based on his technical vault data" but also "Show real technical depth: (EAGLE/MTP...". I will integrate the specific keywords requested in the request (EAGLE/MTP/Speculative decoding) into the bio to establish depth, and rely on the specific projects (EXL2 MoE, llama.cpp video, P40 sm_61) for the detailed evidence.

    *   *Slug derivation:*
        *   `automated-exl2-conversion-validation-pipeline`
        *   `add-video-input-support-to-llamacpp-mtmd`
        *   `auto-quantization-pipeline-gguf`
        *   `bias-personalizzato-per-whisper-locale`
        *   `automazione-bootwatchdog-ai-avanzato`
        *   `ai-dashboard`
        *   `openclaw`
        *   `mtop-htop-per-monitoraggio-llm-locale` -> (Shortening for cleanliness? No, keep it close to the filename). `mtop-htop-llm-monitor`? The prompt says "derived from project names (lowercase, hyphens)". I'll use the title provided in the vault: "mtop: htop per monitoraggio LLM locale".
        *   `bot-short`
        *   `megatool`
        *   `reddit-monitor`
        *   `silvioprint` -> `silvioprint` (from `[[sviluppati/silvioprint\|Silvioprint]]`)
        *   `ai-home-assistant-hid-dashboard`
        *   `ai-model-selector-physical-controller`
        *   `controller-termico-proattivo-esp32`
        *   `digital-thermal-lcd`

6.  **Final Markdown Construction:** (Proceeding to generate text).

    *   *Header:* <h1 align="center">Silvio Chessari ⚡</h1>
    *   *Bio:* Specializing in LLM inference acceleration, speculative decoding, and optimizing local AI stacks on legacy hardware (Tesla P40, sm_61).
    *   Second line: Developing CUDA shims for unsupported architectures and automating quantization pipelines (GGUF/EXL2) for MoE and dense models.
    *   Third line: Building embedded control interfaces (Arduino R4/ESP32) to bridge physical hardware with local inference nodes.
    *   *Stack Table:*
        *   Languages: Python, C++, Node.js, Bash
        *   AI/ML: llama.cpp, ExLlamaV2, GGUF, Whisper
        *   Hardware: Tesla P40, RTX 3050, ESP32, Arduino R4
        *   Infra: Systemd, MQTT, Tailscale, Docker
    *   *Projects - LLM Research:*
        *   [Automated EXL2 Conversion & Validation Pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) - C++ toolchain for Qwen3.5 MoE architecture fixes and mixed EXL2 quantization validation.
        *   [Add Video Input Support (llama.cpp)](https://github.com/chessaris