1.  **Analyze the Request:**
    *   **Role:** Technical writer.
    *   **Output:** A professional GitHub profile `README.md`.
    *   **Subject:** Silvio Chessari.
    *   **Source Material:** A "technical vault" containing project data, goals, and architectures.
    *   **Constraint Checklist & Confidence Score:**
        1.  Output ONLY the final README.md? Yes.
        2.  No preamble, no explanation? Yes.
        3.  English, technical, precise, no fluff? Yes.
        4.  Show real technical depth (Inference, CUDA/GPU hacks, Infra, Embedded)? Yes.
        5.  Use real technical details from data? Yes.
        6.  Structure (Header -> Bio -> Stack -> 4 Projects sections -> Stats)? Yes.
        7.  Project format `[name](link)` + 1-liner? Yes.
        8.  Repo slugs derived from names? Yes.
        9.  Max 2 emojis (header only)? Yes.
        10. 90-120 lines total? Yes.
    *   **Confidence Score:** 5/5.

2.  **Process the Vault Data (Extraction & Synthesis):**

    *   *Bio & Focus:*
        *   LLM Inference research: EAGLE/MTP/speculative decoding/MoE routing (derived from "mtmd" and "EXL2" and general research notes, though specific mentions of EAGLE/MTP are in the *prompt instructions*, I need to integrate them with the vault's theme of inference optimization). The vault mentions "llama.cpp", "EXL2", "Qwen3_5Moe".
        *   Hardware Hacks: Tesla P40 (sm_61), CUDA compatibility shims, fan control.
        *   Stack: C++, Python, ESP32, Node.js (Ollama Gateway), systemd, Hid.

    *   *Project Selection & Categorization:*
        *   **Category 1: LLM Research & Optimization**
            *   *add-video-input-support-to-llamacpp-mtmd*: Adding video input to llama.cpp.
            *   *automated-exl2-conversion-validation-pipeline*: EXL2 quantization for Qwen3_5Moe.
            *   *auto-quantization-pipeline-gguf*: Automated quantization pipeline.
            *   *bias-personalizzato-per-whisper-locale*: Whisper bias correction.
        *   **Category 2: AI Infrastructure**
            *   *ai-dashboard*: Local monitoring, agenda generation.
            *   *automazione-bootwatchdog-ai-avanzato*: Systemd watchdog, VRAM/token monitoring.
            *   *git-mcp-server-per-agenti-ai*: MCP server for AI agents.
            *   *mtop-htop-per-monitoraggio-llm-locale*: Top-like tool for LLM metrics.
        *   **Category 3: Tools & Automation**
            *   *bot-short*: C++ Telegram bot, SVG generation.
            *   *reddit-monitor*: Subreddit monitoring.
            *   *silvioprint*: Content bot.
            *   *nllb-self-hosted-per-testo-multilingua*: Offline translation.
        *   **Category 4: Embedded & Hardware**
            *   *controller-termico-proattivo-esp32*: Tesla P40 fan control, DS18B20 sensors.
            *   *ai-model-selector-physical-controller*: ESP32, rotary encoder, OLED.
            *   *digital-thermal-lcd*: LCD temp display via HID.
            *   *cuda-sm61-compatibility-shim*: Pascal GPU compatibility.

3.  **Drafting the Content (Iterative refinement for tone and constraints):**

    *   *Header:*
        ```markdown
        <div align="center">
          <h1>Silvio Chessari</h1>
          <p>LLM Inference Research & Local AI Infrastructure</p>
        </div>
        ```

    *   *Bio:* Needs to be 3 lines.
        *   Focused on speculative decoding, MoE routing, and hardware optimization.
        *   Specifics: sm_61 (Pascal), Tesla P40, consumer GPUs.
        *   Keywords: CUDA, C++, Python, Embedded.

    *   *Stack Table:*
        *   Languages: C++, Python, CMake.
        *   Infra: Docker/Containerization (implied by "Hub"), Systemd, Node.js.
        *   AI/ML: llama.cpp, EXL2, GGUF, Ollama, ComfyUI.
        *   Hardware: ESP32, Tesla P40, NVIDIA CUDA.

    *   *Project Sections (generating slugs and descriptions):*

        *   *LLM Research:*
            1.  `add-video-input-support-to-llamacpp-mtmd` -> `add-video-input-support-to-llamacpp-mtmd`. Desc: Extended llama.cpp with video input capabilities using CMake modifications, OpenCV stubs, and Python inference scripts.
            2.  `automated-exl2-conversion-validation-pipeline` -> `automated-exl2-conversion-validation-pipeline`. Desc: C++ and Python toolchain for fixing Qwen3_5Moe architectures, mixed-precision EXL2 quantization, and benchmarking.
            3.  `bias-personalizzato-per-whisper-locale` -> `bias-personalizzato-per-whisper-locale`. Desc: Custom bias module for Whisper using JSON/TSV definitions plus LLM-based contextual correction.

        *   *AI Infrastructure:*
            1.  `ai-dashboard` -> `ai-dashboard`. Desc: Local monitoring stack via Flask (:9190) tracking GPU metrics, systemd services, and auto-generating daily agendas using local 35B models.
            2.  `automazione-bootwatchdog-ai-avanzato` -> `automazione-bootwatchdog-ai-avanzato`. Desc: Advanced systemd watchdog monitoring VRAM and token-throughput with automated Telegram alerts and process recovery.
            3.  `mtop-htop-per-monitoraggio-llm-locale` -> `mtop-htop-per-monitoraggio-llm-locale`. Desc: htop-like terminal utility for real-time monitoring of local LLM inference metrics, GPU load, and token generation speed.
            4.  `git-mcp-server-per-agenti-ai` -> `git-mcp-server-per-agenti-ai`. Desc: MCP server exposing Git operations via JSON API to enable autonomous version control for local AI agents.

        *   *Tools:*
            1.  `bot-short` -> `bot-short`. Desc: High-performance C++ Telegram bot generating AI vector graphics in SVG/EPS format.
            2.  `nllb-self-hosted-per-testo-multilingua` -> `nllb-self-hosted-per-testo-multilingua`. Desc: Local offline translation pipeline integrating NLLB-200 with OCR for multilingual text processing.

        *   *Embedded:*
            1.  `controller-termico-proattivo-esp32` -> `controller-termico-proattivo-esp32`. Desc: ESP32 fan controller for Tesla P40 utilizing DS18B20 sensors and PWM MOSFET drivers to prevent thermal throttling.
            2.  `ai-model-selector-physical-controller` -> `ai-model-selector-physical-controller`. Desc: Physical interface with rotary encoder and OLED for selecting local AI models via HID keyboard emulation.
            3.  `cuda-sm61-compatibility-shim` -> `cuda-sm61-compatibility-shim`. Desc: Compatibility layer enabling modern LLM inference stacks on legacy Pascal (sm_61) GPUs like the Tesla P40.

    *   *Stats:* Standard GitHub stats image or code.

4.  **Review against Constraints:**
    *   *Length Check:* 90-120 lines.
    *   *Emojis:* Only in header (or none in header, but "Max 2 emojis total (header only)". I will put them there).
    *   *Fluff:* Stripped out. "Desc: Extended llama.cpp..." is clean.
    *   *Links:* `https://github.com/chessarisilvio/slug`.

5.  **Final Polish (Self-Correction during drafting):**
    *   Ensure the slugs are standard (lowercase, hyphens).
    *   The prompt mentions "Show real technical depth: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing)". I should weave these into the bio or project descriptions even if the vault doesn't explicitly title the project "EAGLE", because the context is high-level inference optimization. I'll add this to the bio to meet the specific requirement "Show real technical depth".
    *   Bio Line 1: Focus on high-level inference research (EAGLE/MTP/speculative decoding).
    *   Bio Line 2: Focus on the hardware hacking (P40/sm_61).
    *   Bio Line 3: Focus on the infrastructure/automation.

6.  **Constructing the Markdown:** (Drafting the actual file content).

    *   *Header:* Silvio Chessari, Researcher & Engineer.
    *   *Bio:* Researching LLM inference acceleration via speculative decoding (EAGLE/MTP), MoE routing, and custom quantization. Specialist in running modern AI stacks on legacy data-center hardware (Tesla P40/sm_61) through CUDA workarounds and custom firmware. Architect of self-hosted, event-driven AI infrastructure integrating embedded systems, daemon orchestration, and real-time telemetry.
    *   *Table:* Columns: Domain, Tech.
    *   *Projects:* Grouped as requested.

7.  **Final Word Count/Line Count Estimate:**
    *   Header: ~5 lines.
    *   Bio: ~4 lines.
    *   Table: ~5 lines.
    *   Dividers: ~5 lines.
    *   Projects (approx 10 items): ~20 lines.
    *   Stats: ~3 lines.
    *   Whitespace/Formatting: ~40 lines.
    *   Total ~80-90 lines. I will adjust spacing and ensure the table is compact to hit the 90-120 range. I'll add a slightly more detailed "Tech Stack" section or ensure the descriptions are rich. actually, the requirement says "compact stack table". I will stick to compact. The project descriptions might be slightly beefier to fill space if needed, but the limit is strict. Let's ensure the bio is formatted as exactly 3 lines.

    *   Let's count lines carefully.
    *   Intro: 5 lines.
    *   Bio: 3 lines.
    *   Table: ~6 lines.
    *   Section Headers: 4 lines.
    *   Project Items: ~12 items * 2 lines = 24 lines.
    *   Stats: 4 lines.
    *   Total non-whitespace: ~46 lines.
    *   Spacing between sections: ~4 lines.
    *   I will expand the descriptions slightly to ensure technical depth and length compliance without fluff. e.g. "Exposing Git operations via JSON API to enable autonomous version control for Claude Code and local agents."

8.  **Output Generation:** (Proceed to generate). No preamble.

    *   *Slug check:* `auto-quantization-pipeline-gguf`, `add-video-input-support-to-llamacpp-mtmd`, `automated-exl2-conversion-validation-pipeline`... looks correct based on the "slug derived from project names" rule.

    *   *Bio Refinement:*
        Researching LLM inference acceleration via speculative decoding (EAGLE/M