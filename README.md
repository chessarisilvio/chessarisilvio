1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **User:** Silvio Chessari.
    *   **Task:** Generate a professional GitHub `README.md` based on provided vault data.
    *   **Constraints:**
        *   Output ONLY the final markdown (no preamble, no explanation).
        *   Language: English, technical, precise (no fluff).
        *   Content Focus: LLM inference research (EAGLE, MTP, speculative decoding, MoE routing), running LLMs on unsupported GPUs (Tesla P40 sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.
        *   Structure:
            1.  Centered header.
            2.  3-line technical bio.
            3.  Compact stack table.
            4.  4 project sections (LLM Research, AI Infrastructure, Tools & Automation, Embedded & Hardware).
            5.  GitHub stats (image).
        *   Project format: `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description. Slug must be lowercase hyphens.
        *   Emojis: Max 2 total (header only).
        *   Length: 90–120 lines.

2.  **Analyze the Vault Data:**
    *   *User Info:* Silvio Chessari.
    *   *Themes:* Local LLM inference, CUDA workarounds (sm_61), GGUF, EXL2, automation (Benchmarking, Watchdogs), embedded (Arduino R4, ESP32), C++/Python.
    *   *Specific Projects:*
        *   `Sistema di Benchmarking Automatizzato per Nuovi Modelli GGUF`: Benchmarking GGUF (P40/RTX3050), auto reports.
        *   `AI Home Assistant HID Dashboard`: Arduino R4 WiFi, ESP32, MQTT/Tailscale for local AI monitoring.
        *   `AI Dashboard`: Python script `:9190`, worker sub-tasks, GPU/Service monitoring.
        *   `Secure LLM Context Vault`: Secure context storage.
        *   `bot-short`: C++ Telegram bot, AI vector graphics (SVG).
        *   `Controller Termico ESP32`: Fan control + sensors.
        *   `Megatool`: C++ OSINT + Flask web app + AI photo analysis.
        *   `VideoStudio`: Python backend, Spot AI from photos (LLM storyboard + Higgsfield clips).
        *   `Openclaw`: Node.js Ollama gateway.
        *   `Reddit Monitor`: Subreddit AI/tech scraping → AGENDA.md.
        *   `Silvioprint`: Telegram content bot.
        *   `Silvioprint — Sito Web`: Static HTML/CSS/JS e-commerce.
        *   `Automazione Boot/Watchdog AI Avanzato`: Watchdog for llama-stack, VRAM/tok/s monitoring, Telegram notifications, systemd.
        *   `cuda-sm61-compatibility-shim`: CUDA sm_61 shim for Pascal (Tesla P40).
        *   `add-video-input-support-to-llamacpp-mtmd`: Video input for llama.cpp, OpenCV.
        *   `AI Model Selector Physical Controller`: ESP32, rotary encoder, OLED, HID interface.
        *   `Automated EXL2 Conversion & Validation Pipeline`: C++ core, Python CLI, Qwen3_5MoeForC fix, mixed precision quantization.
        *   `NLLB Self-Hosted`: Offline NLLB-200 translation.

3.  **Drafting - Section by Section:**

    *   **Header:** `<br><div align="center"> <h1 align="center">Silvio Chessari</h1> ... </div>`
    *   **Bio:** Focus on LLM inference research (EAGLE, MoE), CUDA optimization on legacy hardware (sm_61), and embedded AI integration.
    *   **Stack Table:** Needs to cover Python, C++, CUDA, Arduino/ESP32, Linux/Shell, GGUF/EXL2.

    *   **Section 1: LLM Research & Optimization**
        *   *Project Ideas:* Video input support, EXL2 pipeline, CUDA shim, Quantization pipeline.
        *   *Selection:*
            1.  `Add Video Input Support to llama.cpp` (mtmd) -> `add-video-input-support-to-llamacpp-mtmd`
            2.  `Automated EXL2 Conversion & Validation Pipeline` -> `automated-exl2-conversion-validation-pipeline`
            3.  `Auto-Quantization Pipeline GGUF` -> `auto-quantization-pipeline-gguf`
            4.  `CUDA sm_61 Compatibility Shim` -> `cuda-sm61-compatibility-shim`
    
    *   **Section 2: AI Infrastructure**
        *   *Project Ideas:* AI Dashboard, Openclaw, Watchdog.
        *   *Selection:*
            1.  `AI Dashboard` -> `ai-dashboard`
            2.  `Automazione Boot/Watchdog AI Avanzato` -> `automazione-bootwatchdog-ai-avanzato`
            3.  `Openclaw` -> `openclaw`
            4.  `Secure LLM Context Vault` -> `secure-llm-context-vault`

    *   **Section 3: Tools & Automation**
        *   *Project Ideas:* Megatool, Reddit Monitor, Silvioprint, VideoStudio.
        *   *Selection:*
            1.  `Megatool` -> `megatool`
            2.  `VideoStudio` -> `videostudio`
            3.  `Reddit Monitor` -> `reddit-monitor`
            4.  `bot-short` -> `bot-short` (Fits here as a tool)

    *   **Section 4: Embedded & Hardware**
        *   *Project Ideas:* HID Dashboard, AI Model Selector, ESP32 Thermal Controller.
        *   *Selection:*
            1.  `AI Home Assistant HID Dashboard` -> `ai-home-assistant-hid-dashboard`
            2.  `AI Model Selector Physical Controller` -> `ai-model-selector-physical-controller`
            3.  `Controller Termico ESP32` -> `controller-termico-proattivo-esp32`

    *   **GitHub Stats:** Standard visitor count image.

4.  **Refining the Content (Technical Tone & Constraints):**
    *   *Bio Check:* Needs to mention EAGLE/MTP/Speculative decoding/MoE routing explicitly as per requirements ("Show real technical depth..."). Even though specific files for EAGLE/MTP aren't in the detailed project list, the prompt explicitly asks the writer to *include* these depth areas. I will integrate them into the bio and imply them in the descriptions where appropriate (e.g., the EXL2 pipeline fixing MoE architectures).
    *   *Slugs:* Ensure lowercase-hyphenate.
    *   *Descriptions:* One liners, technical.

    *   *Drafting Bio:*
        Focused on LLM inference efficiency through speculative decoding (EAGLE/MTP) and routing optimization. Specialist in running large models on consumer/legacy hardware (CUDA sm_61, Tesla P40) via custom shims and quantization pipelines. Bridges high-performance AI research with embedded systems and physical interfaces.

    *   *Drafting Descriptions:*
        *   `add-video-input...`: Extends llama.cpp for multimodal video inference via OpenCV frame injection and CMake integration.
        *   `automated-exl2...`: C++/Python toolchain for Qwen3.5 MoE architecture fixing, mixed-precision EXL2 quantization, and validation.
        *   `cuda-sm61...`: Compatibility layer enabling modern CUDA workloads on Pascal architecture (Tesla P40 sm_61).
        *   `ai-dashboard`: Local monitoring stack tracking GPU VRAM, token throughput, and systemd services via Python web server.
        *   `automazione-bootwatchdog...`: Systemd watchdog monitoring llama-stack health, VRAM leaks, and inference rates with Telegram alerts.

5.  **Format Check & Length Estimation:**
    *   90–120 lines.
    *   No emojis in body.
    *   Proper Markdown structure.

6.  **Final Polish (Self-Correction during drafting):**
    *   *Prompt Requirement:* "Show real technical depth: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing)" -> I will put this in the bio explicitly.
    *   *Prompt Requirement:* "Running LLMs on unsupported consumer/datacenter GPUs (Tesla P40 sm_61, CUDA workarounds)" -> Bio and Shim project description.
    *   *Repo URL:* `https://github.com/chessarisilvio/slug`.

7.  **Constructing the Final Output (Mental Simulation):**

    ```markdown
    <br>
    <div align="center">...</div>

    Technical specialist focused on LLM inference efficiency via EAGLE/MTP speculative decoding and MoE routing strategies. Expert in deploying large models on legacy hardware (Tesla P40 sm_61) through CUDA workarounds and custom quantization pipelines. Architect of self-hosted AI infrastructure and embedded control systems.

    ### Tech Stack
    | Category | Technologies |
    | ...
    ```

    *Filling the sections...*

    *LLM Research*
    - [Add Video Support...](...) Extends llama.cpp...
    - [Automated EXL2...](...) C++/Python toolchain...

    *AI Infrastructure*
    - [AI Dashboard](...) Python-based...
    - [Openclaw](...) Node.js gateway...

    *Tools & Automation*
    - [Megatool](...) C++ OSINT...
    - [Bot Short](...) C++ Telegram...

    *Embedded & Hardware*
    - [AI Home Assistant...](...) Arduino R4...
    - [AI Model Selector](...) ESP32...

    *Stats*

8.  **Final Line Count Check:**
    Header: ~10 lines.
    Bio: ~4 lines.
    Stack: ~7 lines.
    Sections: ~4 headers + 3 projects *4 sections = 12 projects + spacing ~30-40 lines.
    Stats: ~5 lines.
    Total ~60-70 lines. I need to ensure it hits the requested 90-120 lines. To achieve this, I will expand the descriptions slightly within the constraints (1 line technically, but maybe slightly longer or break lines logically) or add spacing, but the prompt says "1-line technical description". To reach 90 lines, I might need to ensure the markdown formatting (tables, spacing) is verbose enough, or perhaps the header and stack sections take up more vertical space. Actually, standard markdown spacing often consumes lines. I will ensure the descriptions are dense and precise.

    *Re-evaluating Line Count Strategy:*
    If I strictly follow "1-line technical description", I might fall short of lines. However, "1-line" usually means a single sentence or sentence fragment,未必 a physical line if using code blocks or tables. I will focus on the *density* of information. The prompt asks for 90-120 lines. Let's make the stack table detailed and the layout airy but dense in content.

    *Wait*, re-reading: "For each project... + 1-line technical description".
    If I have 12 projects, that's 12 lines. 4 headers = 4 lines. 3 bio lines = 3 lines. Header = 5 lines. Stack = 5 lines.
    That's ~30 lines of content. How to get to 90-120?
    Maybe the user means the *file