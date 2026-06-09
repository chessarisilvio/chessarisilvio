1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Subject:** Silvio Chessari.
    *   **Task:** Generate a professional GitHub Profile `README.md`.
    *   **Source Material:** Technical vault data (Obsidian/Markdown format).
    *   **Constraints:**
        *   Output ONLY the markdown (no preamble, no explanation).
        *   Language: English, technical, precise (no fluff).
        *   Show technical depth: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), running LLMs on unsupported GPUs (Tesla P40 sm_61, CUDA workarounds), AI infrastructure, embedded systems.
        *   Structure:
            1.  Centered header.
            2.  3-line technical bio.
            3.  Compact stack table.
            4.  4 project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware).
            5.  GitHub stats.
        *   Project Link Format: `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
        *   Slug derivation: lowercase, hyphens.
        *   Emojis: Max 2 (header only).
        *   Line count: 90–120 lines.

2.  **Analyze the Source Data (Vault Content):**
    *   *Overview:* Distinguishes between "Developed" (personal code), "LLM Stack" (infrastructure config), "Installed Services", and "Ideas".
    *   *Developed Projects:*
        *   `ai-dashboard`: Python, monitoring, worker tasks.
        *   `bot-short`: C++ Telegram bot, SVG graphics.
        *   `controller-termico-proattivo-esp32`: ESP32, Fan control for Tesla P40, DS18B20 sensors.
        *   `digital-thermal-lcd`: Python, HID, Thermalright LCD temp display.
        *   `openclaw`: Node.js, Ollama gateway, TG bot.
        *   `silvioprint`: Python, TG bot, systemd service.
        *   `launcher-avanzato-per-llama-server`: Launcher for llama-server.
        *   `cuda-sm61-compatibility-shim`: Compatability shim for Pascal (P40), CUDA sm_61.
        *   `add-video-input-support-to-llamacpp-mtmd`: Video input for llama.cpp (CMake, OpenCV).
    *   *LLM Stack Projects:*
        *   `dashboard-telemetrica-ai-hardware`: Node.js, GPU/VRAM monitoring, TG alerts.
        *   `freellmapi`: Proxy for free cloud tiers (Groq, etc.), OpenAI compatible.
        *   `gateway-telegram-multimodale-offline`: Multimodal TG bot.
        *   `gguf-model-manager-cli`: CLI for GGUF models.
        *   `llm-observability`: FastAPI, Prometheus metrics.
        *   `markitdown`: Document ingestion for RAG.
        *   `proxy-anthropicopenai-con-safety-hooks`: Proxy with safety hooks.
        *   `start-llama`: Launcher with YAML presets.
        *   `whisperapi-self-hosted`: Self-hosted STT.
        *   `llama-cpp-benchmark-suite`: Benchmarking consumer GPUs.
        *   `update-github-profile`: Auto-updater script.
    *   *Installed Services (Third-party):* Aider, ComfyUI, Nextcloud, Odysseus. (Likely exclude from personal project list, but the skills imply familiarity).

3.  **Drafting - Section by Section:**

    *   **Header:** Centered text. Name: Silvio Chessari. Emojis allowed (max 2).
        *   *Draft:* `# Silvio Chessari ⚡️ 🛠️`

    *   **Bio:** 3 lines, technical depth.
        *   *Key topics:* LLM inference research (speculative decoding), unsupported GPU hardware optimization (Tesla P40 sm_61), embedded systems.
        *   *Draft:*
            Specializing in LLM inference optimization, speculative decoding, and running large models on unsupported/legacy hardware.
            Building self-hosted AI infrastructure from the ground up, integrating custom CUDA sm_61 compatibility shims for Tesla P40s.
            Developing embedded solutions for thermal management and automation using ESP32 and sensor networks.

    *   **Stack Table:**
        *   *Languages/Tools:* Python, C++, Node.js, CUDA, CMake.
        *   *AI/ML:* llama.cpp, Ollama, Whisper, RAG, FastAPI.
        *   *Hardware:* ESP32, Tesla P40, Sensors, Linux Systemd.
        *   *Draft Table:* (Standard compact format).

    *   **Project Sections & Categorization:**

        *   *Category 1: LLM Research (Speculative decoding, custom compilation, video input)*
            1.  `cuda-sm61-compatibility-shim`: Enabling modern LLM stacks on legacy Pascal GPUs via custom CUDA shims.
            2.  `add-video-input-support-to-llamacpp-mtmd`: Extending llama.cpp with video input pipelines for multimodal inference.
            3.  (Maybe the benchmark suite fits here? No, fits better in infra). What about the "launcher"? Probably Infra.

        *   *Category 2: AI Infrastructure (Orchestration, Monitoring, APIs)*
            1.  `freellmapi`: OpenAI-compatible proxy aggregating free-tier cloud providers for distributed inference.
            2.  `dashboard-telemetrica-ai-hardware`: Node.js telemetry dashboard monitoring GPU VRAM, temperature, and system health.
            3.  `llm-observability`: FastAPI service providing Prometheus metrics and visualization for llama-server instances.
            4.  `gateway-telegram-multimodale-offline`: Offline multimodal gateway integrating local LLMs with Telegram interfaces.

        *   *Category 3: Tools & Automation (Bots, Managers, Scripts)*
            1.  `ai-dashboard`: Python-based local monitoring and automation system with agenda integration and task workers.
            2.  `openclaw`: Multi-channel AI gateway supporting session memory and tool use over Node.js.
            3.  `gguf-model-manager-cli`: Command-line utility for managing and organizing GGUF model repositories.
            4.  `silvioprint`: Telegram bot service for content management and automated printing routines.

        *   *Category 4: Embedded & Hardware (ESP32, LCD, Sensors)*
            1.  `controller-termico-proattivo-esp32`: ESP32 firmware for proactive fan control of Tesla P40 using DS18B20 sensors.
            2.  `digital-thermal-lcd`: HID interface for real-time temperature display on Thermalright LCD hardware.
            3.  `bot-short`: C++ Telegram bot generating vector graphics (SVG/EPS) via AI pipelines.

    *   **Refining Project Links:** Format `[name](https://github.com/chessarisilvio/slug)`.
        *   Need to generate slugs based on titles.
        *   Example: `cuda-sm61-compatibility-shim` -> `cuda-sm61-compatibility-shim`.
        *   Example: `add-video-input-support-to-llamacpp-mtmd` -> `add-video-input-support-to-llamacpp-mtmd`.

    *   **GitHub Stats:** Standard image placeholders (usually provided by user in prompts, but I will use the generic popular ones like `github-readme-stats` URLs as is standard for technical templates).

4.  **Review and Formatting:**
    *   *Check constraints:* English? Yes. Technical? Yes. No fluff? Yes.
    *   *Structure:* Header -> Bio -> Stack -> Projects -> Stats.
    *   *Line count check:* Let's write it out to estimate.

    *(Self-Correction during drafting)*:
    *   The prompt asks to "Show real technical depth" regarding EAGLE/MTP/speculative decoding/MoE. While the Vault data mentions specific experiments in "ricerca" (implied by the tree structure), the specific project details for EAGLE/MTP aren't fully fleshed out in the *project list* provided, only generic "LLM research". However, the prompt explicitly asks to include depth on these. I will ensure the bio reflects this focus, and perhaps add a note or select the most "research-heavy" project (the CUDA shim or the video input) to anchor the research section, as they relate to model architecture and compilation. *Wait, the prompt says "Output ONLY the final README ... Use real technical details from the vault data". I should not hallucinate projects not in the vault. I will focus the technical depth in the bio and project descriptions based on what *is* there (e.g. llama.cpp modifications, CUDA workarounds), as these demonstrate that depth.*

5.  **Final Code Construction (Mental Draft):**

    *   **Bio:**
        I specialize in pushing the boundaries of local LLM inference on unsupported hardware, specifically optimizing for legacy sm_61 GPUs like the Tesla P40 using custom CUDA workarounds. My work involves speculative decoding research, multimodal input extensions (video), and building resilient self-hosted AI infrastructure. I bridge high-level AI orchestration with low-level embedded controls, implementing thermal management via ESP32 and real-time hardware telemetry.

    *   **Stack:**
        `C++` `Python` `CUDA` `CMake` `Node.js` `llama.cpp` `Ollama` `FastAPI` `Prometheus` `ESP32` `Systemd` `Bash`

    *   **Projects Mapping:**

        *   **LLM Research:**
            *   `cuda-sm61-compatibility-shim` -> Shim enabling modern LLMs on Tesla P40.
            *   `add-video-input-support-to-llamacpp-mtmd` -> Video input for llama.cpp.

        *   **AI Infrastructure:**
            *   `freellmapi` -> Free tier cloud aggregator.
            *   `dashboard-telemetrica-ai-hardware` -> Node.js GPU monitoring.
            *   `llm-observability` -> Prometheus metrics.

        *   **Tools & Automation:**
            *   `ai-dashboard` -> Python dashboard and worker system.
            *   `openclaw` -> Node.js AI gateway.
            *   `gguf-model-manager-cli` -> GGUF management.
            *   `proxy-anthropicopenai-con-safety-hooks` -> Safety proxy.

        *   **Embedded & Hardware:**
            *   `controller-termico-proattivo-esp32` -> P40 fan control.
            *   `digital-thermal-lcd` -> HID temp display.
            *   `bot-short` -> C++ SVG bot.

6.  **Line Count Optimization:**
    The prompt asks for 90-120 lines. I need to make sure the formatting (spacing) fits this. I will use standard markdown spacing (one blank line between sections). Table is compact. Projects are concise.

    *Let's write the content.*

    (Drafting the markdown contents - see final output).
    *Double check emojis:* Header only. `⚡️ 🛠️`.
    *Double check URLs:* `https://github.com/chessarisilvio/[slug]`.

    *Slug Normalization:*
    - `add-video-input-support-to-llamacpp-mtmd`
    - `ai-dashboard`
    - `bot-short`
    - `controller-termico-proattivo-esp32`