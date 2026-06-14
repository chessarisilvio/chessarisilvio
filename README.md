1.  **Analyze the User & Request:**
    *   **Role:** Technical Writer.
    *   **Task:** Generate a professional GitHub README.md for "Silvio Chessari".
    *   **Input Data:** A detailed "Vault" (Obsidian-like notes) containing project lists, descriptions, paths, and code snippets.
    *   **Requirements:**
        *   Output ONLY the final README.md (Markdown).
        *   No preamble, no explanation.
        *   Tone: English, technical, precise, no fluff.
        *   Key Themes: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), running LLMs on unsupported GPUs (Tesla P40 sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.
        *   Structure: Centered header -> 3-line bio -> compact stack table -> 4 project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware) -> GitHub stats.
        *   Project Link Format: `[name](https://github.com/chessarisilvio/slug)`.
        *   Slug Logic: Lowercase, hyphens.
        *   Constraints: Max 2 emojis total (header only).
        *   Length: 90–120 lines.
    *   **Persona:** Silvio Chessari (derived from data) seems to be a systems engineer / AI researcher focused on squeezing performance out of consumer and older datacenter hardware, heavily embedded, and deeply integrated into the LLM ecosystem.

2.  **Analyze the Vault Data & Extract Key Technical Details:**
    *   *Themes:* LLMs, CUDA sm_61 (Pascal), Tesla P40, RTX 3050, GGUF, EXL2, Quantization, Python, C++, Arduino R4, ESP32, MQTT, Docker, Tailscale.
    *   *Projects:*
        *   **LLM Research/Inference:**
            *   *Add video input to llama.cpp (mtmd):* CMake changes, stub video input, OpenCV Python demo.
            *   *CUDA sm_61 Compatibility Shim:* For Tesla P40 (Pascal).
            *   *Automated EXL2 Conversion & Validation Pipeline:* Fix Qwen3.5MoE, quantization, benchmarks.
            *   *Auto-Quantization Pipeline GGUF:* Benchmarking P40/3050, quant comparison.
            *   *Bias for Whisper:* Custom bias loader, local LLM correction.
        *   **AI Infrastructure:**
            *   *AI Home Assistant HID Dashboard:* Arduino R4 + ESP32, MQTT/Tailscale, monitor P40/3050 VRAM/tok/s.
            *   *mtop:* htop like for LLMs, real-time metrics.
            *   *Automazione Boot/Watchdog AI:* Monitor llama-stack, systemd, Telegram alerts.
            *   *OpenClaw:* Ollama Gateway, Node.js.
        *   **Tools & Automation:**
            *   *AI Dashboard + Agenda:* Web monitor (:9190), local 35B idea generation, AGENDA.md.
            *   *Bot-short:* C++ Telegram bot, SVG/EPS generation.
            *   *Megatool:* OSINT in C++, Flask web app, AI photo analysis.
            *   *Reddit Monitor:* AI/tech subreddit scraper, AGENDA integration.
            *   *Silvioprint:* Telegram bot for content.
        *   **Embedded & Hardware:**
            *   *AI Model Selector Physical Controller:* ESP32, rotary encoder, OLED, HID integration.
            *   *Controller Termico ESP32:* Fan control, proactive.
            *   *Digital Thermal LCD:* HID display for temps.
            *   *VideoStudio:* Spot AI, storyboard LLM, Higgsfield clips.

3.  **Drafting Content - Section by Section:**

    *   **Header:**
        *   "Silvio Chessari"
        *   "Research Engineer & Infrastructure Specialist"
        *   Icons: 🚀 ⚙️ (Two emojis max).

    *   **Bio (3 lines):**
        *   Focus on LLM inference acceleration, CUDA workarounds for legacy hardware (Tesla P40), and automated quantization pipelines.
        *   Mention integrating embedded systems with local AI stacks via MQTT/HID.
        *   Self-hosted architecture for low-latency edge computing and MoE routing optimization.

    *   **Stack Table (Compact):**
        *   Languages: C++, Python, C.
        *   AI/ML: GGUF, EXL2, llama.cpp, Ollama, Whisper.
        *   Infra: Docker, systemd, Tailscale, MQTT, Node.js.
        *   Hardware: Tesla P40 (CUDA sm_61), RTX 3050, ESP32, Arduino R4.

    *   **Project Section 1: LLM Research & Inference**
        *   1. `add-video-input-support-to-llamacpp-mtmd` -> [Add video input support to llama.cpp](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd). *Extends llama.cpp core to ingest webcam/file video via custom CMake stubs and OpenCV bridge.*
        *   2. `automated-exl2-conversion-validation-pipeline` -> [Automated EXL2 Conversion & Validation Pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline). *Toolchain for Qwen3.5MoE EXL2 conversion, mixed-precision quantization, and validation benchmarking.*
        *   3. `cuda-sm61-compatibility-shim` -> [CUDA sm_61 Compatibility Shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim). *Enables LLM inference on Pascal architecture (Tesla P40) by bypassing missing CUDA instructions.*

    *   **Project Section 2: AI Infrastructure**
        *   1. `mtop-htop-per-monitoraggio-llm-locale` -> [mtop: LLM Monitor](https://github.com/chessarisilvio/mtop-htop-per-monitoraggio-llm-locale). *Real-time TUI monitoring of local LLM inference metrics (VRAM, tokens/s, GPU load).*
        *   2. `ai-home-assistant-hid-dashboard` -> [AI Home Assistant HID Dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard). *Hardware dashboard (Arduino R4/ESP32) displaying inference state via MQTT/Tailscale.*
        *   3. `automazione-bootwatchdog-ai-avanzato` -> [AI Boot Watchdog](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato). *Systemd watchdog for llama-stack with process, VRAM, and TPS monitoring plus Telegram alerts.*

    *   **Project Section 3: Tools & Automation**
        *   1. `ai-dashboard` -> [AI Dashboard](https://github.com/chessarisilvio/ai-dashboard). *Web interface (:9190) for local stack management, automated agenda generation via 35B LLM.*
        *   2. `bot-short` -> [Bot Short](https://github.com/chessarisilvio/bot-short). *C++ Telegram bot for generating AI vector graphics and SVG pipelines.*
        *   3. `sistema-di-benchmarking-automatizzato-per-nuovi-mo` -> [Automated GGUF Benchmarking](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-mo). *Benchmarks new GGUF models on P40/RTX3050, selects optimal quantization.*

    *   **Project Section 4: Embedded & Hardware**
        *   1. `ai-model-selector-physical-controller` -> [AI Model Selector Physical Controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller). *ESP32 rotary controller + OLED for selecting local LLM models via HID emulation.*
        *   2. `controller-termico-proattivo-esp32` -> [Thermal Controller ESP32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32). *Proactive fan control and sensor monitoring for high-load inference rigs.*
        *   3. `videostudio` -> [VideoStudio](https://github.com/chessarisilvio/videostudio). *Automated storyboard generation from photos using LLM prompts and video synthesis.*

    *   **GitHub Stats Section:**
        *   Standard GitHub stats image links (using the generic `chessarisilvio` username derived from the context, or a placeholder if not verified, but the prompt implies generating the file based on *his* data, so I will assume the username is `chessarisilvio` based on the URL pattern requirement).
        *   Tech stack icons (Shields.io).

4.  **Refining and Formatting:**
    *   Check line count constraints.
    *   Ensure tone is technical (e.g., "Ingest," "Shim," "Quantization," "TPS").
    *   Verify slug generation (lowercase, hyphens).
    *   Structure with Markdown headers.
    *   Ensure distinct sections.

5.  **Draft Review against Constraints:**
    *   *No preamble?* Yes.
    *   *English?* Yes.
    *   *Real details?* Yes (Tesla P40, Pascal, sm_61, Qwen3.5MoE, GGUF, EXL2).
    *   *Structure?* Header -> Bio -> Stack -> 4 Sections -> Stats.
    *   *Max 2 emojis?* Header only.
    *   *90–120 lines?* I need to ensure enough whitespace and distinct lines to hit this range without being verbose.

6.  **Final Polish:**
    *   The bio needs to hit the "Research" aspect hard (EAGLE/MTP mentioned in prompt requirements - I need to make sure I fit that in, even if the specific files linked didn't explicitly name EAGLE, the prompt explicitly asked to "Show real technical depth: LLM inference research (EAGLE/MTP...)". I will incorporate this into the bio or a project description if it fits, or ensure the bio reflects the *capability* described in the prompt.)
    *   *Self-correction:* The prompt explicitly lists "EAGLE/MTP/speculative decoding" as required content. The vault data mentions "add-video-input... llama.cpp" and "EXL2". I will ensure the Bio covers the research intent around speculative decoding, and potentially the "mtop" or "EXL2" project description hints at this, or I'll frame the Bio strongly enough to cover the prompt's requirement for depth in those areas.

    *   *Bio Rewrite:* "Specializing in LLM inference acceleration, speculative decoding (EAGLE/MTP), and MoE routing optimization. Engineering CUDA workarounds for sm_61 architecture (Tesla P40) and building automated quantization pipelines for GGUF/EXL2 formats. Designing embedded interfaces via MQTT/HID to bridge physical hardware with local AI stacks."

    *   *Checking Slugs:*
        *   `add-video-input-support-to-llamacpp-mtmd` -> `add-video-input-support-to-llamacpp-mtmd`
        *   `automated-exl2-conversion-validation-pipeline` -> `automated-exl2-conversion-validation-pipeline`
        *   `cuda-sm61-compatibility-shim` -> `cuda-sm61-compatibility-shim`
        *   `mtop-ht