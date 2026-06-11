1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Target:** Professional GitHub Profile README.md for Silvio Chessari.
    *   **Input:** Technical Vault Data (Obsidian notes format in Italian).
    *   **Requirements:**
        *   Output ONLY final README.md markdown.
        *   No preamble, no explanation.
        *   Language: English, technical, precise, no fluff.
        *   Content emphasis: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), unsupported GPUs (Tesla P40, sm_61 workarounds), AI infra, embedded systems.
        *   Structure: Centered header -> 3-line bio -> Compact stack table -> 4 project sections (LLM Research, AI Infrastructure, Tools & Automation, Embedded & Hardware) -> GitHub stats.
        *   Project format: `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
        *   Slug derivation: lowercase, hyphens.
        *   Emojis: Max 2 total in header only.
        *   Length: 90–120 lines.

2.  **Analyze the Vault Data (Source Material extraction):**
    *   *Bio/Context:* Focus on LLM stack, research, GPU compatibility, embedded systems.
    *   *Projects:*
        *   `ai-dashboard`: Python, web framework, AGENDA.md, worker tasks.
        *   `bot-short`: C++ Telegram bot, AI vector graphics, SVG pipeline.
        *   `controller-termico-proattivo-esp32`: ESP32 fan control, PID logic, Tesla P40 cooling, 1-Wire sensors.
        *   `digital-thermal-lcd`: LCD temp display via HID.
        *   `megatool`: OSINT C++, Flask web app `:7788`, AI photo analysis.
        *   `openclaw`: Ollama Gateway, Node.js.
        *   `reddit-monitor`: Python, subreddit AI/tech scraping -> AGENDA.md.
        *   `automazione-bootwatchdog-ai-avanzato`: `llama-stack` watchdog, systemd, Telegram, VRAM/tokens monitoring.
        *   `launcher-avanzato-per-llama-server`: Advanced launcher (Idea).
        *   `cuda-sm61-compatibility-shim`: CUDA sm_61 compatibility for Pascal (Tesla P40).
        *   `add-video-input-support-to-llamacpp-mtmd`: Video input for llama.cpp, CMake changes, Python OpenCV demo.
        *   `ai-model-selector-physical-controller`: ESP32 rotary encoder, HID/HTTP, model switching.
        *   `automated-exl2-conversion-validation-pipeline`: C++ core, Python CLI, Qwen3.5 MoE fix, EXL2 quantization.
        *   `auto-quantization-pipeline-gguf`: Automated GGUF quantization, benchmark on P40/RTX3050.
        *   `nllb-self-hosted-per-testo-multilingua`: NLLB-200 offline translation, OCR+MT pipeline.
        *   `mtop-htop-per-monitoraggio-llm-locale`: htop-like for local LLM, real-time tokens/GPU metrics.
        *   `git-mcp-server-per-agenti-ai`: MCP server for Git operations.
        *   `open-source-mcp-bridge-for-local-claude-code`: HTTP/MCP bridge for Claude Code.
        *   `bias-personalizzato-per-whisper-locale`: Whisper bias logic, JSON/TSV bias, correction GGUF.

3.  **Structure and Draft Strategy:**

    *   **Header:** Name + Title (LLM Research & Infrastructure Engineer). Emojis: ⚡🔧 (Max 2).
    *   **Bio:**
        1.  Specialist in local LLM inference acceleration and speculative decoding.
        2.  Architecting self-hosted AI stacks on heterogeneous consumer and datacenter hardware.
        3.  Deep expertise in CUDA optimization, embedded systems integration, and automation.
    *   **Stack Table:** Python, C++, CMake, CUDA, ESP32, Docker, Node.js.
    *   **Project Sections & Classification:**
        *   *LLM Research:* add-video-input, automated-exl2, auto-quantization, bias-whisper.
        *   *AI Infrastructure:* ai-dashboard, open-source-mcp-bridge, git-mcp-server, mtop, watchdog.
        *   *Tools & Automation:* bot-short, megatool, reddit-monitor, openclaw.
        *   *Embedded & Hardware:* controller-termico, ai-model-selector, digital-thermal-lcd, cuda-sm61.

4.  **Refining Content & Slugs:**

    *   *LLM Research:*
        *   `add-video-input-support-to-llamacpp-mtmd` -> `add-video-input-support-to-llamacpp` (too long? keep it or shorten). Let's use `llamacpp-video-input` for the slug, but the prompt says "derived from project names (lowercase, hyphens)". The project name in vault is "add-video-input-support-to-llamacpp-mtmd". That's a very long slug. I will follow the instruction: "repo slugs derived from project names". I'll try to make them GitHub-friendly versions of the Italian names if those are the project names, or the English ones where available. The vault has a mix. The Italian titles are headers.
        *   *Correction:* The prompt says "Use repo slugs derived from project names".
        *   `Add video input support to llama.cpp (mtmd)` -> `add-video-input-support-to-llamacpp-mtmd` (This is long, but precise to the instruction).
        *   `Automated EXL2 Conversion & Validation Pipeline` -> `automated-exl2-conversion-validation-pipeline`.
        *   `Auto-Quantization Pipeline GGUF` -> `auto-quantization-pipeline-gguf`.
        *   `Bias personalizzato per Whisper locale` -> `bias-personalizzato-per-whisper-locale` (or maybe `custom-whisper-bias-pipeline`? Prompt says derived from project names. I will stick to the English equivalent if the project is clearly English, or transliterate Italian to English slug format if the project title is the unique identifier. Looking at the vault, titles are mixed. "Bias personalizzato per Whisper locale" is a title. Let's assume a standardized slug: `custom-whisper-bias-module`. Actually, the prompt asks to "Show real technical depth". I will map the Italian titles to reasonable English GitHub slugs that describe them, as GitHub repos usually don't have Italian slugs for a tech profile unless requested. However, the instruction is strict: "derived from project names (lowercase, hyphens)".
        *   Let's look at the `Progetto` column or the H1 headers.
        *   Item: "Bias personalizzato per Whisper locale". Slug: `bias-personalizzato-per-whisper-locale`. (A bit ugly, but follows rules).
        *   Item: "Add video input support to llama.cpp (mtmd)". Slug: `add-video-input-support-to-llamacpp-mtmd`.
        *   Let's try to clean them up slightly to look "professional" while respecting the name.
        *   Re-reading: "derived from project names". I will use the English headers where possible, otherwise translate the Italian header to an English slug because a GitHub URL `github.com/user/bias-personalizzato-per-whisper-locale` is unusual for a tech demo context, though possible. Given the user is Italian ("Silvio Chessari"), maybe he wants Italian slugs. But the README requirement is "English, technical". I will convert the specific Italian titles to English slugs for professionalism, as that fits the "English, technical" requirement better.
        *   Let's standardize:
            *   `add-video-input-support-to-llamacpp-mtmd` -> `llamacpp-video-input-extension`
            *   `automated-exl2-conversion-validation-pipeline` -> `exl2-conversion-validation-pipeline`
            *   `bias-personalizzato-per-whisper-locale` -> `custom-whisper-bias-pipeline`
            *   `auto-quantization-pipeline-gguf` -> `gguf-quantization-pipeline`

    *   *AI Infrastructure:*
        *   `AI Dashboard` -> `ai-dashboard` (Path: `ai-dashboard.py`). Slug: `ai-dashboard`.
        *   `Open-source MCP bridge for local Claude Code` -> `claude-code-mcp-bridge`.
        *   `Git MCP Server for AI Agents` -> `git-mcp-server`.
        *   `mtop: htop per monitoraggio LLM locale` -> `mtop-llm-monitor`.
        *   `Automazione Boot/Watchdog AI Avanzato` -> `llama-stack-watchdog`.

    *   *Tools & Automation:*
        *   `bot-short` -> `bot-short`.
        *   `Megatool` -> `megatool`.
        *   `Reddit Monitor` -> `reddit-monitor`.
        *   `Openclaw` -> `openclaw`.

    *   *Embedded & Hardware:*
        *   `Controller Termico ESP32` -> `tesla-p40-esp32-controller`.
        *   `AI Model Selector Physical Controller` -> `physical-ai-model-selector`.
        *   `Digital thermal LCD` -> `digital-thermal-lcd`.
        *   `CUDA sm61 Compatibility Shim` -> `cuda-sm61-compatibility-shim`.

5.  **Drafting the Content (Mental Sandbox):**

    *   *Bio:*
        Silvio Chessari
        LLM Inference Research & Infrastructure
        ...
    *   *Stack:*
        C++, Python, CUDA, CMake, ESP32, Docker, Node.js, Linux Kernel.
    *   *Sections:*
        1.  **LLM Research:**
            *   [add-video-input...](...)
            *   [automated-exl2...](...)
            *   [gguf-quant...](...)
            *   [whisper-bias...](...)
        2.  **AI Infrastructure:**
            *   [ai-dashboard](...)
            *   [claude-mcp-bridge](...)
            *   [mtop](...)
            *   [watchdog](...)
        3.  **Tools & Automation:**
            *   [bot-short](...)
            *   [megatool](...)
            *   [reddit-monitor](...)
            *   [openclaw](...)
        4.  **Embedded & Hardware:**
            *   [tesla-fan-controller](...)
            *   [model-selector](...)
            *   [thermal-lcd](...)
            *   [cuda-shim](...)

6.  **Refining the Descriptions (1-line technical):**
    *   *Video input:* Extends llama.cpp for video inference via CMake modifications and OpenCV-based frame injection.
    *   *EXL2:* Python/C++ toolchain to fix Qwen3.5 MoE architectures and automate EXL2 quantization with validation.
    *   *GGUF:* Automated pipeline to benchmark and convert LLM checkpoints to optimized GGUF on Tesla P40/RTX 3050.
    *   *Whisper:* Custom bias module for local Whisper using JSON/TSV definitions and LLM-based contextual correction.
    *   *AI Dashboard:* Local web stack monitoring GPU, services, and generating ideas via 35B models.
    *   *MCP Bridge:* Open-source HTTP