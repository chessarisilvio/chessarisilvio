1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Goal:** Generate a professional GitHub profile README.md for "Silvio Chessari".
    *   **Input:** Technical Vault Data (Obsidian notes/Markdown). Data includes Italian project descriptions, taxonomy, and detailed specs for hardware/software projects (LLM inference, CUDA, embedded systems).
    *   **Constraints:**
        *   Output *only* the final README.md markdown (no preamble, no explanation).
        *   English, technical, precise tone (no fluff).
        *   Highlight specific technical depth: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), unsupported GPUs (Tesla P40 sm_61, CUDA workarounds), AI infrastructure, embedded systems.
        *   Structure: Centered header -> 3-line bio -> Compact stack table -> 4 project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware) -> GitHub stats.
        *   Project format: `[name](https://github.com/chessarisilvio/slug)` + 1-line description.
        *   Repo slugs: derived from project names (lowercase, hyphens).
        *   Max 2 emojis total (header only).
        *   Length: 90–120 lines.

2.  **Analyze the Vault Data (Source Material Extraction):**

    *   *User Identity:* Silvio Chessari (`chessarisilvio` is implied as the GitHub handle).
    *   *Core Focus:* LLM Research, AI Infrastructure, Hardware Modding (Tesla P40), Embedded (ESP32).

    *   *Project Categories & Specific Entries:*

        *   **LLM Research:**
            *   *Add video input support to llama.cpp (mtmd)*: Video frame acquisition, CMake modifications.
            *   *Automated EXL2 Conversion & Validation Pipeline*: Fixing Qwen3_5MoeForC architecture, mixed quantization, C++ core + Python CLI.
            *   *Bias personalizzato per Whisper locale*: Bias module (JSON/TSV), LLM correction.

        *   **AI Infrastructure:**
            *   *AI Dashboard + Agenda*: Web dashboard (port 9190), monitoring GPU/System/Agenda, idea generation via local 35B model.
            *   *Automazione Boot/Watchdog AI Avanzato*: Monitor llama-stack (process, VRAM, t/s), Telegram notifications, systemd integration.
            *   *Auto-Quantization Pipeline GGUF*: Benchmarking (Tesla P40/RTX 3050), selecting Q4/Q5 points.

        *   **Tools & Automation:**
            *   *bot-short*: C++, Telegram bot, AI vector graphics (SVG/EPS).
            *   *Megatool*: OSINT C++, Flask web app (:7788), AI photo analysis.
            *   *Openclaw*: Gateway Ollama, Node.js.
            *   *Reddit Monitor*: Subreddit scraping, idea generation to AGENDA.md.

        *   **Embedded & Hardware:**
            *   *Controller Termico ESP32*: Tesla P40 fan control, DS18B20 sensors, MOSFET PWM, IPMI communication.
            *   *Digital Thermal LCD*: LCD temp display via HID.
            *   *AI Model Selector Physical Controller*: ESP32, rotary encoder, OLED SSD1306, HID integration.

3.  **Drafting the Content (Iterative Refinement):**

    *   *Header:* Needs name and role.
    *   *Bio:* High-level summary.
        *   Draft 1: Silvio Chessari. Deep learning researcher specializing in speculative decoding and MoE routing. Expert in running inference on legacy hardware and building DIY AI infrastructure.
        *   Draft 2 (More precise): Researching LLM inference acceleration (EAGLE/MTP, speculative decoding) and pushing consumer/legacy hardware limits (Tesla P40 sm_61 compatibility). designing self-hosted AI infrastructure, embedded control systems, and automation pipelines.

    *   *Stack Table:* Needs to cover languages/tools.
        *   C++, Python, CMake, CUDA, Node.js, Flask, ESP32 (C++), Bash, OpenCV, Telegram API.

    *   *Project Section 1: LLM Research*
        *   *Slug:* `add-video-input-support-to-llamacpp-mtmd` -> `add-video-input-llamacpp`
        *   *Slug:* `automated-exl2-conversion-validation-pipeline` -> `automated-exl2-conversion-validation`
        *   *Slug:* `bias-personalizzato-per-whisper-locale` -> `custom-bias-whisper-local`

    *   *Project Section 2: AI Infrastructure*
        *   *Slug:* `ai-dashboard` -> `ai-dashboard`
        *   *Slug:* `automazione-bootwatchdog-ai-avanzato` -> `advanced-ai-boot-watchdog`
        *   *Slug:* `auto-quantization-pipeline-gguf` -> `auto-quantization-pipeline-gguf`

    *   *Project Section 3: Tools & Automation*
        *   *Slug:* `bot-short` -> `bot-short`
        *   *Slug:* `megatool` -> `megatool`
        *   *Slug:* `openclaw` -> `openclaw`
        *   *Slug:* `reddit-monitor` -> `reddit-monitor`

    *   *Project Section 4: Embedded & Hardware*
        *   *Slug:* `controller-termico-proattivo-esp32` -> `tesla-p40-esp32-fan-controller`
        *   *Slug:* `digital-thermal-lcd` -> `digital-thermal-lcd`
        *   *Slug:* `ai-model-selector-physical-controller` -> `ai-model-selector-hardware`

    *   *Stats Section:* Standard GitHub stats image + generic contributions code block.

4.  **Formatting and Refining (Checking constraints):**

    *   *Language:* English, technical.
    *   *Tone:* Precise.
    *   *Emojis:* Max 2 in header only.
    *   *Lines:* Keep it compact to fit 90-120 lines. This means avoiding excessive vertical spacing.

    *   *Refining Descriptions:*
        *   *Video input:* Extended llama.cpp to ingest video frames via CMake stubs and Python/OpenCV bindings for multimodal inference.
        *   *EXL2 Pipeline:* C++ toolchain to fix Qwen3_5 MoE architecture, convert to EXL2, and validate mixed quantization benchmarks.
        *   *Custom Whisper:* Contextual bias module using JSON/TSV definitions and local LLM correction for offline speech recognition.
        *   *Dashboard:* Web-based monitoring stack (port 9190) tracking GPU metrics, systemd services, and automated schedule generation via local 35B models.
        *   *Watchdog:* Advanced systemd watchdog for llama-stack monitoring VRAM/token-per-second with anomaly alerts to Telegram.
        *   *GGUF Pipeline:* Automated benchmarking on Tesla P40/RTX 3050 to determine optimal GGUF quantization (Q4/Q5) for production.
        *   *Bot-short:* C++ Telegram bot generating AI-powered vector graphics (SVG/EPS) pipeline.
        *   *Megatool:* OSINT suite combining C++ engine with Flask web interface and AI photo analysis capabilities.
        *   *Openclaw:* Node.js gateway providing unified access to local Ollama instances.
        *   *Reddit Monitor:* Scrapes AI/tech subreddits to feed AGENDA.md with curated research threads.
        *   *Tesla P40 Controller:* ESP32 firmware with DS18B20 sensors and PWM MOSFET control for dynamic fan curve and thermal throttling prevention.
        *   *Digital Thermal:* HID-based temperature display interfacing with PC sensors.
        *   *Model Selector:* ESP32 rotary encoder and OLED interface allowing physical switching of local AI models via HID/HTTP.

5.  **Final Assembly:**

    *   Header.
    *   Bio (3 lines).
    *   Table.
    *   Section Headers.
    *   Project lists.
    *   Footer stats.

6.  **Length Check Estimate:**
    *   Header: 4 lines.
    *   Bio: 3 lines.
    *   Table: 5-6 lines.
    *   Projects: ~14 projects x 2 lines = 28 lines + headers = ~35 lines.
    *   Stats: 5 lines.
    *   Footer: 3 lines.
    *   Total: ~55 lines + margins.
    *   *Correction:* The prompt asks for 90–120 lines. To meet this, I should ensure the descriptions are rich enough (but still 1 line technically, maybe wrapping logic) or structure the stack table slightly differently, or simply ensure standard markdown formatting creates enough vertical whitespace (or lack thereof that renders as lines).
    *   *Wait*, strictly counting lines of text. If I have ~15 projects, that's 15 lines of links + 15 lines of descriptions = 30 lines. + Headers (4). + Bio (3). + Table (10). + Stats (5). + Spacing (30). Total ~80-90 lines. I need to ensure the "1-line technical description" is sufficiently dense and perhaps layout the list items on separate lines to bulk up the visual structure without adding fluff.

    Let's maximize technical density in the descriptions to make them long single lines (wrapping is natural, but logically one sentence).

    *Self-Correction on bio:*
    Researcher specializing in LLM inference acceleration (speculative decoding, MoE routing) and porting modern models to legacy hardware (CUDA sm_61).
    Architecting self-hosted AI infrastructure, custom CUDA kernels, and embedded control systems for hardware optimization.
    Building automation pipelines for quantization, testing, and deployment of local multimodal models.

    *Self-Correction on slugs:*
    Ensure `https://github.com/chessarisilvio/` prefix is used.

7.  **Final Polish (Mental Simulation of Output):**

    ```markdown
    <div align="center">
      <h1> ⚡ Silvio Chessari </h1>
    </div>

    ### Technical Profile
    Researching LLM inference optimization (EAGLE/MTP, speculative decoding, MoE routing) and bypassing hardware constraints via CUDA sm_61 shims (Tesla P40).
    Architecting self-hosted AI infrastructure, automated quantization pipelines, and embedded systems for thermal management and physical model switching.
   专注于 local-first deployment, reverse-engineering GPU limitations, and building robust automation tools for inference workloads.

    ### Technical Stack
    | **Category** | **Technologies** |
    | :--- | :--- |
    | **AI/ML** | llama.cpp, Ollama, PyTorch, GGUF, EXL2, Speculative Decoding, Whisper, Multimodal Vision |
    | **Systems** | CUDA, CMake, C++, Python, Node.js, Flask, systemd, Bash Scripting, OpenCV, Docker |
    | **Hardware** | Tesla P40 (sm_61), ESP32, Sensors (I2C/1-Wire), HID, PWM Controllers, Soldering |
    ```

    *Actually, the prompt says "centered header -> 3-line technical bio -> compact stack table".*
    *Centering text in markdown is usually HTML `<div align="center">`.*

    Let's refine the projects list to ensure the descriptions hit the "real technical depth" requirement.

    *LLM Research:*
    - [Add video input support to llama.cpp](https://github.com/chessarisilvio/add-video