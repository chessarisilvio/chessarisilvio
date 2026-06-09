1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Task:** Generate a GitHub profile README.md for Silvio Chessari.
    *   **Input:** Technical vault data (mixed Italian/English, containing project lists, paths, and descriptions).
    *   **Requirements:**
        *   Output ONLY the final README.md.
        *   English, technical, precise, no fluff.
        *   Show depth: LLM research (EAGLE, MTP, speculative decoding, MoE routing), running LLMs on unsupported GPUs (Tesla P40 sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.
        *   Structure:
            1.  Centered header.
            2.  3-line technical bio.
            3.  Compact stack table.
            4.  4 project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware).
            5.  GitHub stats.
        *   Project format: `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
        *   Slug derivation: Lowercase, hyphens.
        *   Max 2 emojis (header only).
        *   Length: 90–120 lines.

2.  **Analyze the Input Data (Vault):**
    *   *User:* Silvio Chessari.
    *   *Keywords/Topics:* LLMs, CUDA, Tesla P40, ESP32, Python, C++, Node.js, Dashboard, Automation, Video Input, EXL2 quantization.
    *   *Projects (Sviluppati - Developed):*
        *   `ai-dashboard` -> Python, monitoring, local automation.
        *   `bot-short` -> C++, Telegram bot, AI SVG graphics.
        *   `controller-termico-proattivo-esp32` -> ESP32, Fan control, Tesla P40, IPMI, OneWire.
        *   `digital-thermal-lcd` -> Python, HID, Thermalright display, CPU/GPU stats.
        *   `openclaw` -> Node.js, Gateway Ollama/LLaMA, Telegram skills.
        *   `silvioprint` -> Python, Telegram bot, content strategy.
        *   `launcher-avanzato-per-llama-server` -> Bash/Python, launcher.
        *   `cuda-sm61-compatibility-shim` -> CUDA workarounds for Tesla P40 (sm_61).
        *   `add-video-input-support-to-llamacpp-mtmd` -> llama.cpp, CMake, video frame inference, OpenCV.
        *   `ai-model-selector-physical-controller` -> ESP32, HID, rotary encoder, OLED.
        *   `automated-exl2-conversion-validation-pipeline` -> C++/Python, Qwen3.5 MoE, quantization, workflow.
    *   *LLM Stack (Infra):*
        *   `dashboard-telemetrica-ai-hardware` -> Flask, hardware telemetry.
        *   `freellmapi` -> Proxy for Groq, Google, etc.
        *   `gateway-telegram-multimodale-offline` -> Multimodal Telegram.
        *   `gguf-model-manager-cli` -> CLI for models.
        *   `llm-observability` -> FastAPI, Plotly, Prometheus metrics.
        *   `markitdown` -> Ingestion RAG.
        *   `proxy-anthropicopenai-con-safety-hooks` -> Security proxy.
        *   `whisperapi-self-hosted` -> STT.
        *   `llama-cpp-benchmark-suite` -> Benchmarking.

3.  **Drafting Content - Section by Section:**

    *   **Header:** Needs to be centered.
        *   `# Silvio Chessari`
        *   Subtext: "LLM Inference Research & AI Infrastructure engineer specializing in speculative decoding, CUDA hackery, and embedded systems." (Need to keep it concise, maybe just the name and title).

    *   **Bio (3 lines):**
        *   Focus on the prompt's keywords: EAGLE/MTP/speculative decoding, Tesla P40 (sm_61), self-built infra.
        *   *Draft:*
            *   Researching efficient LLM inference via speculative decoding, MoE routing, and speculative sampling methods.
            *   Architecting self-hosted AI stacks on unsupported hardware (e.g., Tesla P40 sm_61) using custom CUDA shims.
            *   Developing embedded control systems and automation pipelines bridging physical hardware with generative models.

    *   **Stack Table:**
        *   Columns: Domain, Tech.
        *   *Inference:* llama.cpp, EXL2, vLLM.
        *   *Languages:* C++, Python, Bash.
        *   *Hardware:* CUDA (sm_61), ESP32, OneWire.
        *   *Infra:* Docker, FastAPI, Flask, Node.js.

    *   **Project Sections & Sorting:**

        *   *LLM Research:*
            *   `automated-exl2-conversion-validation-pipeline` -> Automated EXL2 conversion and validation pipeline for Qwen3.5 MoE with mixed quantization.
            *   `add-video-input-support-to-llamacpp-mtmd` -> Patched llama.cpp for video frame ingestion via OpenCV and webcam inference.
            *   (Maybe mention speculative decoding context in descriptions if possible, or just stick to the specific projects). Let's stick to the projects listed.

        *   *AI Infrastructure:*
            *   `llm-observability` -> FastAPI and Plotly-based monitoring dashboard for Prometheus metrics from llama-server.
            *   `dashboard-telemetrica-ai-hardware` -> Flask telemetry dashboard tracking GPU/RAM utilization with Telegram alerting.
            *   `freellmapi` -> Unified aggregation proxy for cloud endpoints (Kilo, Groq, Cerebras) providing fallback routing.

        *   *Tools & Automation:*
            *   `openclaw` -> Node.js gateway for LLaMA/Ollama with persistent session memory and multi-channel skill routing.
            *   `gguf-model-manager-cli` -> CLI utility for managing local GGUF model repositories and metadata.
            *   `silvioprint` -> Python-based Telegram bot for automated content generation and channel management.
            *   `cuda-sm61-compatibility-shim` -> Compatibility layer enabling modern LLM binaries on legacy Pascal (Tesla P40) architectures.

        *   *Embedded & Hardware:*
            *   `controller-termico-proattivo-esp32` -> Proactive thermal management firmware for Tesla P40 using DS18B20 sensors and PWM control.
            *   `ai-model-selector-physical-controller` -> ESP32 rotary encoder and OLED interface for hardware-triggered model switching via HID.
            *   `digital-thermal-lcd` -> HID driver for Thermalright LCD displaying real-time thermal data.

    *   **GitHub Stats:**
        *   Standard image placeholders: `chessarisilvio`, `chessarisilvio?show_icons=true&hide_border=true`.

4.  **Refining and Formatting (Line Count check & Constraints):**
    *   *Constraint:* Max 2 emojis total (header only).
    *   *Constraint:* 90-120 lines total.
    *   *Constraint:* Output ONLY markdown.
    *   *Language:* English, technical.

    *Let's build the Markdown structure.*

    ```markdown
    <div align="center">

    # Silvio Chessari
    ### LLM Inference Research & AI Infrastructure

    </div>

    I specialize in efficient LLM inference, speculative decoding, and optimizing models for unsupported consumer/datacenter GPUs.
    Building self-hosted AI stacks from scratch, hacking CUDA drivers for legacy hardware, and integrating embedded systems with LLMs.
    Focused on low-latency architecture, MoE routing strategies, and bridging physical hardware interfaces with generative AI.

    ### 💻 Technical Stack

    | Domain | Technologies |
    |--------|--------------|
    | **LLM Research** | Speculative Decoding, MoE Routing, MTMD, EAGLE, EXL2 Quantization |
    | **Inference Engines** | llama.cpp, vLLM, TensorRT-LLM, Ollama |
    | **Systems** | CUDA (sm_61), Coreboot, IPMI, Linux Kernel Modules |
    | **Embedded** | ESP32, OneWire, I2C, HID, C++ Firmware |
    | **DevOps** | Docker, systemd, FastAPI, Flask, Node.js |
    | **Languages** | Python, C++, Shell, CMake |

    <br>

    ## 🐦 LLM Research & Optimization

    - [Automated EXL2 Conversion & Validation Pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline)
       Toolchain for fixing Qwen3.5 MoE architectures, EXL2 conversion, mixed quantization, and benchmark validation.
    - [Add Video Input to llama.cpp (MTMD)](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd)
       Patch enabling webcam/video frame ingestion in llama.cpp via CMake modifications and OpenCV bindings.
    - [CUDA sm_61 Compatibility Shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim)
       Runtime patches allowing modern LLM binaries to execute on legacy Pascal GPUs (Tesla P40) bypassing arch checks.

    <br>

    ## 🏗️ AI Infrastructure

    - [LLM Observability](https://github.com/chessarisilvio/llm-observability)
       Real-time metrics dashboard using FastAPI and Plotly to monitor Prometheus data from llama-server instances.
    - [AI Telemetry Dashboard](https://github.com/chessarisilvio/dashboard-telemetrica-ai-hardware)
       Flask-based hardware monitor tracking VRAM, temperatures, and system loads with Telegram alert integration.
    - [FreeLLM API](https://github.com/chessarisilvio/freellmapi)
       Unified proxy managing routing and fallback logic across multiple free cloud inference providers (Groq, Google, Cerebras).
    - [Whisper API Self-Hosted](https://github.com/chessarisilvio/whisperapi-self-hosted)
       Local STT service wrapper around faster-whisper for integration into offline AI pipelines.

    <br>

    ## 🛠️ Tools & Automation

    - [OpenClaw](https://github.com/chessarisilvio/openclaw)
       Node.js multi-channel gateway for Ollama/LLaMA featuring persistent session memory, tool use, and skill routing.
    - [GGUF Manager CLI](https://github.com/chessarisilvio/gguf-model-manager-cli)
       Command-line utility for organizing, validating, and managing local GGUF model repositories.
    - [AI Dashboard](https://github.com/chessarisilvio/ai-dashboard)
       Local monitoring automation center integrating hardware stats, sprint agendas, and task management with LLM generation.
    - [Anthropic/OpenAI Safety Proxy](https://github.com/chessarisilvio/proxy-anthropicopenai-con-safety-hooks)
       Intermediate proxy layer enforcing custom safety hooks and content filtering on API requests.

    <br>

    ## 🔌 Embedded & Hardware

    - [ESP32 Proactive Thermal Controller](https://github.com/chessarisilvio/controller-termico-proattivo-esp32)
       Firmware managing Tesla P40 fan curves via PWM, utilizing DS18B20 sensors and IPMI for proactive thermal throttling.
    - [AI Model Selector Physical Controller](https://github.com/chessarisil