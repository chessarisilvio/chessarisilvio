**User Request Analysis:**
*   **Persona:** Technical Writer.
*   **Output:** A professional GitHub profile README.md.
*   **Subject:** Silvio Chessari.
*   **Source Material:** "Vault Data" (Obsidian notes) in Italian detailing various projects.
*   **Requirements:**
    *   **Format:** Only the final Markdown (no preamble/explanation).
    *   **Tone:** English, technical, precise, no fluff.
    *   **Content:**
        *   Deep technical details: LLM inference (EAGLE, MTP, speculative decoding, MoE routing), consumer/datacenter GPU hacks (Tesla P40, sm_61, CUDA), self-built AI infra, embedded systems.
        *   Structure: Centered header (max 2 emojis) -> 3-line technical bio -> Compact stack table -> 4 project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware) -> GitHub stats.
        *   Projects: `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description. Slugs must be derived from project names (lowercase, hyphens).
    *   **Length:** 90–120 lines total.

**Source Data Analysis & Extraction:**

*   *Bio/Hint:* Focus on LLM inference research, CUDA hacks (Tesla P40 sm_61), self-built AI infra, embedded systems (ESP32).
*   *Projects:*
    1.  *LLM Reseach:*
        *   `add-video-input-support-to-llamacpp-mtmd` -> Video input for llama.cpp. (Slug: `add-video-input-support-to-llamacpp-mtmd`)
        *   `ai-dashboard` -> Monitoring, GPU panels, AGENDA.md. (Slug: `ai-dashboard`)
        *   `mtop-htop-per-monitoraggio-llm-locale` -> htop-like monitor for local LLM inference, real-time metrics. (Slug: `mtop-htop-for-local-llm-monitoring`)
    2.  *AI Infrastructure:*
        *   `auto-quantization-pipeline-gguf` -> Auto download/benchmark/quantize (Tesla P40/RTX 3050), generate GGUF. (Slug: `auto-quantization-pipeline-gguf`)
        *   `automated-exl2-conversion-validation-pipeline` -> Auto fix Qwen3_5MoeForC, EXL2 conversion, mixed quantization. (Slug: `automated-exl2-conversion-validation-pipeline`)
        *   `nllb-self-hosted-per-testo-multilingua` -> Offline NLLB-200 translation. (Slug: `nllb-self-hosted-multilingual`)
    3.  *Tools & Automation:*
        *   `automazione-bootwatchdog-ai-avanzato` -> Watchdog for `llama-stack`, VRAM/token monitoring, Telegram alerts, systemd restart. (Slug: `advanced-boot-watchdog-ai`)
        *   `bot-short` -> Python/C++ Telegram bot for AI vector graphics (SVG/EPS). (Slug: `bot-short`)
        *   `reddit-monitor` -> Subreddit AI/tech monitor -> AGENDA. (Slug: `reddit-monitor`)
        *   `git-mcp-server-per-agenti-ai` -> MCP server for Git via JSON. (Slug: `git-mcp-server`)
    4.  *Embedded & Hardware:*
        *   `controller-termico-proattivo-esp32` -> Tesla P40 fan control, ESP32, DS18B20 sensors, MOSFET driver. (Slug: `proactive-thermal-controller-esp32`)
        *   `digital-thermal-lcd` -> Thermalright LCD display via HID. (Slug: `digital-thermal-lcd`)
        *   `ai-model-selector-physical-controller` -> ESP32 physical controller (rotary/OLED) for model selection, HID/OpenClaw. (Slug: `ai-model-selector-physical-controller`)
        *   `edge-vision-node-esp32-s3-moondream` -> ESP32-S3 + moondream. (Slug: `edge-vision-node-esp32-s3-moondream`)
        *   `cuda-sm61-compatibility-shim` -> CUDA sm_61 shim for Pascal (Tesla P40). (Slug: `cuda-sm61-compatibility-shim`)

**Drafting Strategy:**

*   **Header:** `<div align="center">` + Name + Emojis (Brain, CPU).
*   **Bio:** Needs to cover: LLM inference research, running LLMs on unsupported hardware (Tesla P40/CUDA), self-built infra, embedded.
    *   Draft: Focused on pushing LLM inference limits on consumer and legacy datacenter hardware via speculative decoding and CUDA workarounds. Architecting self-hosted AI stacks that integrate high-performance compute with custom embedded control systems. Deep expertise in MoE routing, GGUF/EXL2 conversion, and bridging physical controllers with neural interfaces.
*   **Stack Table:** C++, Python, CUDA, ESP32, Docker, Ollama. Keep it compact.
*   **Project Sections:**
    *   *LLM Research:* Video input llama.cpp, mtop, Dashboard.
    *   *AI Infrastructure:* Auto GGUF pipeline, Auto EXL2, NLLB.
    *   *Tools & Automation:* Boot Watchdog, bot-short, Reddit Monitor, Git MCP.
    *   *Embedded & Hardware:* Controller Termico (P40), Shim sm_61, Model Selector, Digital LCD, Edge Vision.
*   **Stats:** Standard GitHub stats image URLs.

**Refining Content for "Real Technical Depth":**
*   Use terms like "Tesla P40", "sm_61", "speculative decoding", "HID", "PWM", "DS18B20", "EXL2", "MoE".

**Formatting & Constraints Check:**
*   *Line Count:* Need to ensure it's substantial but between 90-120 lines. I will need enough spacing and project entries.
*   *No preamble.*
*   *English only.*
*   *Slugs:* Correctly derived.

**Step-by-Step Construction:**

1.  **Header/Image:** Standard placeholder.
2.  **Bio:** 3 lines.
3.  **Stack:** `<table>` syntax.
4.  **Projects:**
    *   Group 1: LLM Research.
        *   [Add video input support to llama.cpp (mtmd)](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) - CMake integration and OpenCV pipeline for real-time frame injection into LLM inference.
        *   [mtop: htop for local LLM monitoring](https://github.com/chessarisilvio/mtop-htop-for-local-llm-monitoring) - Terminal UI displaying real-time GPU utilization, VRAM allocation, and token-per-second metrics.
        *   [AI Dashboard + Agenda](https://github.com/chessarisilvio/ai-dashboard) - Web-based orchestration layer monitoring GPU health, service status, and automating sprint tracking.
    *   Group 2: AI Infrastructure.
        *   [Auto-Quantization Pipeline GGUF](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) - Automated benchmarking against Tesla P40/RTX 3050 to determine optimal Q4_K_M vs Q5_K_S quantization.
        *   [Automated EXL2 Conversion & Validation](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) - C++/Python toolchain for fixing Qwen3_5 architecture, mixed-precision EXL2 conversion, and validation.
        *   [NLLB Self-Hosted Multilingual](https://github.com/chessarisilvio/nllb-self-hosted-multilingual) - Offline OCR + Machine Translation pipeline utilizing NLLB-200 for localized multilingual processing.
    *   Group 3: Tools & Automation.
        *   [Advanced Boot Watchdog AI](https://github.com/chessarisilvio/advanced-boot-watchdog-ai) - Systemd-dependent daemon monitoring `llama-stack` VRAM and throughput with Telegram alerting.
        *   [bot-short](https://github.com/chessarisilvio/bot-short) - C++ Telegram bot leveraging local LLMs to generate and transmit vector graphics (SVG/EPS).
        *   [Reddit Monitor](https://github.com/chessarisilvio/reddit-monitor) - Asynchronous scraper tracking AI/tech subreddits to populate AGENDA.md with actionable research insights.
        *   [Git MCP Server](https://github.com/chessarisilvio/git-mcp-server) - JSON-RPC interface exposing Git operations to autonomous AI agents via the Model Context Protocol.
    *   Group 4: Embedded & Hardware.
        *   [Proactive Thermal Controller ESP32](https://github.com/chessarisilvio/proactive-thermal-controller-esp32) - PWM fan regulation for Tesla P40 using DS18B20 sensors and load prediction to minimize noise.
        *   [CUDA sm_61 Compatibility Shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim) - Workaround layer enabling modern inference frameworks on legacy Pascal architecture (sm_61).
        *   [AI Model Selector Physical Controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) - ESP32-based rotary encoder with OLED UI controlling model swaps via HID emulation.
        *   [Digital Thermal LCD](https://github.com/chessarisilvio/digital-thermal-lcd) - Python daemon driving HID interface on Thermalright coolers to display real-time thermal metrics.
        *   [Edge Vision Node ESP32-S3 + moondream](https://github.com/chessarisilvio/edge-vision-node-esp32-s3-moondream) - Edge computing node integrating ESP32-S3 vision capabilities with moondream inference.

5.  **Stats:** Standard stats blocks.

**Line Count Check (Mental):**
*   Header: 5 lines
*   Bio: 3 lines
*   Break: 2 lines
*   Stack: ~10 lines
*   Break: 2 lines
*   Heading 1 + Projects (3 items): ~6 lines
*   Heading 2 + Projects (3 items): ~6 lines
*   Heading 3 + Projects (4 items): ~8 lines
*   Heading 4 + Projects (5 items): ~10 lines
*   Break: 2 lines
*   Stats: 5 lines
*   Total ~ 60 lines. I need to expand the spacing or structure slightly to hit 90-120 lines comfortably without fluff. I will use standard Markdown spacing (line breaks) and ensuring the formatting is clean.

Let's refine the structure to reach the line count naturally.

**Final Polish:**
*   Ensure slugs are lowercase-hyphens.
*   Ensure technical terms are accurate (sm_61, Pascal, DS18B20, EXL2, MCP).

**Project Slug Derivation:**
*   `add-video-input-support-to-llamacpp-mtmd` -> `add-video-input-support-to-llamacpp-mtmd` (Keep as is or shorten to `llamacpp-mtmd-video-input`? The requirement says "derived from project names". I will stick to the close derivation or the filename structure used in the prompt. The prompt lists "add-video-input-support-to-llamacpp-mtmd". That is long. I will use `add-video-input-support-to-llamacpp-mtmd`.)
*   `