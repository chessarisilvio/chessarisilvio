1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Target:** Professional GitHub profile README.md for Silvio Chessari.
    *   **Source Data:** A provided "VAULT DATA" consisting of Obsidian-style notes describing projects (LLM research, AI infrastructure, embedded systems, etc.).
    *   **Requirements:**
        *   Output ONLY the README.md markdown.
        *   English, technical, precise, fluff-free.
        *   Show depth: LLM inference (EAGLE/MTP/speculative decoding/MoE), running LLMs on unsupported GPUs (Tesla P40, sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.
        *   Use details from vault data.
        *   Structure:
            1.  Centered header (Max 2 emojis).
            2.  3-line technical bio.
            3.  Compact stack table.
            4.  4 project sections: LLM Research, AI Infrastructure, Tools & Automation, Embedded & Hardware.
            5.  GitHub stats at the bottom.
        *   Project format: `[name](https://github.com/chessarisilvio/slug) + 1-line tech description`.
        *   Slug generation: Lowercase, hyphens.
        *   Length: 90-120 lines.

2.  **Analyze the Vault Data (Extraction & Categorization):**

    *   *General Info:* Silvio Chessari, Italian speaker (docs are in Italian), works with local AI stacks, P40/RTX3050 setup.
    *   *LLM Research:*
        *   `add-video-input-support-to-llamacpp-mtmd`: llama.cpp video input support.
        *   `automated-exl2-conversion-validation-pipeline`: EXL2 conversion, quantization, Qwen3.5MoE arch fix.
        *   `auto-quantization-pipeline-gguf`: Automated GGUF quantization/benchmarking.
        *   `mtp` (inferred from context of spec decoding or just general LLM knowledge, but data mentions "mtmd").
    *   *AI Infrastructure:*
        *   `openclaw`: Ollama Gateway, Node.js.
        *   `llama-stack` (inferred context in Automazione Boot/Watchdog).
        *   `nllb-self-hosted`: Offline translation pipeline.
    *   *Tools & Automation:*
        *   `ai-dashboard`: Monitoring dashboard, AGENDA.md.
        *   `automazione-bootwatchdog-ai-avanzato`: Watchdog for llama-stack, systemd, Telegram.
        *   `mtop-htop-per-monitoraggio-llm-locale`: htop-like for LLM inference.
        *   `bot-short`: Telegram bot, C++, SVG graphics.
        *   `megatool`: OSINT C++ + Flask.
        *   `reddit-monitor`: Subreddit AI monitoring.
        *   `silvioprint`: Telegram content bot.
        *   `bias-personalizzato-per-whisper-locale`: Whisper bias correction.
    *   *Embedded & Hardware:*
        *   `ai-home-assistant-hid-dashboard`: Arduino R4 WiFi, ESP32, MQTT, P40 status display.
        *   `ai-model-selector-physical-controller`: ESP32, OLED, Rotary encoder.
        *   `controller-termico-proattivo-esp32`: Fan control, sensors.
        *   `digital-thermal-lcd`: HID LCD temperature display.
        *   `cuda-sm61-compatibility-shim`: CUDA sm_61 shim for Tesla P40.

3.  **Drafting Content - Step-by-Step:**

    *   **Header:** Needs to be centered. "Silvio Chessari". 2 emojis max. Let's use 🚀 (tech) or 🧠 (AI).
        *   *Draft:*
            <div align="center">
              <h1>Silvio Chessari 🧠⚡</h1>
            </div>

    *   **Bio (3 lines):**
        *   Focus on LLM inference optimization (P40/RTX3050), speculative decoding, CUDA workarounds.
        *   Focus on embedded integration.
        *   Focus on building self-hosted infra.
        *   *Draft:*
            Optimizing LLM inference on consumer and legacy hardware via speculative decoding, MoE routing, and CUDA compatibility shims.
            Building self-hosted AI infrastructure integrating CUDA workarounds (Tesla P40 sm_61), automated benchmarks, and embedded control systems.
            Researching efficient token generation through EAGLE/MTP architectures and custom quantization pipelines (GGUF/EXL2).

    *   **Stack Table:**
        *   Langs: C++, Python, CMake.
        *   Infra: CUDA, Docker, Node.js.
        *   Hardware: ESP32, Arduino, Tesla P40.
        *   AI: llama.cpp, Ollama, GGUF, EXL2.

    *   **Project Sections (Select best items for 90-120 lines):**

        *   *LLM Research:*
            *   `add-video-input-support-to-llamacpp-mtmd`: Video input for vision models.
            *   `automated-exl2-conversion-validation-pipeline`: EXL2 quantization/Qwen MoE.
            *   `auto-quantization-pipeline-gguf`: Automated benchmarking/Quantization.
            *   `cuda-sm61-compatibility-shim`: (Maybe here or Infra? Better Research/Infra). Let's put Shim here or a subsection of infra. The prompt asks for 4 sections. Research fits best for low-level CUDA hacks.

        *   *AI Infrastructure:*
            *   `openclaw`: Ollama Gateway.
            *   `nllb-self-hosted`: Translation pipeline.
            *   `mtop-htop-per-monitoraggio-llm-locale`: Monitoring.
            *   `automazione-bootwatchdog-ai-avanzato`: Watchdog.

        *   *Tools & Automation:*
            *   `ai-dashboard`: Web dashboard.
            *   `bot-short`: Telegram SVG bot.
            *   `megatool`: OSINT/Flask.
            *   `reddit-monitor`: Subreddit scraper.
            *   `bias-personalizzato-per-whisper-locale`: Whisper bias.

        *   *Embedded & Hardware:*
            *   `ai-home-assistant-hid-dashboard`: Arduino R4 + MQTT.
            *   `ai-model-selector-physical-controller`: ESP32 Encoder.
            *   `controller-termico-proattivo-esp32`: Fan control.
            *   `digital-thermal-lcd`: Temp display.

    *   **Refining Project Descriptions (Technical & Precise):**
        *   *Shim:* Shim layer enabling LLM inference on Pascal GPUs (sm_61) by bypassing architectural checks in modern runtimes.
        *   *EXL2:* Pipeline for arch-fixing Qwen3.5MoE, converting to EXL2, mixed quantization, and automated validation.
        *   *llama.cpp:* CMake integration for video input, webcam frame capture via OpenCV, and inference server stubs.
        *   *mtop:* Real-time htop-like monitor displaying VRAM usage, token throughput, and GPU temperature for local inference.
        *   *Dashboard:* Web UI (:9190) visualizing GPU metrics, service status, and AGENDA.md driven sprint automation.

    *   **Slugs:**
        *   `add-video-input-support-to-llamacpp-mtmd` -> `add-video-input-support-to-llamacpp-mtmd`
        *   `automated-exl2-conversion-validation-pipeline` -> `automated-exl2-conversion-validation-pipeline`
        *   `cuda-sm61-compatibility-shim` -> `cuda-sm61-compatibility-shim`
        *   `openclaw` -> `openclaw`
        *   `nllb-self-hosted` -> `nllb-self-hosted`
        *   `mtop` -> `mtop-htop-per-monitoraggio-llm-locale`
        *   `ai-dashboard` -> `ai-dashboard`
        *   `bot-short` -> `bot-short`
        *   `megatool` -> `megatool`
        *   `ai-home-assistant` -> `ai-home-assistant-hid-dashboard`
        *   `ai-model-selector` -> `ai-model-selector-physical-controller`
        *   `esp32-fan-control` -> `controller-termico-proattivo-esp32`

    *   **GitHub Stats:** Standard stats block at the end.

4.  **Review against Constraints:**
    *   English? Yes.
    *   No preamble? Yes.
    *   Technical depth? Yes (mentioning sm_61, MoE, EXL2, etc.).
    *   Structure? Header -> Bio -> Stack -> 4 Sections -> Stats.
    *   Line count? Need to ensure spacing is tight but readable to hit 90-120 lines.
    *   Emojis? Only in header.

5.  **Final Polish of Text:**
    *   *Bio Optimization:* "Specialized in LLM inference on unsupported hardware (Tesla P40 sm_61) via CUDA shims and speculative decoding (EAGLE/MTP). Developing self-hosted AI stacks with MoE routing, automated EXL2/GGUF quantization pipelines, and integration with embedded control systems."
    *   *Project ordering logic:* Put the most impressive (Shim, EXL2, llama.cpp video) first.

6.  **Constructing the Markdown (Mental or Scratchpad):**
    (Self-Correction during drafting: Ensure the URL format is strictly `https://github.com/chessarisilvio/[slug]`).

    *   *Section 1: LLM Research*
        *   `cuda-sm61-compatibility-shim`
        *   `automated-exl2-conversion-validation-pipeline`
        *   `add-video-input-support-to-llamacpp-mtmd`
        *   `auto-quantization-pipeline-gguf`

    *   *Section 2: AI Infrastructure*
        *   `openclaw`
        *   `mtop-htop-per-monitoraggio-llm-locale`
        *   `automazione-bootwatchdog-ai-avanzato`
        *   `nllb-self-hosted-per-testo-multilingua`

    *   *Section 3: Tools & Automation*
        *   `ai-dashboard`
        *   `bot-short`
        *   `megatool`
        *   `reddit-monitor`
        *   `bias-personalizzato-per-whisper-locale`

    *   *Section 4: Embedded & Hardware*
        *   `ai-home-assistant-hid-dashboard`
        *   `ai-model-selector-physical-controller`
        *   `controller-termico-proattivo-esp32`
        *   `digital-thermal-lcd`

7.  **Final Line Count Check:**
    Header: 3 lines.
    Bio: 3 lines.
    Stack: 3-4 lines.
    Sections: ~15-16 items * 2 lines (header + item) = ~32 lines + headers ~4 lines.
    Stats: 2-3 lines.
    Spacing: ~10-15 lines.
    Total approx: 60-80 lines. I need to expand slightly on descriptions or formatting to hit 90-120 without fluff.
    *Adjustment:* Use separate lines for the description under the link to break it up? No, requirements say `[