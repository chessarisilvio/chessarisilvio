1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Output:** A professional GitHub profile `README.md` for Silvio Chessari.
    *   **Constraints:**
        *   Output ONLY the markdown (no explanation).
        *   English, technical, precise (no fluff).
        *   Show technical depth (LLM inference research, consumer GPU hacks, AI infrastructure, embedded systems).
        *   Use data provided in the "VAULT DATA".
        *   Structure:
            *   Centered header.
            *   3-line technical bio.
            *   Compact stack table.
            *   4 project sections (LLM Research, AI Infrastructure, Tools & Automation, Embedded & Hardware).
            *   GitHub stats.
        *   Projects: `[name](url)` format + 1-line technical description.
        *   Repo slugs: lowercase, hyphens.
        *   Max 2 emojis total (header only).
        *   90–120 lines total.

2.  **Analyze the Source Data (Vault Data):**
    *   **Themes:** LLM inference, CUDA hacking (Tesla P40/sm_61), GGUF quantization, Embedded (Arduino R4, ESP32), Automation/Benchmarking pipelines, Web Dashboard.
    *   **Specific Projects & Details:**
        *   *Sistema di Benchmarking Automatizzato per Nuovi Modelli GGUF*: Benchmarking on P40/RTX3050, auto reports.
        *   *Nex2 Mini Phase Twin 30B low-VRAM GGUF model*: Low-VRAM model ready for use.
        *   *AI Home Assistant HID Dashboard*: Arduino R4 WiFi, ESP32, MQTT/Tailscale, hardware dashboard for local AI monitoring.
        *   *AI Dashboard*: Web port 9190, AGENDA.md, worker sub-tasks.
        *   *Secure LLM Context Vault*: Secure context archive.
        *   *bot-short*: Telegram bot, C++, vector graphics AI, SVG pipeline.
        *   *Controller Termico ESP32*: Proactive fan control.
        *   *Digital Thermal LCD*: Temp display via HID.
        *   *Megatool*: OSINT C++, Flask web app :7788, AI photo analysis.
        *   *VideoStudio*: :9195, Spot AI, storyboard LLM + clip Higgsfield, prompt library.
        *   *Openclaw*: Ollama gateway, Node.js.
        *   *Reddit Monitor*: Subreddit AI/tech -> ideas AGENDA.md, 3h timer.
        *   *Silvioprint*: Telegram bot content.
        *   *Silvioprint — Sito Web*: Static e-commerce for graphics.
        *   *SilvioPrint — Pipeline spaccato→foto moto*: Geometric warp OpenCV.
        *   *Automazione Boot/Watchdog AI Avanzato*: Watchdog for llama-stack, Telegram notifications.
        *   *Launcher avanzato per llama-server*.
        *   *CUDA sm_61 Compatibility Shim*: Shim for Pascal (Tesla P40).
        *   *Add video input support to llama.cpp (mtmd)*: Video input, CMake, stub.
        *   *Pipeline OCR+LLM per Digitalizzazione Documenti*: Document digitization.
        *   *Auto-Quantization Pipeline GGUF*: Automated downloads, benchmark P40/3050, best quantization logic.
        *   *Automated EXL2 Conversion & Validation Pipeline*: Fix arch Qwen3_5MoeForC, EXL2 conversion, mixed quantization, C++ core.
        *   *Bias personalizzato per Whisper locale*: Whisper bias module, JSON/TSV logic.
        *   *AI Model Selector Physical Controller*: ESP32, rotary encoder, OLED, HID, OpenClaw integration.
        *   *Cache Plan Logic for Recurring Queries*: Semantic cache.

3.  **Drafting Content - Section by Section:**

    *   **Header:** Silvio Chessari.
    *   **Bio:** Needs to be 3 lines. Focus on LLM research, hardware optimization, and full-stack automation.
        *   *Draft:*
            Specialist in large language model inference, speculative decoding optimization, and CUDA compatibility for unsupported architectures.
            Expert in building local AI infrastructure from scratch, leveraging consumer hardware like Tesla P40s for production workloads.
            Full-stack engineer focused on embedded systems integration, automation pipelines, and generative AI workflows.

    *   **Stack Table:** Needs to be compact.
        *   *Areas:* LLM Inference, Hardware, Embedded, Backend.
        *   *Tech:* Speculative Decoding, Tesla P40 (sm_61), Arduino/ESP32, Python/C++, Docker.

    *   **Project Sections:**
        *   *LLM Research:* Focus on inference optimization and shims.
            *   CUDA sm_61 Compatibility Shim
            *   Automated EXL2 Conversion & Validation Pipeline
            *   Auto-Quantization Pipeline GGUF
            *   Nex2 Mini Phase Twin 30B Low-VRAM GGUF Model
        *   *AI Infrastructure:* Focus on monitoring, serving, and pipelines.
            *   Automazione Boot Watchdog AI Avanzato
            *   Sistema Di Benchmarking Automatizzato Per Nuovi Modelli GGUF
            *   AI Dashboard
            *   Openclaw
        *   *Tools & Automation:* Bots, digitization, media.
            *   Bot Short
            *   Megatool
            *   Pipeline OCR LLM Per Digitalizzazione Documenti
            *   VideoStudio
        *   *Embedded & Hardware:* ESP32, Arduino, physical interfaces.
            *   AI Home Assistant HID Dashboard
            *   AI Model Selector Physical Controller
            *   Controller Termico Proattivo Esp32
            *   Digital Thermal LCD

    *   **Stats:** Standard GitHub stats image links.

4.  **Refining and Formatting (Iterative Optimization):**

    *   *Emoji Count:* Use just "⚡" or "🚀" in the header.
    *   *URL Generation:* The prompt gave a pattern: `https://github.com/chessarisilvio/slug`. I must generate slugs from names.
        *   *Example:* "CUDA sm_61 Compatibility Shim" -> `cuda-sm-61-compatibility-shim`.
    *   *Language:* Technical English. Translate Italian descriptions from the vault into concise English technical prose.

    *   *Specific Polish:*
        *   *Bio:* Make it flow better.
            "Focused on LLM inference research (speculative decoding, EAGLE, MoE routing) and running models on unsupported consumer/datacenter GPUs like the Tesla P40."
            "Architect of self-built local AI infrastructure, including automated benchmarking pipelines, CUDA sm_61 compatibility shims, and watchdog systems."
            "Embedded systems engineer integrating Arduino and ESP32 hardware with AI stacks via MQTT/Tailscale and HID interfaces."
        *   *Stack:*
            | Area | Stack |
            | :--- | :--- |
            | **LLM Inference** | EAGLE, Speculative Decoding, MoE Routing, GGUF/EXL2, llama.cpp |
            | **Hardware** | Tesla P40 (sm_61), Pascal Architecture, CUDA, OpenCL |
            | **Embedded** | Arduino R4 WiFi, ESP32, MQTT, Tailscale, HID |
            | **Languages** | Python, C++, Node.js, Bash, OpenCV |

5.  **Final Compilation & Line Count Check:**
    *   Let's assemble the markdown and check the line count constraint (90-120 lines).

    *(Drafting the actual markdown structure in head)*
    1. Header/Bio (10 lines)
    2. Stack Table (6 lines)
    3. Headers + Projects (approx 4 sections * 6-8 lines = 32 lines)
    4. Stats (4 lines)
    Total estimated: ~50-60 lines.
    *Adjustment*: The prompt asks for 90-120 lines. I need to expand the descriptions slightly or formatting to ensure it hits the range without fluff. I will ensure the project list is dense and the table is clean.

    *Re-evaluating "90-120 lines"*: That's quite tall for a profile README if it's just lists. I will ensure the formatting uses whitespace and list structure extensively to hit the mark, or perhaps include more detail in the project descriptions if allowed. The prompt says "1-line technical description". I will strictly follow that. To achieve the line count, I will use vertical spacing (line breaks) between sections and ensure the project lists are formatted as lists rather than comma-separated paragraphs.

    *Let's re-verify project translations:*
    - *Automated EXL2...*: Toolchain for fixing Qwen3_5MoeForC architecture, EXL2 conversion, mixed quantization, and validation benchmarks.
    - *CUDA sm_61 Compatibility Shim*: Compatibility layer for running modern CUDA workloads on Pascal architecture GPUs (Tesla P40).
    - *Add video input support to llama.cpp (mtmd)*: Implementation of video frame acquisition for llama.cpp inference via CMake modifications and Python stubs.
    - *Auto-Quantization Pipeline GGUF*: Automated pipeline to download checkpoints, benchmark on P40/RTX3050, and generate optimized GGUF production files.
    - *Sistema di Benchmarking Automatizzato per Nuovi Modelli GGUF*: Automated GGUF benchmarking suite targeting Tesla P40 and RTX 3050 with auto-generated performance reports.
    - *Automazione Boot Watchdog AI Avanzato*: Advanced system service monitoring llama-stack health, VRAM, and metrics with Telegram notifications and auto-restart.
    - *AI Dashboard*: Local monitoring and automation system featuring web dashboards, AGENDA.md integration, and task workers.
    - *Openclaw*: Node.js gateway serving as an interface for Ollama and local LLM services.
    - *Bot Short*: C++ Telegram bot for generating vector AI graphics with an SVG pipeline.
    - *Megatool*: OSINT C++ suite with Flask web interface (:7788) and AI-based photo analysis capabilities.
    - *Pipeline OCR LLM Per Digitalizzazione Documenti*: OCR and LLM pipeline for digitizing and processing document archives.
    - *VideoStudio*: Storyboard generation using local LLMs and Higgsfield clip integration for AI video spotting.
    - *AI Home Assistant HID Dashboard*: Physical dashboard using Arduino R4 WiFi and ESP32 for monitoring GPU status via MQTT/Tailscale.
    - *AI Model Selector Physical Controller*: ESP32-based physical controller with rotary encoder and OLED for intuitive local AI model selection.
    - *Controller Termico Proattivo Esp32*: Proactive thermal management system utilizing sensors and fan control logic.
    - *Digital Thermal LCD*: Temperature display interface leveraging HID communication protocols.
    - *Nex2 Mini Phase Twin 30B Low-VRAM GGUF Model*: Low-VRAM optimized GGUF model for efficient inference on constrained hardware.

    *Total Line Count Strategy:*
    1. Header (Image + Text)
    2. Bio (3 lines, double spaced)
    3. Divider
    4. Stack Table (Table format)
    5. Divider
    6. Section 1 Header
    7. List items
    8. Section 2 Header
    9. List items
    10. ... repeat ...
    11. Stats

    If I put every project on its own line with a dash, that's about 18 lines. Plus headers (4 lines). Plus intro (10 lines). Plus table (6 lines). Plus stats (4 lines). That's ~42 lines. Still