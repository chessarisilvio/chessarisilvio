1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Subject:** Silvio Chessari.
    *   **Source Material:** Technical vault data (Obsidian notes structure + project details).
    *   **Requirements:**
        *   Output *only* the final README.md (no preamble, no explanation).
        *   Tone: English, technical, precise, no fluff.
        *   Focus: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), running LLMs on unsupported GPUs (Tesla P40 sm_61, CUDA workarounds), AI infrastructure, embedded systems.
        *   Structure:
            1.  Centered header.
            2.  3-line technical bio.
            3.  Compact stack table.
            4.  4 project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware).
            5.  GitHub stats.
        *   Project Format: `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
        *   Slug derivation: lowercase, hyphens.
        *   Constraints: Max 2 emojis (header only), 90–120 lines total.

2.  **Process the Source Data (Vault Data):**
    *   *General Profile:* Silvio focuses on local AI research, hardware integration (Tesla P40, ESP32), and automation.
    *   *Key Technical Areas:* CUDA sm_61, Pascal architecture, LLMs, IoT, Embedded, Python, C++, Docker/Systemd.
    *   *Projects Mapping:*

        *   **Category: LLM Research**
            *   *Add video input to llama.cpp:* `add-video-input-support-to-llamacpp-mtmd` -> `add-video-input-support-to-llamacpp-mtmd`. Desc: Extends llama.cpp CMake and stubs for webcam/video frame injection into LLM inference.
            *   *Automated EXL2 Pipeline:* `automated-exl2-conversion-validation-pipeline` -> `automated-exl2-conversion-validation-pipeline`. Desc: C++ core + Python CLI for Qwen3_5 MoE architecture fixes and mixed-precision EXL2 quantization.
            *   *Auto-Quantization Pipeline GGUF:* `auto-quantization-pipeline-gguf` -> `auto-quantization-pipeline-gguf`. Desc: Automates checkpoint download, local benchmarking on P40/RTX 3050, and optimal GGUF quantization generation.
            *   *CUDA sm_61 Compatibility Shim:* `cuda-sm61-compatibility-shim` -> `cuda-sm61-compatibility-shim`. Desc: Compatibility layer enabling modern LLM toolchains on legacy Pascal GPUs (Tesla P40).

        *   **Category: AI Infrastructure**
            *   *AI Dashboard:* `ai-dashboard` -> `ai-dashboard`. Desc: Local monitoring stack on :9190 for GPU metrics, services, and sprint agenda integration.
            *   *Automazione Boot Watchdog:* `automazione-bootwatchdog-ai-avanzato` -> `advanced-ai-boot-watchdog`. Desc: Systemd watchdog for llama-stack monitoring VRAM/token-rate with Telegram alerts and auto-restart.
            *   *Openclaw:* `Openclaw` -> `openclaw`. Desc: Node.js gateway for local model management.

        *   **Category: Tools & Automation**
            *   *Megatool:* `Megatool` -> `megatool`. Desc: OSINT C++ toolkit with Flask web interface and AI-based photo analysis.
            *   *Reddit Monitor:* `Reddit Monitor` -> `reddit-monitor`. Desc: Python script scraping subreddits for AI/tech trends, feeding ideas into AGENDA.md.
            *   *mtop:* `mtop: htop per monitoraggio LLM locale` -> `mtop-llm-monitor`. Desc: htop-like CLI tool for real-time LLM inference metrics including GPU load and token generation speed.
            *   *Git MCP Server:* `git-mcp-server-per-agenti-ai` -> `git-mcp-server`. Desc: JSON API server enabling AI agents to perform Git operations via MCP protocol.
            *   *MCP Bridge for Claude Code:* `open-source-mcp-bridge-for-local-claude-code` -> `mcp-bridge-claude-code`. Desc: HTTP bridge connecting local Claude Code instances via MIT-licensed MCP server.
            *   *NLLB Self-Hosted:* `NLLB Self-Hosted per Testo Multilingua` -> `nllb-self-hosted`. Desc: Offline multilingual translation pipeline using NLLB-200 with OCR integration.

        *   **Category: Embedded & Hardware**
            *   *Controller Termico ESP32:* `Controller Termico ESP32` -> `esp32-tesla-p40-cooling`. Desc: ESP32 firmware with DS18B20 sensors and PWM fan control for proactive Tesla P40 thermal management.
            *   *AI Model Selector Physical:* `AI Model Selector Physical Controller` -> `ai-model-physical-controller`. Desc: Rotary encoder and OLED interface on ESP32 sending HID/HTTP commands to switch local AI models.
            *   *Edge Vision Node:* `edge-vision-node-esp32-s3-moondream` -> `edge-vision-node-esp32-s3`. Desc: ESP32-S3 edge node integrating moondream for on-device vision processing.
            *   *Digital Thermal LCD:* `Digital thermal right LCD` -> `digital-thermalright-lcd`. Desc: Python script driving Thermalright LCD via USB HID to display real-time CPU/GPU temps.

3.  **Drafting the Content (Iterative refinement for tone and constraints):**

    *   *Header:* Needs to be centered. Name: Silvio Chessari. Emojis: 🧠 ⚡.
    *   *Bio:* 3 lines. Focus on local AI, low-level GPU hacks (P40), and embedded integration.
    *   *Stack:* Table format. C++, Python, CUDA, ESP32, Docker, etc.

    *   *Project Selection & Descriptions:*
        *   *LLM Research:* Focus on the shim, video input, and quantization.
        *   *AI Infra:* Dashboard and Watchdog.
        *   *Tools:* Git MCP, mtop, Reddit monitor.
        *   *Embedded:* P40 Fan controller, physical selector, edge node.

4.  **Constructing the Markdown (Mental Draft & Line Count Check):**

    *   *Intro:* `<div align="center">...</div>`
    *   *Bio:* "Specializing in local LLM inference optimization on legacy hardware (sm_61 Pascal architecture). Research focus on speculative decoding, MoE routing, and CUDA compatibility layers for unsupported GPUs. Building end-to-end AI infrastructure from bare-metal firmware to inference orchestration."
    *   *Stack:*
        *   C++ / Python
        *   CUDA / OpenCL / Vulkan
        *   ESP32 / FreeRTOS
        *   Docker / Systemd
    *   *Sections:*
        *   `## 🧠 LLM Research` (Wait, emoji rule: max 2 total. Must remove emojis from sections).
        *   `## LLM Research`
        *   `## AI Infrastructure`
        *   `## Tools & Automation`
        *   `## Embedded & Hardware`

5.  **Refining Technical Details based on "Real Technical Depth":**
    *   Instead of just "Fan controller", use "Active thermal regulation for Tesla P40 via ESP32 PWM".
    *   Instead of "Compatibility shim", use "CUDA sm_61 compatibility layer for Pascal GPUs".
    *   Instead of "Video input", use "CMake integration for video frame capture to LLM context".

6.  **Final Polish (Simulated):**
    *   Check line count. The request asks for 90–120 lines. I need to ensure spacing is sufficient but not excessive, and descriptions are dense.
    *   Check slug format: lowercase, hyphens.
    *   Check constraint: "Output ONLY the final README.md markdown".

7.  **Detailed Content Generation:**

    *   *Bio:*
        Silvio Chessari
        Engineer specializing in local LLM inference optimization on legacy data-center hardware (Tesla P40 sm_61).
        Research focus: speculative decoding (EAGLE/MTP), MoE routing, and CUDA binary compatibility shims.
        Architecting self-hosted AI infrastructure from embedded firmware (ESP32/S3) to high-level orchestration.

    *   *Stack:*
        | System | C++, Python, Bash, Node.js |
        | --- | --- |
        | AI/ML | llama.cpp, Ollama, ComfyUI, EXL2, GGUF |
        | Hardware | CUDA (sm_61), ESP32, USB HID, IPMI |
        | Infra | Docker, systemd, Nginx, Flask |

    *   *Projects:*
        *   Research: `cuda-sm61-compatibility-shim`, `add-video-input-support-to-llamacpp-mtmd`, `automated-exl2-conversion-validation-pipeline`, `auto-quantization-pipeline-gguf`.
        *   Infra: `ai-dashboard`, `advanced-ai-boot-watchdog`.
        *   Tools: `git-mcp-server`, `mtop-llm-monitor`, `reddit-monitor`, `mcp-bridge-claude-code`.
        *   Embedded: `esp32-tesla-p40-cooling`, `ai-model-physical-controller`, `edge-vision-node-esp32-s3`, `digital-thermalright-lcd`.

8.  **Formatting:** Ensure standard markdown, centered header using `<div>`.

9.  **Review against constraints:**
    *   90-120 lines? Yes, by adding spacing between sections and proper formatting of the table and links.
    *   No fluff? Yes.
    *   Real technical depth? Yes (sm_61, EXL2, VRAM monitoring, PWM).

    *Self-Correction during drafting:* Make sure not to use emojis in the section headers since I used them in the main header (limit is 2 total).
    *Header Emojis:* 🧠 ⚡

    *Slug Check:*
    *   `cuda-sm61-compatibility-shim` (from `cuda-sm61-compatibility-shim`)
    *   `add-video-input-support-to-llamacpp-mtmd` (from `add-video-input-support-to-llamacpp-mtmd`)
    *   `automated-exl2-conversion-validation-pipeline` (from `automated-exl2-conversion-validation-pipeline`)
    *   `auto-quantization-pipeline-gguf` (from `auto-quantization-pipeline-gguf`)
    *   `ai-dashboard` (from `ai-dashboard`)
    *   `advanced-ai-boot-watchdog` (from `automazione-bootwatchdog-ai-avanzato`)
    *   `git-mcp-server` (from `git-mcp-server-per-agenti-ai`)
    *   `mtop-llm-monitor` (from `mtop: htop per monitoraggio LLM locale`)
    *   `reddit-monitor` (from `reddit-monitor`)
    *   `mcp-bridge-claude-code` (from `open-source-mcp-bridge-for-local-claude-code`)
    *   `esp32-tesla-p40-cooling` (from `controller-termico-proattivo-esp32`)
    *   `ai-model-physical-controller` (from `ai-model-selector-physical-controller`)
    *   `edge-vision-node-esp32-s3