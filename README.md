1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Output:** Professional GitHub `README.md` markdown.
    *   **User:** Silvio Chessari.
    *   **Constraints:**
        *   Output ONLY the markdown. No preamble, no explanation.
        *   Language: English, technical, precise, no fluff.
        *   Content: Real technical depth (LLM inference research EAGLE/MTP/MoE, CUDA workarounds for Tesla P40, self-built AI infrastructure, embedded systems).
        *   Data Source: "VAULT DATA" provided in the prompt.
        *   Structure: Centered header -> 3-line technical bio -> compact stack table -> 4 project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware) -> GitHub stats.
        *   Project Links: `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
        *   Slug format: lowercase, hyphens.
        *   Emojis: Max 2 (header only). Clean prose elsewhere.
        *   Length: 90–120 lines.

2.  **Analyze the Vault Data:**
    *   *Panoramica:* Structure of projects (developed, llm-stack, services, research, ideas).
    *   *Sviluppati (Developed):*
        *   `ai-dashboard`: Dashboard web (9190), AGENDA.md, worker tasks.
        *   `bot-short`: C++ Telegram bot, AI vector graphics, SVG pipeline.
        *   `controller-termico-proattivo-esp32`: ESP32, Tesla P40 Fan control, proactive.
        *   `digital-thermal-lcd`: LCD display temp via HID (Thermalright).
        *   `megatool`: OSINT C++, Flask web app (7788), AI photo analysis.
        *   `openclaw`: Ollama gateway, Node.js.
        *   `reddit-monitor`: AI/tech subreddit monitor -> AGENDA.md.
        *   `silvioprint`: Bot Telegram contents.
        *   `automazione-bootwatchdog-ai-avanzato`: Watchdog for llama-stack, systemd, Telegram notifications.
        *   `launcher-avanzato-per-llama-server`: Advanced launcher.
        *   `cuda-sm61-compatibility-shim`: Pascal (Tesla P40) compatibility.
        *   `add-video-input-support-to-llamacpp-mtmd`: Video input to llama.cpp, OpenCV, CMake.
        *   `ai-model-selector-physical-controller`: ESP32 physical selector, rotary encoder, OLED.
        *   `automated-exl2-conversion-validation-pipeline`: Qwen3_5Moe fix, quantization, C++/Python.
        *   `nllb-self-hosted-per-testo-multilingua`: NLLB-200 offline, OCR+MT pipeline.
        *   `mtop-htop-per-monitoraggio-llm-locale`: htop-like for LLM inference (GPU/token metrics).
        *   `git-mcp-server-per-agenti-ai`: MCP server for Git, JSON API.
        *   `qwen-image-edit-inpainting-workflow`: ComfyUI, Qwen Image Edit.
        *   `open-source-mcp-bridge-for-local-claude-code`: MCP bridge for Claude Code, HTTP server.
        *   `edge-vision-node-esp32-s3-moondream`: ESP32-S3 + moondream.
    *   *Specific Project Details (Added later in data):*
        *   `add-video-input-support-to-llamacpp-mtmd`: CMake changes, stub input, Python demo.
        *   `ai-dashboard`: Monitoring, automation, 35B local idea generator.
        *   `ai-model-selector-physical-controller`: ESP32, rotary encoder, HID/OpenClaw integration.
        *   `auto-quantization-pipeline-gguf`: Benchmark P40/RTX3050, Q4 vs Q5 quantization, auto-GGUF generation.
        *   `automated-exl2-conversion-validation-pipeline`: Mixtral/Qwen MoE architecture fix, mixed quantization.
        *   `automazione-bootwatchdog-ai-avanzato`: Process/VRAM/token rate monitoring.
        *   `bot-short`: C++ Telegram bot, SVG/EPS.
        *   `controller-termico-proattivo-esp32`: Tesla P40 specific, DS18B20 sensors, PWM fan control.
        *   `digital-thermal-lcd`: Thermalright LCD, HID.
        *   `edge-vision-node-esp32-s3-moondream`: ESP32-S3 vision node.

3.  **Drafting - Section by Section:**

    *   **Header:** Centered. Name (Silvio Chessari). Emojis: 🔬 (Research) ⚙️ (Systems) or similar.
    *   **Bio:** 3 lines. Needs to cover LLM inference research (EAGLE/MTP/MoE, speculative decoding), running LLMs on unsupported GPUs (Tesla P40 sm_61), embedded systems (ESP32, sensors).
        *   *Draft:* Specializing in high-efficiency LLM inference research and speculative decoding, focusing on EAGLE/MTP and MoE routing optimization. Expert in deploying large-scale AI on unsupported consumer hardware, including CUDA shims for Tesla P40 (sm_61). Architected self-hosted AI infrastructure integrating embedded systems (ESP32) with local inference clusters.

    *   **Stack Table:** Compact. Columns: Domain | Tech.
        *   Inference: llama.cpp, EXL2, vLLM, Ollama.
        *   Hardware: Tesla P40, RTX 3050, ESP32, S3.
        *   Languages: C++, Python, CUDA, Node.js.
        *   Tools: Flask, Systemd, ComfyUI, OpenCV.

    *   **Project Section 1: LLM Research**
        *   *Selection:* `automated-exl2-conversion-validation-pipeline`, `add-video-input-support-to-llamacpp-mtmd`, `cuda-sm61-compatibility-shim`.
        *   *Descriptions:* Focus on the technical depth.
            *   EXL2: Qwen/MoE architecture fix, EXL2 conversion, mixed quantization, benchmarking.
            *   llama.cpp video: Video frame acquisition, CMake integration, OpenCV pipeline.
            *   sm61 shim: Pascal GPU compatibility, CUDA workarounds.

    *   **Project Section 2: AI Infrastructure**
        *   *Selection:* `ai-dashboard`, `auto-quantization-pipeline-gguf`, `open-source-mcp-bridge-for-local-claude-code`.
        *   *Descriptions:*
            *   Dashboard: Web monitoring (9190), local 35B model generation, AGENDA.md integration.
            *   GGUF Pipeline: Automated benchmark (P40/3050), Q4/Q5 selection, Obsidian vault updates.
            *   MCP Bridge: Claude Code integration, HTTP server, MIT license.

    *   **Project Section 3: Tools & Automation**
        *   *Selection:* `mtop-htop-per-monitoraggio-llm-locale`, `git-mcp-server-per-agenti-ai`, `bot-short`, `reddit-monitor`.
        *   *Descriptions:*
            *   mtop: htop-like real-time GPU/token metrics for local inference.
            *   Git MCP: JSON API for Git operations via AI agents.
            *   bot-short: C++ Telegram bot, AI SVG/EPS vector graphics, Flask web app.
            *   reddit-monitor: Scrapes AI/tech subreddits, populates AGENDA.md via local parsing.

    *   **Project Section 4: Embedded & Hardware**
        *   *Selection:* `controller-termico-proattivo-esp32`, `digital-thermal-lcd`, `ai-model-selector-physical-controller`, `edge-vision-node-esp32-s3-moondream`.
        *   *Descriptions:*
            *   Controller: ESP32 firmware for Tesla P40 fan control, proactive PWM, DS18B20 sensors.
            *   LCD: Thermalright LCD HID integration, real-time system temp display.
            *   Physical Selector: ESP32 rotary encoder + OLED, HID commands for model switching.
            *   Edge Vision: ESP32-S3 node integrated with moondream for on-device vision.

    *   **GitHub Stats:** Standard placeholder for streak/commits. (Will use standard syntax `![Stats]...`).

4.  **Refining and Formatting:**

    *   *Slugs:* Must be `https://github.com/chessarisilvio/[slug]`.
    *   *Line Count Check:* The prompt asks for 90–120 lines. I need to ensure spacing is efficient but sufficient.
    *   *Language:* strictly English.
    *   *Technical Check:* Mention "sm_61", "speculative decoding", "MoE", "vLLM", "Tesla P40".

5.  **Constructing the Markdown (Mental or Scratchpad):**

    *   *Header:*
        ```markdown
        # <div align="center">Silvio Chessari 🔬 ⚙️</div>
        ```
    *   *Bio:*
        ```markdown
        <div align="center">
        <br>
        Researching high-efficiency LLM inference and decoding strategies (EAGLE/MTP, speculative decoding, MoE routing) on resource-constrained hardware.
        Architecting self-hosted AI stacks and CUDA compatibility shims for unsupported GPUs (Tesla P40 sm_61).
        Building the bridge between embedded systems and server-side inference via custom firmware and automation pipelines.
        <br>
        </div>
        ```
    *   *Stack:*
        ```markdown
        <table align="center">
        <tr><th>Inference</th><th>Hardware</th><th>Stack</th></tr>
        <tr><td>llama.cpp • vLLM • EXL2 • Ollama</td><td>Tesla P40 • RTX 3050 • ESP32 • ESP32-S3</td><td>C++ • Python • CUDA • Node.js • Flask</td></tr>
        </table>
        ```
    *   *Projects:* (Need to group strictly as requested: LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware).

    *   *LLM Research:*
        *   [Automated EXL2 Conversion & Validation Pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) - Fixes Qwen/MoE architectures, converts to EXL2, applies mixed quantization, and runs validation benchmarks.
        *   [Add Video Input to llama.cpp (mtmd)](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) - Implements video frame capture via CMake and OpenCV, extending multimodal support for local inference.
        *   [CUDA sm_61 Compatibility Shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim) - Enables modern LLM runtime execution on legacy Pascal GPUs (Tesla P40) by overriding SM arch checks.

    *   *AI Infrastructure:*
        *   [AI Dashboard + Agenda](https://github.com/chessarisilvio/ai-dashboard) - Local web interface (:9190) for GPU monitoring, integrated with a 35B model for automated idea generation.
        *   [Auto-Quantization Pipeline GGUF](https://github.com/chessarisilvio/auto-quantization-p