1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Target:** Professional GitHub profile README.md for Silvio Chessari.
    *   **Source Material:** "Technical vault data" (Obsidian-style notes).
    *   **Requirements:**
        *   Output *only* the README.md.
        *   No preamble, no explanation.
        *   Language: English, technical, precise, no fluff.
        *   Technical Depth: LLM inference (EAGLE/MTP/speculative decoding/MoE routing), unsupported GPU runtimes (Tesla P40 sm_61, CUDA workarounds), self-built AI infra, embedded systems.
        *   Use real details from the vault (ESP32 thermal control, custom bots, EXL2 pipelines, CUDA shims).
        *   Structure:
            *   Centered header (Max 2 emojis).
            *   3-line technical bio.
            *   Compact stack table.
            *   4 project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware).
            *   GitHub stats at the bottom.
        *   Project format: `[name](https://github.com/chessarisilvio/slug)` + 1-line description.
        *   Slug format: lowercase, hyphens.
        *   Length: 90–120 lines total.

2.  **Extract & Analyze Data:**
    *   *User:* Silvio Chessari.
    *   *Core Focus:* Local AI, Inference optimization (unsupported hardware), Embedded AI, Automation.
    *   *Specific Projects to Highlight:*
        *   **LLM Research:**
            *   `add-video-input-support-to-llamacpp-mtmd` (Video input for llama.cpp).
            *   `automated-exl2-conversion-validation-pipeline` (EXL2/MoE quantization).
            *   `mtop-htop-per-monitoraggio-llm-locale` (Inference monitoring).
        *   **AI Infrastructure:**
            *   `ai-dashboard` (Web dashboard at :9190).
            *   `automazione-bootwatchdog-ai-avanzato` (Systemd watchdog for llama-stack).
            *   `openclaw` (Ollama Gateway).
            *   `nllb-self-hosted-per-testo-multilingua` (OCR+MT pipeline).
        *   **Tools & Automation:**
            *   `git-mcp-server-per-agenti-ai` (MCP server).
            *   `bot-short` (C++ Telegram bot SVG generation).
            *   `megatool` (OSINT C++ + Flask + AI photo analysis).
            *   `auto-quantization-pipeline-gguf` (GGUF benchmarking P40/3050).
            *   `launcher-avanzato-per-llama-server` (Launcher).
        *   **Embedded & Hardware:**
            *   `controller-termico-proattivo-esp32` (Tesla P40 fan control via ESP32).
            *   `digital-thermal-lcd` (LCD temperature HID).
            *   `ai-model-selector-physical-controller` (Physical knob for model selection).
            *   `edge-vision-node-esp32-s3-moondream` (ESP32-S3 Vision).
            *   `cuda-sm61-compatibility-shim` (Pascal sm_61 support).

3.  **Drafting the Content:**

    *   **Header:** Name, Simple title. Emojis: ⚡ 🛠️ (stay under 2).
    *   **Bio:** Needs to cover LLM inference research (EAGLE/MTP/speculative decoding/MoE), running LLMs on unsupported GPUs (P40 sm_61), and embedded systems integration.
    *   **Stack Table:** Python, C++, CUDA, ESP32, Linux/Systemd, LLM Tooling (llama.cpp, EXL2).
    *   **Project Sections:** I need to categorize the extracted projects into the requested 4 sections.

        *   *LLM Research:*
            *   `add-video-input-support-to-llamacpp-mtmd` -> Video input for llama.cpp via custom OpenCV integration.
            *   `automated-exl2-conversion-validation-pipeline` -> Qwen3.5 MoE architecture fix and mixed precision EXL2 quantization.
            *   `bias-personalizzato-per-whisper-locale` -> Contextual bias module and LLM-based correction for local Whisper.

        *   *AI Infrastructure:*
            *   `ai-dashboard` -> Local monitoring web service for GPU metrics, systemd status, and AGENDA tasks.
            *   `automazione-bootwatchdog-ai-avanzato` -> Advanced systemd watchdog monitoring VRAM and token-per-second for llama-stack.
            *   `openclaw` -> Node.js gateway for Ollama integration.
            *   `nllb-self-hosted-per-testo-multilingua` -> Offline NLLB-200 OCR and machine translation pipeline.

        *   *Tools & Automation:*
            *   `git-mcp-server-per-agenti-ai` -> Model Context Protocol server exposing Git operations for AI agents.
            *   `auto-quantization-pipeline-gguf` -> Automated benchmarking and quantization pipeline for Tesla P40 and RTX 3050.
            *   `bot-short` -> C++ Telegram bot generating AI vector graphics in SVG/EPS.
            *   `megatool` -> OSINT suite in C++ with Flask web interface and AI photo analysis.
            *   `launcher-avanzato-per-llama-server` -> Advanced launcher wrapper for inference servers.

        *   *Embedded & Hardware:*
            *   `controller-termico-proattivo-esp32` -> ESP32 PWM fan controller for Tesla P40 with thermal sensors.
            *   `cuda-sm61-compatibility-shim` -> Compatibility layer for running modern CUDA stacks on Pascal (sm_61) GPUs.
            *   `ai-model-selector-physical-controller` -> ESP32 rotary encoder and OLED device for physical model switching.
            *   `digital-thermal-lcd` -> HID-based LCD display for real-time thermal metrics.
            *   `edge-vision-node-esp32-s3-moondream` -> ESP32-S3 edge vision node integrating Moondream.

    *   **GitHub Stats:** Standard placeholders (e.g., `![Stats](...)`).

4.  **Refining and Formatting:**

    *   *Constraint Check:* 90-120 lines. Need to ensure descriptions are concise but technical.
    *   *Constraint Check:* `chessarisilvio` username.
    *   *Constraint Check:* Slugs need to be consistent.

    *   *Drafting the Bio:*
        Specializing in high-performance local AI inference and unsupported hardware enablement. Expertise in speculative decoding, MoE routing, and CUDA architecture shims (sm_61) for legacy datacenter GPUs. Developer of self-hosted AI infrastructure, embedded control systems for thermal management, and automation tooling.

    *   *Drafting the Stack Table:*
        | Area | Tech |
        | :--- | :--- |
        | Inference | llama.cpp, EXL2, GGUF, Speculative Decoding |
        | Languages | Python, C++, Bash |
        | Embedded | ESP32, Arduino, FreeRTOS |
        | Systems | Linux, Systemd, Docker, CUDA (Legacy) |

    *   *Refining Project descriptions:*
        *   `add-video-input-support-to-llamacpp-mtmd` -> `llama-cpp-video-extension`: Extended `llama.cpp` CMake and core stubs to accept video frames via OpenCV pipeline for multimodal inference.
        *   `automated-exl2-conversion-validation-pipeline` -> `exl2-moe-pipeline`: Automated Qwen3.5 MoE architecture fix, mixed-precision EXL2 conversion, and benchmarking validation.
        *   `mtop-htop-per-monitoraggio-llm-locale` -> `mtop`: htop-like CLI utility specifically designed for real-time local LLM token/performance metrics.
        *   `controller-termico-proattivo-esp32` -> `tesla-p40-esp32-controller`: ESP32-based proactive fan controller using 1-Wire sensors and PWM to manage Tesla P40 thermals.
        *   `cuda-sm61-compatibility-shim` -> `cuda-sm61-shim`: Compatibility shim layer enabling modern LLM toolchains on Pascal architecture (sm_61) GPUs.
        *   `git-mcp-server-per-agenti-ai` -> `git-mcp-server`: Model Context Protocol server exposing Git operations to facilitate autonomous AI agent workflows.
        *   `ai-dashboard` -> `ai-dashboard`: Local web dashboard aggregating GPU telemetry, systemd service states, and automated AGENDA.md tasks.
        *   `automazione-bootwatchdog-ai-avanzato` -> `llama-watchdog`: Advanced systemd watchdog monitoring VRAM saturation and TPS for local inference stacks.

5.  **Final Assembly & Line Count Check:**

    *   Header: ~5 lines.
    *   Bio: ~4 lines.
    *   Stack: ~8 lines.
    *   Projects:
        *   LLM Research: ~6 lines.
        *   AI Infra: ~8 lines.
        *   Tools: ~8 lines.
        *   Embedded: ~8 lines.
    *   Stats: ~5 lines.
    *   Total: ~52 lines. This is too short. The requirement is 90-120 lines. I need to expand the formatting, add spacing (but keep it "compact"), and perhaps add more detail to the project descriptions or add more projects from the list (there are plenty).

    *   *Expansion Strategy:*
        *   Split the project sections clearly with headers.
        *   Use bullet points for projects instead of a single dense list.
        *   Make the tech stack table slightly more detailed or split into rows.
        *   Ensure there are enough projects. I have about 15-20 good ones. If I list 4-5 per section, that fills space.

    *   *Revised Plan:*
        *   **Header:** 5 lines.
        *   **Bio:** 4 lines.
        *   **Stack:** 10 lines.
        *   **LLM Research Section:** Header + 4 projects (8 lines).
        *   **AI Infrastructure:** Header + 4 projects (8 lines).
        *   **Tools & Automation:** Header + 4 projects (8 lines).
        *   **Embedded & Hardware:** Header + 4 projects (8 lines).
        *   **Stats:** 5 lines.
        *   Total still under 60? Wait, standard markdown spacing.
        *   Let's count lines in a standard editor view.
        *   If I add 5 projects per section:
        *   4 sections * 5 projects = 20 lines.
        *   Plus headers, spacer lines.
        *   Maybe I should write a "Technical Focus" section or split the Stack to take more vertical space? No, keep structure.
        *   Actually, just listing the projects takes more lines if formatted cleanly with a blank line between them or a dash indentation.
        *   Let's try to pack more projects from the specific list provided.
        *   Missing in first pass: `qwen-image-edit-inpainting-workflow`, `open-source-mcp-bridge-for-local-claude-code`, `silvioprint`, `reddit-monitor`.

    *   Let's list 5 projects per section if available.

    *   *LLM Research:*
        1. exl2-pipeline
        2. llama-cpp-video