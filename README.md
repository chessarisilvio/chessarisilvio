1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Target:** GitHub Profile README for Silvio Chessari.
    *   **Source Material:** Technical vault data (Obsidian-style Markdown).
    *   **Output Format:** ONLY the final README.md markdown. No preamble, no explanation.
    *   **Tone/Style:** English, technical, precise, no fluff. Show real technical depth.
    *   **Key Focus Areas:** LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), unsupported GPU hacking (Tesla P40 sm_61, CUDA), self-built AI infrastructure, embedded systems.
    *   **Structure Requirements:**
        1.  Centered header.
        2.  3-line technical bio.
        3.  Compact stack table.
        4.  4 Project sections (LLM Research, AI Infrastructure, Tools & Automation, Embedded & Hardware).
        5.  GitHub stats.
    *   **Link Format:** `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
    *   **Naming Convention:** Repo slugs derived from project names (lowercase, hyphens).
    *   **Constraints:** Max 2 emojis total (header only). 90-120 lines total.

2.  **Analyze the Vault Data:**
    *   *Persona:* Silvio Chessari. clearly a hardware/software hacker focused on AI, specifically running local models on older/unsupported hardware and automating workflows.
    *   *Projects (Sviluppati & LLM Stack):*
        *   `ai-dashboard`: Python, Agenda, worker tasks.
        *   `bot-short`: C++, Telegram, SVG pipeline.
        *   `controller-termico-proattivo-esp32`: ESP32, Tesla P40 fan control (PWM, DS18B20), IPMI.
        *   `digital-thermal-lcd`: HID, 7-segment display, real-time monitoring.
        *   `megatool`: OSINT, C++ web app Flask, AI photo analysis (Ollama qwen2.5vl), Dark web agent.
        *   `openclaw`: Ollama gateway, Node.js.
        *   `reddit-monitor`: Python, AI/tech subreddit monitoring.
        *   `silvioprint`: Telegram bot content service.
        *   `cuda-sm61-compatibility-shim`: Pascal GPU (Tesla P40) compatibility.
        *   `add-video-input-support-to-llamacpp-mtmd`: Video input to llama.cpp (CMake, OpenCV).
        *   `ai-model-selector-physical-controller`: ESP32, OLED, rotary encoder, HID.
        *   `automated-exl2-conversion-validation-pipeline`: C++/Python, Qwen3.5 MoE architecture fix, quantization.
        *   `nllb-self-hosted-per-testo-multilingua`: NLLB-200, OCR+MT.
        *   `gguf-per-cohere-30b-a3b-su-p40`: Tesla P40 (BeeLLama), offloading.
        *   *LLM Stack:* AI Telemetry (Flask), FreeLLM API, Gateway Telegram, GGUF Manager, LLM Observability (FastAPI), Markitdown, Proxy Anthropic/OpenAI, Start-llama, Whisper API.

3.  **Drafting - Section by Section:**

    *   **Header:** Centered, 2 emojis max.
        *   *Draft:* `# Silvio Chessari 🚀 ⚙️` or `## Silvio Chessari 🧪 ⚡`. Let's use `# Silvio Chessari` with a bracket or title. The prompt asks for a centered header.

    *   **Bio:** 3 lines. Technical, precise.
        *   *Focus:* Local AI, Deep tech, Hardware hacking.
        *   *Draft:* Specializing in local LLM inference optimization and speculative decoding research. Architecting self-hosted AI infrastructure to run large models on legacy consumer hardware through low-level CUDA workarounds. Bridging embedded systems and high-performance compute with custom firmware and intelligent automation pipelines.

    *   **Stack Table:** Compact. Needs to cover the main tech mentioned (C++, Python, CUDA, Embedded, LLM tools).
        *   *Columns:* Domain, Technologies.
        *   *Content:* AI Inference (llama.cpp, EAGLE), Hardware (CUDA sm_61, ESP32), Backend (FastAPI, Flask, C++), Ops.

    *   **Project Sections:**
        *   *LLM Research:* Needs speculative decoding, MoE, video input.
            *   `add-video-input-support-to-llamacpp-mtmd` -> `video-input-llama-cpp`
            *   `automated-exl2-conversion-validation-pipeline` -> `exl2-conversion-pipeline`
            *   `cuda-sm61-compatibility-shim` -> `cuda-sm61-shim`
        *   *AI Infrastructure:* Dashboards, Gateways, Observability.
            *   `ai-dashboard` -> `ai-dashboard`
            *   `openclaw` -> `openclaw-gateway`
            *   `gateway-telegram-multimodale-offline` -> `telegram-gateway`
        *   *Tools & Automation:* OSINT, Monitors, Bots.
            *   `megatool` -> `megatool-osint`
            *   `reddit-monitor` -> `reddit-monitor`
            *   `gguf-model-manager-cli` -> `gguf-manager`
        *   *Embedded & Hardware:* ESP32, Fans, LCDs.
            *   `controller-termico-proattivo-esp32` -> `tesla-p40-fan-control`
            *   `digital-thermal-lcd` -> `thermal-lcd`
            *   `ai-model-selector-physical-controller` -> `model-selector-controller`

    *   **Refining Descriptions for "Real Technical Depth":**
        *   *exl2-pipeline:* Automated toolchain fixing Qwen3.5 MoE arch, converting to EXL2 with mixed quantization and C++ core.
        *   *cuda-shim:* Compatibility layer enabling CUDA sm_61 binaries for Tesla P40 via source-level patching and binary shims.
        *   *tesla-fan:* ESP32 firmware driving 24V PWM fans based on DS18B20 feedback and IPMI signals for proactive thermal throttling prevention.
        *   *megatool:* C++/Flask OSINT suite integrating Ollama vision models for EXIF analysis and dark web reconnaissance via Tor.

    *   **GitHub Stats:** Standard stats image at the bottom.

4.  **Review against Constraints:**
    *   *Length:* 90-120 lines. Need to be concise but detailed.
    *   *Emojis:* Only in header.
    *   *Links:* `[Name](https://github.com/chessarisilvio/slug)`
    *   *Language:* English.

5.  **Final Polish (Self-Correction during drafting):**
    *   *Name normalization:* Ensure slugs are lowercase and hyphenated.
    *   *Tone check:* "Bot Telegram grafica AI" -> "Telegram bot generating AI vector graphics".
    *   *Tech Depth check:* Ensure "EAGLE/MTP/speculative decoding" is mentioned in the bio or descriptions.
    *   *Structure check:* Header -> Bio -> Stack -> Projects (4 headers) -> Stats.

6.  **Constructing the Markdown:**

    (Simulating the output generation)
    *   *Bio:* Focus on EAGLE/MTP, sm_61.
    *   *Stack:* Table format.
    *   *Projects:* Grouped logically.

    Let's refine the slugs based on the prompt instructions (`lowercase, hyphens`).
    - `cuda-sm61-compatibility-shim` -> `cuda-sm61-compatibility-shim`
    - `automated-exl2-conversion-validation-pipeline` -> `automated-exl2-pipeline`
    - `tesla-p40-fan-control` (derived from controller-termico) -> `tesla-p40-esp32-controller`
    - `ai-dashboard` -> `ai-dashboard`
    - `megatool` -> `megatool`

    *Bio Draft:*
    Researching speculative decoding (EAGLE/MTP) and MoE routing to maximize LLM token throughput on limited hardware. Engineering custom inference runtimes to support sm_61 GPUs (Tesla P40) through manual CUDA patching and binary shims. Building end-to-end, self-hosted AI ecosystems ranging from embedded thermal controls to automated RAG pipelines.

    *Stack Table:*
    | Domain | Tech Stack |
    | :--- | :--- |
    | LLM Research | llama.cpp, Speculative Decoding, MoE Quantization, EXL2 |
    | Compute | CUDA (sm_61), OpenCL, Tesla P40, Local Deployment |
    | Embedded | ESP32, FreeRTOS, HID, PWM Control, Sensor Fusion |
    | Backend | C++, Python, FastAPI, Flask, Node.js, Systemd |

    *Projects Section Draft:*
    [cuda-sm61-compatibility-shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim) - Compatibility layer enabling modern LLM inference on Pascal GPUs (Tesla P40) by bypassing compiler checks and manipulating binary headers.
    [automated-exl2-pipeline](https://github.com/chessarisilvio/automated-exl2-pipeline) - C++/Python toolchain for fixing Qwen3.5 MoE architectures, converting to EXL2, and validating mixed-precision quantization.
    [video-input-llama.cpp](https://github.com/chessarisilvio/video-input-llama-cpp) - Extension of llama.cpp with CMake hooks and Python OpenCV bindings to stream real-time video frames into multimodal models.
    [tesla-p40-esp32-controller](https://github.com/chessarisilvio/tesla-p40-esp32-controller) - ESP32 firmware with DS18B20 sensors and PWM MOSFET driving for proactive Tesla P40 fan speed management via IPMI.
    [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) - Local monitoring system (Flask) tracking GPU telemetry, managing inference workers, and orchestrating automated agenda generation.
    [openclaw](https://github.com/chessarisilvio/openclaw) - Node.js gateway providing a unified API and control plane for local Ollama instances and model hot-swapping.
    [megatool](https://github.com/chessarisilvio/megatool) - C++ OSINT suite featuring Flask web interface, AI vision analysis (Ollama), and dark web reconnaissance agents.
    [thermal-lcd](https://github.com/chessarisilvio/thermal-lcd) - Python daemon interfacing with Thermalright LCD displays via USB HID to visualize real-time CPU/GPU load.

    *Reviewing line count and structure.*
    The prompt asks for 4 specific project sections: LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware.
    I need to split the drafted projects into these.

    *LLM Research:* cuda-shim, exl2-pipeline, video-input.
    *AI Infrastructure:* ai-dashboard, openclaw, telegram-gateway, llm-observability.
    *Tools & Automation:* megatool, reddit-monitor, gguf-manager.
    *Embedded:* tesla-p40-controller, thermal-lcd, physical-selector.

7.  **Final Code Generation:** (Proceeding to generate output).
    *   *