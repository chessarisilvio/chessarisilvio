1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Subject:** Silvio Chessari.
    *   **Source Material:** Vault data (Markdown/Obsidian format) detailing projects, paths, and technical details.
    *   **Output Format:** ONLY the final `README.md` markdown. No preamble.
    *   **Tone/Style:** English, professional, technical, precise, no fluff, real technical depth.
    *   **Specific Content Requirements:**
        *   LLM inference research (EAGLE/MTP/speculative decoding/MoE routing).
        *   Running LLMs on unsupported consumer/datacenter GPUs (Tesla P40 sm_61, CUDA workarounds).
        *   Self-built AI infrastructure.
        *   Embedded systems.
    *   **Structure:**
        1.  Centered header.
        2.  3-line technical bio.
        3.  Compact stack table.
        4.  4 Project sections: LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware.
        5.  GitHub stats.
    *   **Project Format:** `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description. Slugs: lowercase, hyphens.
    *   **Constraints:** Max 2 emojis total (header only). 90–120 lines total.

2.  **Analyze the Vault Data (Information Extraction):**

    *   *Meta:* User is Silvio Chessari.
    *   *Themes:* LLMs, Infrastructure (Tesla P40), Embedded (ESP32), Tooling (Python/C++).
    *   *Specific Projects & Details:*

        *   **LLM Research:**
            *   *Add video input support to llama.cpp (mtmd):* CMake mods, video input stub, Python demo with OpenCV.
            *   *Automated EXL2 Conversion & Validation Pipeline:* Fixes Qwen3_5MoeForC architecture, quantization, C++ core.
            *   *Auto-Quantization Pipeline GGUF:* Benchmarking P40/RTX 3050, Q4_K_M vs Q5_K_S.
            *   *Qwen Image Edit Inpainting Workflow:* ComfyUI workflow.
            *   *NLLB Self-Hosted:* Multilingual translation, OCR+MT pipeline.

        *   **AI Infrastructure:**
            *   *AI Dashboard:* http://localhost:9190/, GPU panels, AGENDA.md, 35B local idea gen.
            *   *Openclaw:* Ollama gateway, Node.js.
            *   *Automazione Boot/Watchdog AI Avanzato:* Watchdog for llama-stack, systemd, Telegram alerts, VRAM/token-per-second monitoring.
            *   *CUDA sm_61 Compatibility Shim:* Compatibility for Pascal (Tesla P40).

        *   **Tools & Automation:**
            *   *Megatool:* OSINT C++, Flask web app `:7788`, AI photo analysis.
            *   *Reddit Monitor:* AI/tech subreddit scraper, updates AGENDA.md.
            *   *Git MCP Server for AI Agents:* JSON API for Git.
            *   *Open-source MCP bridge for local Claude Code:* MIT license, HTTP server.
            *   *mtop (htop for LLM):* Real-time GPU/token metrics.
            *   *Silvioprint:* Telegram bot.

        *   **Embedded & Hardware:**
            *   *Controller Termico Proattivo ESP32:* Tesla P40 fan control, DS18B20 sensors, MOSFET PWM, IPMI.
            *   *AI Model Selector Physical Controller:* ESP32, encoder rotary, OLED SSD1306, HID/OpenClaw integration.
            *   *Edge Vision Node ESP32-S3 + moondream:* (Cut off in source, but clear intent).
            *   *Digital Thermal LCD:* LCD temperature display via HID.

3.  **Drafting Content - Section by Section:**

    *   **Header:** Standard centered header.
    *   **Bio:** Needs to hit 3 lines. Focus on: LLM inference engineering, hardware hacking (P40/sm_61), embedded systems integration.
    *   **Stack Table:** Need to infer common tools from the data.
        *   *Languages:* C++, Python, C/CMake.
        *   *ML/AI:* llama.cpp, PyTorch, Ollama, EXL2, GGUF.
        *   *Embedded:* ESP32, C (Arduino style), HID.
        *   *Infra:* Linux, systemd, Node.js, Docker (implied), Flask.

    *   **Project Section 1: LLM Research:**
        *   *add-video-input-support-to-llamacpp-mtmd*
        *   *automated-exl2-conversion-validation-pipeline*
        *   *auto-quantization-pipeline-gguf*
        *   *qwen-image-edit-inpainting-workflow*

    *   **Project Section 2: AI Infrastructure:**
        *   *ai-dashboard*
        *   *openclaw*
        *   *automazione-bootwatchdog-ai-avanzato*
        *   *cuda-sm61-compatibility-shim*

    *   **Project Section 3: Tools & Automation:**
        *   *mtop-htop-per-monitoraggio-llm-locale* (Let's shorten slug to `mtop`)
        *   *git-mcp-server-per-agenti-ai* (`git-mcp-server`)
        *   *open-source-mcp-bridge-for-local-claude-code* (`mcp-bridge-claude-code`)
        *   *megatool*
        *   *reddit-monitor*

    *   **Project Section 4: Embedded & Hardware:**
        *   *controller-termico-proattivo-esp32* (`tesla-p40-esp32-controller`)
        *   *ai-model-selector-physical-controller* (`ai-model-selector-hardware`)
        *   *edge-vision-node-esp32-s3-moondream* (`edge-vision-esp32`)
        *   *digital-thermal-lcd*

    *   **GitHub Stats:** Placeholders for standard stats images/shields.

4.  **Refining and Formatting (Iterative Polish):**

    *   *Constraint Check:* Line count target (90-120). Need to be concise but detailed enough. No fluff.
    *   *Slug Logic:* Lowercase, hyphens.
    *   *Bio Draft:* Specialized in high-performance inference and low-level hardware optimization. Architect of local AI stacks integrating custom CUDA workarounds for legacy GPUs (Tesla P40/sm_61). Expert in embedded systems bridging physical controllers with large model services.
    *   *Descriptions:* Must be 1 line per project, technical.

    *   *Drafting Project Descriptions:*
        *   `add-video-input-support-to-llamacpp-mtmd`: Implements video frame capture and transmission via modified llama.cpp CMake builds with OpenCV Python demo.
        *   `automated-exl2-conversion-validation-pipeline`: C++ toolchain for fixing Qwen3.5 MoE arch, EXL2 conversion, mixed quantization, and automated validation.
        *   `auto-quantization-pipeline-gguf`: Automated benchmarking pipeline for Tesla P40/RTX3050 to optimize GGUF quantization (Q4/Q5).
        *   `ai-dashboard`: Local monitoring webstack (`:9190`) tracking GPU metrics, systemd services, and a 35B-powered AGENDA generator.
        *   `cuda-sm61-compatibility-shim`: Compatibility layer enabling modern LLM toolchains on Pascal architecture (Tesla P40, sm_61).
        *   `automazione-bootwatchdog-ai-avanzato`: Systemd watchdog monitoring `llama-stack` VRAM and token throughput with Telegram-based alerting.
        *   `mtop`: Real-time CLI monitor (htop-like) visualizing local LLM inference metrics, GPU load, and token generation speeds.
        *   `git-mcp-server`: JSON-RPC API server enabling AI agents to perform Git operations via the Model Context Protocol.
        *   `controller-termico-proattivo-esp32`: ESP32 firmware proactively regulating Tesla P40 fan speeds via PWM based on DS18B20 thermal sensors.
        *   `ai-model-selector-physical-controller`: Physical ESP32 interface with rotary encoder and OLED for switching local AI models via HID.
        *   `megatool`: Full-stack OSINT suite combining C++ backend, Flask web interface, and AI photo analysis pipelines.

5.  **Final Assembly & Review:**

    *   *Emojis:* Add 2 max in header. Let's use 💻 and ⚙️.
    *   *Line Count Check:* I need to make sure I don't use too much whitespace or verbose text. The structure needs to be tight.
    *   *Tone Check:* Is it "technical, precise"? Yes.
    *   *Bio Check:* 3 lines? Yes.

6.  **Constructing the Markdown:** (Self-Correction during drafting)
    *   *Slug:* `controller-termico-proattivo-esp32` -> `tesla-p40-thermal-controller` (Better, shorter).
    *   *Slug:* `ai-dashboard` -> `ai-dashboard`.
    *   *Slug:* `mtop-htop-per-monitoraggio-llm-locale` -> `mtop-llm-monitor`.

    *   *Bio:*
        Silvio Chessari | High-Performance Inference Engineer
        Architecting self-hosted AI infrastructure with a focus on speculative decoding, MoE routing, and CUDA optimization for legacy hardware.
        Bridging the gap between embedded systems (ESP32) and large-scale model deployment through custom firmware and automation tooling.

    *   *Stack Table:*
        Languages | C++, Python, Bash, CMake, Lua
        ML/AI | llama.cpp, EXL2, GGUF, Ollama, ComfyUI
        Embedded | ESP32, Arduino Core, HID, 1-Wire, PWM
        Infra | Linux (systemd), Node.js, Flask, Docker

    *   *Projects:*
        Group 1: LLM Research
        Group 2: AI Infrastructure
        Group 3: Tools & Automation
        Group 4: Embedded & Hardware

    Let's assemble.

    *Counting lines:*
    Header: 4 lines
    Bio: 3 lines
    Stack: 4 lines
    Dividers: 4 lines
    Projects: ~12 lines (3 per section approx)
    Stats: 3 lines
    Total body content: ~30 lines.
    *Wait,* the prompt asks for **90–120 lines total**. 30 lines is way too short.
    *Adjustment:* I need to expand the descriptions slightly or add more technical detail per project, or create a more dense structure.
    *Re-reading requirement:* "1-line technical description" per project.
    *Wait*, "1-line" usually means a single sentence. If I have 4 sections x 3 projects = 12 projects. 12 lines of text. Total file will be <50 lines.
    *Correction:* Maybe "90-120 lines" is a constraint to ensure *enough* detail? Or maybe I should include *more* projects or make the bio/stack longer?
    *Let's look at the vault data again.* There are many entries.
    *Strategy:* I will increase the project count per section to hit the line count, or add a "Technical Focus" section? No, requirements say: "Structure: centered header → 3-line technical