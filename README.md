1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Subject:** Silvio Chessari.
    *   **Output:** GitHub `README.md` markdown file.
    *   **Requirements:**
        *   Output *only* the markdown (no preamble/explanation).
        *   Style: English, technical, precise, no fluff.
        *   Technical Depth: Focus on LLM inference research (EAGLE, speculative decoding, MoE routing), running LLMs on unsupported GPUs (Tesla P40 sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.
        *   Structure:
            1.  Centered header.
            2.  3-line technical bio.
            3.  Compact stack table.
            4.  4 Project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware).
            5.  GitHub stats (image placeholder).
        *   Project Format: `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
        *   Repo Slugs: Derived from project names (lowercase, hyphens).
        *   Emojis: Max 2 (header only).
        *   Length: 90–120 lines total.
    *   **Source Data:** Provided "vault data" (Obsidian notes style) containing project lists, taxonomy, and descriptions.

2.  **Process Source Data & Extract Key Info:**

    *   *Bio Keywords:* AI infrastructure, LLM inference, Tesla P40, CUDA compatibility, speculative decoding, embedded systems, automation.
    *   *Stack:* C++, Python, ESP32, CUDA, Node.js, Flask, GGUF, EXL2.
    *   *Projects Mapping:*

        *   *LLM Research:*
            *   `add-video-input-support-to-llamacpp-mtmd`: Video input for llama.cpp (CMake, OpenCV).
            *   `automated-exl2-conversion-validation-pipeline`: EXL2 conversion, Qwen3.5 MoE, mixed quantization.
            *   `auto-quantization-pipeline-gguf`: Automated GGUF quantization, benchmarking on P40/RTX3050.
            *   `bias-personalizzato-per-whisper-locale`: Whisper bias injection via JSON/TSV.
            *   `qwen-image-edit-inpainting-workflow`: ComfyUI workflow for Qwen.

        *   *AI Infrastructure:*
            *   `ai-dashboard`: Web dashboard (port 9190), AGENDA.md, 35B local generation.
            *   `automazione-bootwatchdog-ai-avanzato`: Watchdog for llama-stack, VRAM monitoring, Telegram notifications.
            *   `git-mcp-server-per-agenti-ai`: MCP server for Git operations.
            *   `openclaw`: Node.js Ollama gateway.
            *   `nllb-self-hosted-per-testo-multilingua`: Offline NLLB-200, OCR+MT pipeline.

        *   *Tools & Automation:*
            *   `sviluppati/sistema-di-benchmarking-automatizzato-per-nuovi-mo`: GGUF benchmarking on P40/RTX3050.
            *   `reddit-monitor`: Subreddit monitoring, feeding AGENDA.md.
            *   `mtop-htop-per-monitoraggio-llm-locale`: htop-like LLM monitor, real-time GPU/token metrics.
            *   `silvioprint`: Telegram content bot.
            *   `cache-plan-logic-for-recurring-queries`: Semantic caching for LLM plans.

        *   *Embedded & Hardware:*
            *   `controller-termico-proattivo-esp32`: Proactive fan control for Tesla P40, ESP32.
            *   `ai-model-selector-physical-controller`: ESP32 rotary encoder, OLED, HID/Gateway integration.
            *   `digital-thermal-lcd`: Thermalright LCD, HID interface.
            *   `cuda-sm61-compatibility-shim`: Pascal (P40) compatibility.

3.  **Drafting Content - Section by Section:**

    *   *Header:* Center `<h1>` with max 2 emojis.
        *   "Silvio Chessari 🧠 ⚙️" (Brains + Gears fits the tech/infra vibe).

    *   *Bio:* 3 lines.
        *   L1: Focus on LLM inference optimization and proprietary hardware workarounds (Tesla P40/sm_61).
        *   L2: Building self-hosted AI infrastructure with automation and real-time monitoring pipelines.
        *   L3: Developing embedded interfaces and tools for local model deployment and hardware control.

    *   *Stack Table:* Compact.
        *   Languages: C++, Python, Bash.
        *   Hardware/Infra: Tesla P40, ESP32, CUDA, GGUF, EXL2.
        *   Tools: Ollama, Node.js, Flask, OpenCV, ComfyUI.

    *   *Project Sections:*
        *   **LLM Research & Inference**
            *   [Auto-Quantization Pipeline GGUF](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) -> Automated GGUF quantization, benchmarking, and validation on Tesla P40 and RTX 3050.
            *   [Automated EXL2 Conversion Pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) -> Toolchain for Qwen3.5 MoE EXL2 conversion, quantization tuning, and validation.
            *   [Video Input to llama.cpp](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) -> Implementation of video input via CMake patches and OpenCV integration for multimodal inference.
            *   [Cache Plan Logic](https://github.com/chessarisilvio/cache-plan-logic-for-recurring-queries) -> Semantic caching for LLM action plans to reduce latency on local 35B models.
            *   [Whisper Bias Module](https://github.com/chessarisilvio/bias-personalizzato-per-whisper-locale) -> Customizable JSON/TSV bias injection and contextual correction for local Whisper transcription.

        *   **AI Infrastructure & Monitoring**
            *   [AI Dashboard](https://github.com/chessarisilvio/ai-dashboard) -> Local web interface (port 9190) for GPU monitoring, AGENDA management, and worker orchestration.
            *   [Advanced AI Watchdog](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) -> Systemd watchdog monitoring llama-stack VRAM and TPS with Telegram failover notifications.
            *   [Git MCP Server](https://github.com/chessarisilvio/git-mcp-server-per-agenti-ai) -> Model Context Protocol server enabling Git operations for local AI agents.
            *   [mtop: LLM Monitor](https://github.com/chessarisilvio/mtop-htop-per-monitoraggio-llm-locale) -> Real-time htop-like terminal utility for local LLM token throughput and GPU utilization.

        *   **Tools & Automation**
            *   [GGUF Benchmarking System](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-mo) -> Automated benchmarking suite for GGUF models across legacy P40 and consumer GPUs.
            *   [Reddit Monitor](https://github.com/chessarisilvio/reddit-monitor) -> Script that scans AI/tech subreddits to populate the AGENDA.md with fresh ideas every 3 hours.
            *   [Bot Short](https://github.com/chessarisilvio/bot-short) -> C++ Telegram bot generating AI-driven vector graphics (SVG/EPS) via serverless pipeline.
            *   [OpenClaw](https://github.com/chessarisilvio/openclaw) -> Node.js gateway providing standardized access to local Ollama instances.

        *   **Embedded & Hardware**
            *   [Proactive Thermal Controller](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) -> ESP32-based fan controller for Tesla P40 utilizing predictive algorithms and sensor data.
            *   [AI Model Selector](https://github.com/chessarisilvio/ai-model-selector-physical-controller) -> Rotary encoder and OLED interface for physical local model switching via HID/gateway.
            *   [CUDA sm_61 Compatibility Shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim) -> Compatibility layer to enable modern LLM runtimes on legacy Pascal architecture GPUs.
            *   [Digital Thermal LCD](https://github.com/chessarisilvio/digital-thermal-lcd) -> HID interfaced LCD display for real-time thermal readings of hardware components.

    *   *GitHub Stats:*
        *   Standard layout: `![stats](...), ![streak](...)`

4.  **Review and Refine:**
    *   *Check Constraints:*
        *   Markdown only? Yes.
        *   English/Technical? Yes.
        *   Deep tech shown? Yes (Pascal, EXL2, GGUF, MoE, ESP32 HID).
        *   Structure correct? Yes.
        *   Slugs correct? Yes.
        *   Line count check:
            *   Header: 3
            *   Bio: 3
            *   Stack: 1 (table) + header = 3
            *   Projects: ~15 items lines + headers = ~30
            *   Stats: 2
            *   Spacing: ~20
            *   Total: ~60-70 lines? A bit short. I should add more detail to the descriptions or ensure the formatting (list spacing) fills it out visually to hit the 90-120 range without adding fluff *text*. I will ensure standard markdown spacing or add a brief "Connect" section if needed, but the requirement implies dense content.
            *   Let's maximize the line count by keeping the list format clean but utilizing the full project list provided in the vault.
            *   *Adjustment:* The prompt asks for Max 2 emojis. I used 2. It asks for 4 project sections. I have 4. It asks for 90-120 lines. I need to make sure I don't compress the list too much. I will put each project on its own line in the markdown source.

5.  **Final Polish of Descriptions:**
    *   *Make them sound sharper.*
    *   Instead of "Toolchain for...", "C++ core and Python CLI for fixing Qwen3 architecture and converting to EXL2."
    *   "Watchdog that monitors..."

6.  **Constructing the Markdown:**

    ```markdown
    <div align="center">
      <h1>Silvio Chessari 🧠 ⚙️</h1>
    </div>

    Focused on LLM inference optimization, speculative decoding, and speculative execution on unsupported architectures (Tesla P40/sm_61).
    Engineering self-hosted AI infrastructure featuring automated pipelines, CUDA workarounds, and real-time monitoring embedded systems.
    Developing local-first solutions for MoE routing, multimodal inputs, and hardware-controlled model orchestration.

    ### Technical Stack

    | **Core** | **Hardware** | **Infra** | **AI/ML** |
    | :--- | :--- | :--- | :--- |
    | C++, Python, Bash | Tesla P40, ESP32, | Docker, Systemd, | GGUF, EXL2, |
    | Node.js, CMake | CUDA (sm