1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Output:** Professional GitHub profile `README.md` for Silvio Chessari.
    *   **Requirements:**
        *   ONLY the final Markdown (no preamble).
        *   English, technical, precise.
        *   Tone: Real technical depth (LLM inference, CUDA/hardware hacks, local AI infra).
        *   Structure: Header (centered) -> 3-line bio -> Compact stack table -> 4 Project sections (LLM Research, AI Infra, Tools & Automation, Embedded & Hardware) -> GitHub stats.
        *   Project Format: `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
        *   Slugs: Lowercase, hyphens.
        *   Emojis: Max 2 (header only).
        *   Length: 90–120 lines.

2.  **Analyze the Vault Data:**
    *   **Profile:** Silvio Chessari (inferred from username `chessarisilvio` in project links).
    *   **Categories:** Code developed, LLM stack, third-party tools, research, ideas.
    *   **Key Projects/Themes:**
        *   *LLM Research/Inference:* `add-video-input-support-to-llamacpp-mtmd`, `auto-quantization-pipeline-gguf`, `automated-exl2-conversion-validation-pipeline`, `cuda-sm61-compatibility-shim` (Tesla P40 support), `bias-personalizzato-per-whisper-locale`, `mtop` (htop for LLMs), `nllb-self-hosted`.
        *   *AI Infrastructure:* `ai-dashboard`, `automazione-bootwatchdog-ai-avanzato`, `openclaw` (Ollama gateway).
        *   *Tools & Automation:* `megatool` (OSINT C++ + Flask), `silvioprint`, `bot-short` (Telegram bot, SVG), `git-mcp-server`, `reddit-monitor`.
        *   *Embedded & Hardware:* `controller-termico-proattivo-esp32` (Tesla P40 fan control via ESP32), `ai-model-selector-physical-controller` (ESP32 + OLED + Encoder), `digital-thermal-lcd`, `edge-vision-node-esp32-s3-moondream`.
    *   **Technical Details:**
        *   Hardware: Tesla P40 (sm_61 compatibility, IPMI, fan control), ESP32, DS18B20, MOSFETs, OLED SSD1306.
        *   Software: CUDA (sm_61), llama.cpp, C++, Python, Flask, Node.js, systemd, Telegram API.
        *   Focus: Running LLMs on unsupported hardware, speculative decoding, MoE routing (implied by Qwen3_5Moe), EXL2, GGUF.

3.  **Drafting - Section by Section:**

    *   **Header:**
        ```markdown
        <div align="center">
        <h1>Silvio Chessari</h1>
        <p>LLM Inference Research & System Engineering</p>
        </div>
        ```
        *Emoji constraint:* Add max 2 emojis here or near the bio. Let's keep it clean. Maybe "🚀" or "⚡". Let's stick to just text for the header to be professional, or put emojis in the header title line.

    *   **3-line Technical Bio:**
        Needs to cover: LLM inference (optimization/research), Hardware hacks (Tesla P40, CUDA), Embedded (ESP32).
        *Draft:*
        researcher in efficient LLM inference, specializing in speculative decoding, MoE routing, and CUDA compatibility shims for legacy datacenter hardware.
        I architect self-hosted AI stacks on consumer-grade hardware, focusing on Tesla P40 optimization and automated quantization pipelines (EXL2/GGUF).
        My work bridges embedded systems and AI, implementing custom controllers for thermal management and physical model selection.

    *   **Compact Stack Table:**
        Columns: Domain, Tech.
        *Rows:* Inference, Embedded, Infra, Languages.
        *Content:* CUDA/C++, llama.cpp, ESP32, Python, systemd.

    *   **Project Sections (Constraint: 4 sections):**
        1.  *LLM Research & Inference*
        2.  *AI Infrastructure*
        3.  *Tools & Automation*
        4.  *Embedded & Hardware*

    *   **Selecting Projects & Generating Links/Descriptions:**

        *   *Section 1: LLM Research & Inference*
            *   `cuda-sm61-compatibility-shim`: [CUDA sm_61 Compatibility Shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim) - CUDA compatibility layer for Pascal architecture (Tesla P40) to enable modern LLM inference.
            *   `automated-exl2-conversion-validation-pipeline`: [Automated EXL2 Conversion & Validation Pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) - Toolchain for fixing Qwen3.5 MoE architecture, converting to EXL2, and applying mixed quantization.
            *   `add-video-input-support-to-llamacpp-mtmd`: [Add video input support to llama.cpp (mtmd)](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) - Extends llama.cpp to accept video frames from OpenCV for multimodal processing.
            *   `bias-personalizzato-per-whisper-locale`: [Bias personalizzato per Whisper locale](https://github.com/chessarisilvio/bias-personalizzato-per-whisper-locale) - Post-processing module for Whisper using local LLMs to apply context-aware bias and ASR correction.

        *   *Section 2: AI Infrastructure*
            *   `ai-dashboard`: [AI Dashboard](https://github.com/chessarisilvio/ai-dashboard) - Local monitoring web app (port 9190) tracking GPU metrics, services, and AGENDA integration.
            *   `automazione-bootwatchdog-ai-avanzato`: [Automazione Boot/Watchdog AI Avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) - Advanced systemd watchdog for llama-stack monitoring VRAM/token throughput with Telegram alerts.
            *   `auto-quantization-pipeline-gguf`: [Auto-Quantization Pipeline GGUF](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) - Automated pipeline for model downloading, benchmarking (Tesla P40/RTX 3050), and optimal GGUF generation.
            *   `openclaw`: [Openclaw](https://github.com/chessarisilvio/openclaw) - Node.js gateway acting as an interface for local Ollama instances.

        *   *Section 3: Tools & Automation*
            *   `megatool`: [Megatool](https://github.com/chessarisilvio/megatool) - OSINT suite built in C++ with a Flask web interface for photo analysis and data gathering.
            *   `mtop-htop-per-monitoraggio-llm-locale`: [mtop: htop per monitoraggio LLM locale](https://github.com/chessarisilvio/mtop-htop-per-monitoraggio-llm-locale) - Real-time terminal monitor for local LLM inference, displaying GPU utilization and token speed.
            *   `git-mcp-server-per-agenti-ai`: [Git MCP Server for AI Agents](https://github.com/chessarisilvio/git-mcp-server-per-agenti-ai) - Model Context Protocol server exposing Git operations via a JSON API for AI agents.
            *   `bot-short`: [bot-short](https://github.com/chessarisilvio/bot-short) - C++ Telegram bot that generates and delivers AI-created vector graphics (SVG/EPS).

        *   *Section 4: Embedded & Hardware*
            *   `controller-termico-proattivo-esp32`: [Controller Termico Proattivo ESP32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) - ESP32 thermal regulator for Tesla P40 using DS18B20 sensors and PWM fan control to prevent throttling.
            *   `ai-model-selector-physical-controller`: [AI Model Selector Physical Controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) - Hardware interface with rotary encoder and OLED to switch local AI models via HID/OpenClaw.
            *   `digital-thermal-lcd`: [Digital Thermal LCD](https://github.com/chessarisilvio/digital-thermal-lcd) - HID-based display that renders temperature metrics for local hardware monitoring.
            *   `edge-vision-node-esp32-s3-moondream`: [Edge Vision Node ESP32-S3 + moondream](https://github.com/chessarisilvio/edge-vision-node-esp32-s3-moondream) - Embedded vision node integrating ESP32-S3 with lightweight computer vision models.

4.  **Refining and Formatting:**

    *   Review constraints: English, technical, precise. No fluff.
    *   Line count check: The current draft looks to be around 110 lines including the GitHub stats section (which I need to format using standard syntax).
    *   Usernames: Must use `chessarisilvio`.
    *   Structure check:
        *   Centered header.
        *   3-line bio.
        *   Stack table.
        *   4 Project sections with specific linking format.
        *   GitHub stats (using the standard `github-readme-stats` images).

5.  **Final Polish (Self-Correction during drafting):**
    *   *Project Titles:* Some are Italian in the vault (e.g., "Controller Termico Proattivo ESP32"). The prompt says "English, technical", but project names usually stay in original language if they are code folders, or get translated for consistency. The prompt asks to "Generate... based on his technical vault data" and "Use real technical details". It doesn't explicitly say "translate project names". However, for an English README, Italian titles might look odd *unless* they are code folders. Looking at the "Path sorgente" column, e.g., `ai-dashboard`, `bot-short`, `megatool` are English. Others like `automazione-bootwatchdog-ai-avanzato` are Italian. I will keep the project titles as they appear in the "Progetto" column of the vault to be accurate to the data, but I will ensure the descriptions are English.
    *   *Slugs:* Convert titles to lowercase-hyphen. `automazione-bootwatchdog-ai-avanzato` -> `automazione-bootwatchdog-ai-avanzato`. `controller-termico-proattivo-esp32` -> `controller-termico-proattivo-esp32`.
    *   *Emojis:* Add 2 emojis to the header. "🔬" and "🛠️".

6.  **Constructing the Final Output:**

    (Proceeding to generate the Markdown block.)

    *   *Stats section:* I'll use the standard generic URLs since I can't generate real-time stats, but I'll format them correctly.
    *   *Stack Table:*
        ```markdown
        | Domain | Tech |
        | :--- | :--- |
        | **Inference** | llama.cpp, EXL2, GGUF, Speculative Decoding, MoE |
        | **Embedded