1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Output:** GitHub profile README.md (Markdown only).
    *   **Persona/Subject:** Silvio Chessari.
    *   **Style:** Professional, technical, precise, no fluff, English.
    *   **Content:** LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), GPU compatibility (Tesla P40 sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.
    *   **Input:** "Vault data" (Obsidian notes in Italian) describing various projects.
    *   **Structure Requirements:**
        1.  Centered header.
        2.  3-line technical bio.
        3.  Compact stack table.
        4.  4 Project sections: LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware.
        5.  GitHub stats.
    *   **Project Format:** `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
    *   ** Slug Rule:** lowercase, hyphens.
    *   **Constraints:** Max 2 emojis (header only), 90–120 lines total.
    *   **Instruction:** Output ONLY the final README.md.

2.  **Analyze the Source Data (Vault Data):**
    *   *Context:* Silvio seems to be a deep technical tinkerer, focused on local LLMs, hardware optimization, and automation.
    *   *Projects identified:*
        *   *LLM Research/Infrastructure:*
            *   `Sistema di Benchmarking Automatizzato per Nuovi Modelli GGUF` (Benchmarking GGUF on P40/3050).
            *   `Auto-Quantization Pipeline GGUF` (Automated quantization check).
            *   `Add video input support to llama.cpp (mtmd)` (llama.cpp mods, OpenCV, CMake).
            *   `Automated EXL2 Conversion & Validation Pipeline` (Qwen MoE, EXL2, mixed quant).
            *   `CUDA sm_61 Compatibility Shim` (Tesla P40 support, CUDA workarounds).
            *   `AI Dashboard` (:9190, monitoring local AI).
            *   `Openclaw` (Node.js Ollama gateway).
            *   `Automazione Boot/Watchdog AI Avanzato` (systemd, llama-stack, VRAM monitoring).
            *   `NLLB Self-Hosted` (OCR+MT pipeline).
            *   `Bias personalizzato per Whisper locale` (Whisper biasing).
        *   *Tools & Automation:*
            *   `bot-short` (C++, Telegram, SVG generation, AI graphics).
            *   `Megatool` (C++ OSINT, Flask web app, AI photo analysis).
            *   `Reddit Monitor` (Subreddit tracking to AGENDA.md).
            *   `VideoStudio` (Storyboard LLM, Higgsfield, Python backend).
            *   `Silvioprint` (Telegram bot content, systemd).
            *   `Silvioprint — Sito Web` (HTML/CSS/JS e-commerce).
        *   *Embedded & Hardware:*
            *   `AI Home Assistant HID Dashboard` (Arduino R4 WiFi, ESP32, MQTT/Tailscale, LCD).
            *   `AI Model Selector Physical Controller` (ESP32, encoder, OLED, HID).
            *   `Controller Termico ESP32` (Fan control, sensors).
            *   `Thermalright LCD` (HID temp display).
            *   `mtop` (htop for LLM monitoring).

3.  **Drafting Content - Section by Section:**

    *   **Header:** Simple, centered.
        `# Silvio Chessari`
        `### High-Performance AI Enthusiast`

    *   **Bio (3 lines):** Focus on the prompt's keywords (Inference, P40, Infrastructure, Embedded).
        *   *Draft:* Specialized in local LLM inference optimization, focusing on speculative decoding (EAGLE/MTP), MoE routing, and running models on legacy hardware (Tesla P40 sm_61). I build self-hosted AI infrastructure, CUDA compatibility shims, and automated benchmarking pipelines. My work bridges embedded systems (ESP32/Arduino) with high-performance compute to create physical interfaces for generative AI.

    *   **Compact Stack Table:** Categorize the tech mentioned.
        *   *Languages:* C++, Python, CMake, Bash, HTML/CSS/JS.
        *   *Frameworks:* llama.cpp, Ollama, OpenCV, Flask, Node.js.
        *   *Hardware:* NVIDIA Tesla P40 (sm_61), RTX 3050, ESP32, Arduino R4 WiFi.
        *   *ML/AI:* EXL2, GGUF, Whisper, NLLB-200, MoE Routing.

    *   **Projects - LLM Research:**
        *   `CUDA sm-61 Compatibility Shim` -> [cuda-sm61-compatibility-shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim)
        *   `Add video input support to llama.cpp` -> [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd)
        *   `Automated EXL2 Conversion` -> [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline)
        *   `Auto-Quantization Pipeline` -> [auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf)
        *   `Bias per Whisper` -> [bias-personalizzato-per-whisper-locale](https://github.com/chessarisilvio/bias-personalizzato-per-whisper-locale)

    *   **Projects - AI Infrastructure:**
        *   `Sistema di Benchmarking` -> [sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf)
        *   `Automazione Boot/Watchdog` -> [automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato)
        *   `Openclaw` -> [openclaw](https://github.com/chessarisilvio/openclaw)
        *   `AI Dashboard` -> [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard)
        *   `NLLB Self-Hosted` -> [nllb-self-hosted-per-testo-multilingua](https://github.com/chessarisilvio/nllb-self-hosted-per-testo-multilingua)

    *   **Projects - Tools & Automation:**
        *   `bot-short` -> [bot-short](https://github.com/chessarisilvio/bot-short)
        *   `Megatool` -> [megatool](https://github.com/chessarisilvio/megatool)
        *   `VideoStudio` -> [videostudio](https://github.com/chessarisilvio/videostudio)
        *   `Reddit Monitor` -> [reddit-monitor](https://github.com/chessarisilvio/reddit-monitor)
        *   `Silvioprint` -> [silvioprint](https://github.com/chessarisilvio/silvioprint)

    *   **Projects - Embedded & Hardware:**
        *   `AI Home Assistant HID` -> [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard)
        *   `AI Model Selector` -> [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller)
        *   `Controller Termico` -> [controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32)
        *   `Thermalright LCD` -> [digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd)
        *   `mtop` -> [mtop](https://github.com/chessarisilvio/mtop) (This fits here or infrastructure, but hardware monitor implies embedded/systems interface).

    *   **Stats:** Standard GitHub stats image code.

4.  **Refining and Formatting:**
    *   Check line count constraints (90-120 lines).
    *   Ensure descriptions are 1 line technical.
    *   Ensure no fluff.
    *   Check slugs (lowercase-hyphens).
    *   Check emoji limit (header only).

    *   *Self-Correction during drafting:* The prompt specifically mentions "LLM inference research (EAGLE/MTP...)" in the *Requirements*, but the *Vault Data* doesn't explicitly name EAGLE/MTP, just implies deep inference via llama.cpp mods and MoE architectures. I will incorporate the specific inference tech requirements into the *Bio* and descriptions where the vault implies them (e.g., "Advanced CUDA workarounds," "MoE Architecture Fix," "Speculative Decoding" can be inferred from the high-level request applied to the specific projects).
    *   *Refining Descriptions:*
        *   *CUDA shim:* "Compatibility layer for Pascal (Tesla P40) to run modern CUDA binaries on legacy sm_61 architecture."
        *   *Video input llama.cpp:* "CMake modifications and C stubs extending llama.cpp for real-time webcam/video frame ingestion."
        *   *EXL2:* "Mixed precision quantization pipeline featuring Qwen3.5 MoE architecture fixes and automated validation."
        *   *Bot-short:* "High-performance C++ Telegram bot leveraging generative AI for dynamic vector graphics (SVG) synthesis."

5.  **Final Code Structure Construction:**

    ```markdown
    <center>
    <img src="..." width="200">
    # Silvio Chessari

    ### Research Engineer · Infrastructure & Embedded AI
    </center>

    Specializing in local LLM inference, I research speculative decoding, MoE routing, and EAGLE implementations.
    I engineer self-hosted AI infrastructure optimized for edge cases, running models on unsupported consumer/datacenter GPUs (Tesla P40 sm_61) via custom CUDA workarounds.
    My workflow connects embedded systems (ESP32/Arduino) to high-performance compute, building physical interfaces and automated monitoring for generative models.

    ### 🛠 Technical Stack

    | Core | Infra | ML/AI | Hardware |
    | :--- | :--- | :--- | :--- |
    | C++, Python, CMake | Docker, Systemd, Tailscale | llama.cpp, EXL2, GGUF | Tesla P40, RTX 3050 |
    | Node.js, Flask | OpenClaw Gateway | MoE Routing (Qwen) | ESP32, Arduino R4 WiFi |
    | Bash, OpenCV | MQTT, Home Automation | Whisper, NLLB-200 | HID Protocols, Sensors |

    <br>

    ### 🧠 LLM Research & Inference

    - [cuda-sm61-compatibility-shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim) — Compatibility layer executing modern CUDA binaries on legacy Pascal GPUs (Tesla P40 sm_61).
    - [automated-exl2-conversion-validation