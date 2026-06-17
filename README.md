1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Subject:** Silvio Chessari (GitHub profile README).
    *   **Source Material:** "Vault Data" provided (mix of project lists, descriptions, and Italian metadata).
    *   **Constraints:**
        *   Output *only* the README.md markdown.
        *   No preamble, no explanation.
        *   English, technical, precise, no fluff.
        *   Show real technical depth (LLM inference, CUDA hacks, embedded systems).
        *   Structure: Centered header -> 3-line technical bio -> Compact stack table -> 4 project sections -> GitHub stats.
        *   Project format: `[name](https://github.com/chessarisilvio/slug)` + 1-line description.
        *   Slugs: lowercase-hyphens.
        *   Max 2 emojis (header only).
        *   Length: 90–120 lines.
    *   **Key Tech Details to Extract:**
        *   LLM Inference: EAGLE, MTP, speculative decoding, MoE routing.
        *   Hardware unsupported: Tesla P40 (sm_61), CUDA workarounds.
        *   Self-built AI infrastructure.
        *   Embedded: Arduino R4, ESP32.

2.  **Analyze the Source Data (Vault):**
    *   *Bio/Overview:* Silvio develops low-VRAM GGUF models, benchmarking on P40/RTX3050, automated pipelines, CUDA shimming for Pascal GPUs.
    *   *Projects:*
        *   `nex2-mini-phase-twin-30b-lowvram-gguf-model`: 30B model, low-VRAM.
        *   `sistema-di-benchmarking-automatizzato-per-nuovi-mo`: GGUF benchmarking automation.
        *   `automated-exl2-conversion-validation-pipeline`: Qwen3.5 MoE fix, EXL2 conversion, mixed precision.
        *   `cuda-sm61-compatibility-shim`: Pascal (P40) support.
        *   `ai-home-assistant-hid-dashboard`: Arduino R4, ESP32, hardware monitoring.
        *   `ai-model-selector-physical-controller`: ESP32, HID control.
        *   `controller-termico-proattivo-esp32`: Thermal control.
        *   `add-video-input-support-to-llamacpp-mtmd`: Video input for llama.cpp, CMake/OpenCV.
        *   `bot-short`: C++, Telegram, SVG/AI graphics.
        *   `ai-dashboard`: Monitoring dashboard, system metrics.
        *   `automazione-bootwatchdog-ai-avanzato`: Systemd watchdog, Telegram notify.
    *   *Research/Stack:* llama-stack, Ollama (via OpenClaw), Whisper bias correction.

3.  **Drafting - Section by Section:**

    *   **Header:** Needs to be centered. Silvio Chessari.
    *   **Bio (3 lines):** Needs to hit: LLM inference, unsupported hardware (P40), infrastructure, embedded.
        *   *Draft:* Specializing in LLM inference optimization and speculative decoding on legacy hardware.
        *   *Draft:* Architected a self-hosted AI stack featuring automated GGUF/EXL2 pipelines and CUDA compatibility shims for Tesla Pascal GPUs.
        *   *Draft:* Bridging high-performance compute and embedded systems via Arduino/ESP32 controllers for physical AI interfaces.

    *   **Stack Table:** Compact.
        *   *OS:* Linux/Server.
        *   *Languages:* Python, C++, CMake.
        *   *AI/ML:* llama.cpp, ExLlamaV2, Qwen MoE, Whisper, GGUF.
        *   *Hardware:* Tesla P40, RTX 3050, Arduino R4, ESP32.

    *   **Section 1: LLM Research & Quantization**
        *   *Nex2 Model:* [Nex2 Mini Phase Twin 30B Low-VRAM Model](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model) | Optimized 30B GGUF pipeline for constrained memory environments.
        *   *Automated Pipeline:* [Automated GGUF Benchmarking System](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf) | Automated evaluation of GGUF quantization levels on P40 and RTX 3050.
        *   *EXL2 Pipeline:* [Automated EXL2 Conversion & Validation](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) | Toolchain for Qwen3.5 MoE architecture fixes and mixed-precision EXL2 export.

    *   **Section 2: AI Infrastructure & CUDA Hacks**
        *   *CUDA Shim:* [CUDA sm61 Compatibility Shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim) | Enabling modern LLM software stacks on legacy Tesla Pascal GPUs.
        *   *Watchdog:* [Advanced Boot/Watchdog Automation](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) | Systemd watchdog with VRAM/tok/s monitoring and Telegram alerts for llama-stack.
        *   *Dashboard:* [AI Dashboard & Agenda](https://github.com/chessarisilvio/ai-dashboard) | Local monitoring interface tracking GPU metrics, VRAM, and automated task scheduling.

    *   **Section 3: Tools & Automation**
        *   *Video Input:* [Add Video Input to llama.cpp (mtmd)](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) | Patching llama.cpp for webcam/video frame ingestion using OpenCV and CMake.
        *   *Whisper Bias:* [Custom Bias for Local Whisper](https://github.com/chessarisilvio/bias-personalizzato-per-whisper-locale) | Context-aware bias injection modules for improved speech-to-text accuracy.
        *   *Bot:* [Bot Short](https://github.com/chessarisilvio/bot-short) | C++ Telegram bot generating AI vector graphics via SVG pipelines.

    *   **Section 4: Embedded & Hardware**
        *   *Home Assistant:* [AI Home Assistant HID Dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) | Arduino R4 WiFi and ESP32-based physical interface for AI stack control.
        *   *Model Selector:* [AI Model Selector Physical Controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) | Hardware interface with rotary encoder and OLED for real-time model switching.
        *   *Thermal:* [Proactive Thermal Controller ESP32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) | Embedded fan control logic with proactive sensor feedback.

    *   **GitHub Stats:** Standard markdown images format.

4.  **Refining and Formatting:**
    *   Check line count.
    *   Check emojis (only in header).
    *   Check tone (technical, precise).
    *   Check slugs.

    *Self-Correction on Slugs/Links:*
    *   `nex2-mini-phase-twin-30b-lowvram-gguf-model`
    *   `sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf` (Need to make the slug English-based or keep Italian? The prompt says "derived from project names (lowercase, hyphens)". Since project names are in Italian, I should probably transliterate or keep the Italian slug, but to make it "GitHub-ready" I will slugify the Italian name provided).
    *   `automated-exl2-conversion-validation-pipeline`
    *   `cuda-sm61-compatibility-shim`
    *   `automazione-bootwatchdog-ai-avanzato`
    *   `ai-dashboard`
    *   `add-video-input-support-to-llamacpp-mtmd`
    *   `bias-personalizzato-per-whisper-locale`
    *   `bot-short`
    *   `ai-home-assistant-hid-dashboard`
    *   `ai-model-selector-physical-controller`
    *   `controller-termico-proattivo-esp32`

5.  **Final Polish (Simulated Render):**

    *   Header: `# Silvio Chessari`
    *   Bio: 3 lines.
    *   Stack: Table.
    *   Projects: 4 sections.
    *   Stats: Bottom.

    *Specific Content check:*
    *   "Show real technical depth: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing)..." -> I should ensure these keywords fit naturally into the bio or project descriptions. The bio is good for this.
    *   "Running LLMs on unsupported consumer/datacenter GPUs (Tesla P40 sm_61, CUDA workarounds)..." -> Covered in Bio and CUDA Shim project.
    *   "Self-built AI infrastructure..." -> Covered in Bio and Dashboard/Watchdog.

6.  **Constructing the Markdown:**

    (Writing the actual content in the final output block)

    *Bio Adjustment:* Make sure to mention "speculative decoding" and "MoE routing" explicitly since they were requirements, even if not explicitly in the project names (though implied by "Nex2" and "Qwen3.5 MoE"). I will put them in the bio.

    *Line Count Check:*
    Header: 3 lines.
    Bio: 3 lines.
    Table: 4-5 lines.
    Projects: ~15-18 lines (headers + descriptions).
    Stats: 4 lines.
    Spacing: Adds lines.
    Total should roughly hit 60-80 lines if compact, maybe more if spaced out. The prompt asks for 90-120.
    *Action:* I need to expand the descriptions slightly or ensure the formatting takes up space (e.g., double spacing between sections is not counted as fluff, but readability). I will ensure the descriptions are detailed single lines.

    *Let's calculate lines:*
    Header (centered): ~5 lines.
    Bio: 3 lines.
    Stack Table: ~5 lines.
    H2 Dividers: 4 lines.
    Project Headers: 4 lines.
    Project Items: 12 items x 2 lines = 24 lines.
    Stats: ~5 lines.
    Total so far: ~50 lines. I need to reach 90.
    *Strategy:* I will add a "Technical Focus" list or expand the Stack table, or ensure the project descriptions use standard GitHub README formatting which often breaks lists onto new lines. However, the requirement was "1-line technical description".
    *Alternative Strategy:* Add a specific "Hardware" section in the stack or make the table longer? No, "compact stack table".
    Wait, the prompt says "90–120 lines total". If I write compact markdown, it's hard to hit 120.
    I will ensure I use standard horizontal rules and perhaps add a "Focus Areas" section or split the project lists with more space/headers? No, strict structure requested.
    I will add a "Tools" breakdown within the stack or ensure the table row count is sufficient.
    Actually, standard spacing (newlines after headers, between sections) helps.
    Let's look at the project count. There are 12 projects.
    Header + Bio + Table + Intro + 4 Sections + 12 items + Footer.
    5 + 3 + 6 + 4 + 4 + 12 + 5 = 39 lines