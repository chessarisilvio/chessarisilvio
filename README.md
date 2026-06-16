1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Subject:** Silvio Chessari.
    *   **Output:** Professional GitHub profile `README.md`.
    *   **Constraints:**
        *   Output ONLY the markdown.
        *   No preamble, no explanation.
        *   Tone: English, technical, precise, no fluff.
        *   Content Depth: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), running LLMs on unsupported consumer/datacenter GPUs (Tesla P40 sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.
        *   Use real technical details from the provided "vault data".
        *   Structure:
            1.  Centered header.
            2.  3-line technical bio.
            3.  Compact stack table.
            4.  4 Project Sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware).
            5.  GitHub stats.
        *   Project format: `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
        *   Slugs: Lowercase, hyphens.
        *   Max 2 emojis (header only).
        *   Length: 90–120 lines.

2.  **Analyze the Vault Data:**
    *   *Key Technologies/Themes:* CUDA sm_61, Tesla P40, RTX 3050, GGUF, EXL2, llama.cpp, video input, benchmarking, quantization, ESP32, Arduino R4, MQTT, Tailscale, Telegram bots, OSINT, C++, Python, Flasks, systemd.
    *   *Projects:*
        *   `Sistema di Benchmarking Automatizzato per Nuovi Modelli GGUF` -> GGUF benchmarking on P40/3050.
        *   `AI Home Assistant HID Dashboard` -> Arduino R4, ESP32, MQTT, Tailscale, local AI monitoring.
        *   `AI Dashboard` -> Web dash (Port 9190), AGENDA.md integration.
        *   `bot-short` -> Telegram bot, C++, SVG/AI graphics.
        *   `Controller Termico ESP32` -> Fan control.
        *   `Megatool` -> OSINT C++, Flask, AI photo analysis.
        *   `VideoStudio` -> Storyboard LLM, Higgsfield clips, Spot AI.
        *   `Openclaw` -> Ollama Gateway, Node.js.
        *   `Reddit Monitor` -> Subreddit scraping -> AI ideas.
        *   `Automazione Boot/Watchdog AI` -> Watchdog for llama-stack, Telegram alerts, systemd.
        *   `CUDA sm_61 Compatibility Shim` -> Pascal (P40) compatibility.
        *   `Add video input support to llama.cpp` -> CMake, OpenCV.
        *   `AI Model Selector Physical Controller` -> ESP32, rotary encoder, OLED, HID.
        *   `Automated EXL2 Conversion & Validation Pipeline` -> Qwen3_5MoeForC fix, mixed quantization, C++/Python CLI.
        *   `Auto-Quantization Pipeline GGUF` -> Automated quantization/testing.
        *   `Bias personalizzato per Whisper` -> Context correction.

3.  **Drafting - Section by Section:**

    *   **Header:** Standard `# Hi, I'm Silvio Chessari`. Add emojis here (e.g., ⚡️ 🤖).

    *   **Bio (3 lines):** Needs to cover LLM inference, GPU hacking (P40/sm_61), and embedded systems.
        *   *Draft:* Specialized in optimizing LLM inference on legacy and consumer hardware, focusing on speculative decoding and CUDA sm_61 compatibility shims for Tesla P40 GPUs. I build self-hosted AI infrastructure, integrating high-performance compute with Python/C++ automation. My work bridges the gap between theoretical research (MoE routing, EAGLE) and physical implementation via embedded systems (ESP32, Arduino R4).

    *   **Stack Table:** Needs columns for Tech/Tool. I'll categorize based on the data.
        *   *Draft:*
            | LLM & Inference | CUDA (sm_61), GGUF, EXL2, llama.cpp, Speculative Decoding |
            | Dev & Ops | Python, C++, Bash, systemd, Docker, Tailscale, MQTT |
            | Embedded | ESP32, Arduino R4 WiFi, OpenCV, HID |

    *   **Project Sections:**
        *   *Constraint:* 4 specific sections.
        *   *Mapping:*
            1.  **LLM Research & Optimization:** `cuda-sm-61-compatibility-shim`, `add-video-input-support-to-llama.cpp`, `automated-exl2-conversion-validation-pipeline`, `bias-personalizzato-per-whisper-locale`.
            2.  **AI Infrastructure:** `sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf`, `auto-quantization-pipeline-gguf`, `automazione-bootwatchdog-ai-avanzato`, `openclaw`.
            3.  **Tools & Automation:** `ai-dashboard`, `reddit-monitor`, `megatool`, `bot-short`.
            4.  **Embedded & Hardware:** `ai-home-assistant-hid-dashboard`, `controller-termico-proattivo-esp32`, `ai-model-selector-physical-controller`.

    *   **Refining Project Descriptions (Technical & Concise):**
        *   *shim:* `CUDA sm_61 Compatibility Shim` -> Layer bypassing architectural checks to enable modern LLM kernels on Tesla P40 GPUs.
        *   *video:* `Add video input support to llama.cpp` -> Patched CMake/C++ integration for OpenCV-based frames streaming directly into inference context.
        *   *exl2:* `Automated EXL2 Conversion & Validation Pipeline` -> Toolchain fixing Qwen3_5MoeForC architecture and validating mixed-precision quantization benchmarks.
        *   *benchmark:* `Sistema di Benchmarking Automatizzato per Nuovi Modelli GGUF` -> Automated pipelines testing P40 and RTX 3050 inference speeds across quantization levels.
        *   *watchdog:* `Automazione Boot/Watchdog AI` -> Systemd-integrated bash monitor tracking VRAM and tok/s, triggering Telegram alerts and recovery.
        *   *megatool:* `Megatool` -> C++ OSINT engine with Flask backend and AI photo analysis modules.
        *   *dashboard:* `ai-dashboard` -> Local web interface aggregating GPU telemetry and LLM sprint management.
        *   *home-assistant:* `AI Home Assistant HID Dashboard` -> embedded stack (Arduino R4/ESP32) exposing physical controls over MQTT/Tailscale.

    *   **GitHub Stats:** Standard image placeholders.

4.  **Refining and Formatting:**
    *   Check line count. Aim for ~100 lines.
    *   Check emojis (Header only).
    *   Check slugs (lowercase hyphens).
    *   Verify the "Technical depth" requirement. I need to ensure terms like "sm_61", "GGUF", "EXL2", "speculative decoding", and "MoE" appear naturally.

5.  **Final Polish (Self-Correction during drafting):**
    *   *Correction:* The user specifically mentioned "EAGLE/MTP/speculative decoding". The vault data didn't explicitly mention EAGLE/MTP code, but the prompt asked to *include* technical depth on those topics. I should weave them into the bio or project descriptions where appropriate (e.g., the benchmarking or shim projects imply this context). The prompt says "Show real technical depth... based on his technical vault data", but also "Use real technical details from the vault data below". I will stick primarily to the data in the vault for the projects, but use the prompt's keywords in the bio/intro to set the persona, as requested.
    *   *Correction:* Project names need to be slugs. `cuda-sm-61-compatibility-shim`, `add-video-input-support-to-llama.cpp-mtmd`, etc. I will keep them reasonably short but accurate.
    *   *Formatting:* Use `<div align="center">` for the profile image and header.

6.  **Constructing the Markdown:**

    *   *Bio Line 1:* Focused on LLM research/inference and specific hardware challenges (P40/sm_61).
    *   *Bio Line 2:* Infrastructure and automation (pipeline, benchmarking).
    *   *Bio Line 3:* Embedded systems integration (Arduino/ESP32).

    *   *Projects:*
        *   *LLM Research:*
            *   [CUDA sm_61 Compatibility Shim](https://github.com/chessarisilvio/cuda-sm-61-compatibility-shim) - Compatibility layer enabling modern CUDA kernels on Pascal (Tesla P40) architecture for local LLM inference.
            *   [Automated EXL2 Conversion & Validation Pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) - C++/Python toolchain for fixing Qwen3_5MoeForC architecture and validating mixed-precision quantizations.
            *   [Add video input support to llama.cpp](https://github.com/chessarisilvio/add-video-input-support-to-llama.cpp-mtmd) - Patched CMake/C++ build injecting OpenCV frame capture directly into inference graphs.
            *   [Bias personalizzato per Whisper locale](https://github.com/chessarisilvio/bias-personalizzato-per-whisper-locale) - Custom bias module and LLM-based contextual correction layer for offline Whisper transcription.
        *   *Infrastructure:*
            *   [Sistema di Benchmarking Automatizzato per Nuovi Modelli GGUF](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-modelli-gguf) - Automated workload evaluation comparing GGUF quantizations on Tesla P40 and RTX 3050 architectures.
            *   [Auto-Quantization Pipeline GGUF](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) - Bash-based automation for downloading checkpoints, generating production GGUFs, and updating documentation.
            *   [Automazione Boot/Watchdog AI Avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) - Systemd-aware watchdog monitoring VRAM/tok/s rates with Telegram-based anomaly alerts and recovery.
            *   [Openclaw](https://github.com/chessarisilvio/openclaw) - Node.js gateway bridging local LLM services over Tailscale for distributed compute access.
        *   *Tools:*
            *   [Megatool](https://github.com/chessarisilvio/megatool) - C++ OSINT framework with Flask web interface and AI-powered photographic analysis modules.
            *   [AI Dashboard](https://github.com/chessarisilvio/ai-dashboard) - Local telemetry dashboard visualizing system metrics and managing AGENDA.md-driven sprints.
            *   [Reddit Monitor](https://github.com/chessarisilvio/reddit-monitor) - Python monitor scraping tech subreddits to feed project ideas into the local AGENDA pipeline.
            *   [bot-short](https://github.com/chessarisilvio/bot-short) - C++ Telegram bot generating AI vector graphics and dispatching SVG/EPS files.
        *   *Hardware:*
            *   [AI Home Assistant HID Dashboard](https://github.com/chessarisilvio/ai-home-ass