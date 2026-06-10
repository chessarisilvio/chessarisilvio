1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Subject:** Silvio Chessari.
    *   **Task:** Generate a GitHub `README.md` based on provided "vault data" (technical notes).
    *   **Constraints:**
        *   Output ONLY the markdown (no preamble).
        *   Language: English, technical, precise (no fluff).
        *   Focus: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), running LLMs on unsupported GPUs (Tesla P40 sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.
        *   Structure: Centered header -> 3-line technical bio -> compact stack table -> 4 project sections (LLM Research, AI Infrastructure, Tools & Automation, Embedded & Hardware) -> GitHub stats.
        *   Project format: `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
        *   Repo slugs: Lowercase, hyphens.
        *   Max 2 emojis (header only).
        *   Line count: 90–120 lines.

2.  **Analyze the Source Data (Vault Data):**

    *   **Identity:** Silvio Chessari.
    *   **Core Themes:**
        *   LLM Research (Speculative decoding, MoE, video input to LLMs).
        *   Hardware Hacking (Tesla P40, ESP32, thermal control, CUDA sm_61 compatibility).
        *   Infrastructure (Dashboards, RAG, telemetry, proxies).
        *   Tools (Bots, CLI tools, automation).

    *   **Projects (Source -> Mapping):**
        *   `CUDA sm_61 Compatibility Shim`: *LLM Research* (Hardware support).
        *   `Add video input support to llama.cpp (mtmd)`: *LLM Research* (Multimodal).
        *   `Automated EXL2 Conversion & Validation Pipeline`: *LLM Research* (Quantization/Tooling).
        *   `AI Dashboard`: *AI Infrastructure* (Telemetry).
        *   `AI Telemetry`: *AI Infrastructure* (Metrics).
        *   `LLM Observability`: *AI Infrastructure* (Plotly/Prometheus).
        *   `Markitdown`: *AI Infrastructure* (Ingestion).
        *   `FreeLLM API`: *AI Infrastructure* (Proxy).
        *   `bot-short`: *Tools & Automation* (SVG generation).
        *   `Megatool`: *Tools & Automation* (OSINT).
        *   `Controller Termico ESP32`: *Embedded & Hardware* (Fan control).
        *   `Digital Thermal LCD`: *Embedded & Hardware* (HID display).
        *   `AI Model Selector Physical Controller`: *Embedded & Hardware* (Physical interface).

3.  **Drafting - Section by Section:**

    *   **Header:** Centered, Name, Role, 2 emojis max.
        *   `<div align="center">`
        *   `# Silvio Chessari`
        *   `Systems Engineer & LLM Researcher 🚀 🔬` (Emojis used here).

    *   **Technical Bio:** 3 lines, specific depth.
        *   *Draft 1:* Focused on optimizing LLM inference on consumer and legacy datacenter hardware using speculative decoding and MoE routing.
        *   *Draft 2:* Specializing in CUDA sm_61 compatibility to run modern models on Tesla P40s, along with building self-hosted AI infrastructure and embedded control systems.
        *   *Draft 3:* Active research in EAGLE/MTP speculative decoding, EXL2 quantization pipelines, and multimodal inputs for local inference engines.

    *   **Compact Stack Table:**
        *   Columns: Research, Infrastructure, Embedded.
        *   Content: Python/C++/CUDA, llama.cpp/Ollama, ESP32/CircuitPython.

    *   **Project Section 1: LLM Research:**
        *   *CUDA sm_61 Compatibility Shim* -> `[cuda-sm61-compatibility-shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim)`: Compatibility layer enabling modern CUDA kernels on Pascal GPUs (Tesla P40) for local LLM inference.
        *   *Add video input support to llama.cpp (mtmd)* -> `[add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd)`: Extends `llama.cpp` to process webcam and video frames as input for vision-language models via CMake and Python bindings.
        *   *Automated EXL2 Conversion & Validation Pipeline* -> `[automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline)`: C++/Python toolchain for converting Qwen3_5 MoE architectures to EXL2 with mixed quantization and automated validation benchmarks.

    *   **Project Section 2: AI Infrastructure:**
        *   *AI Dashboard* -> `[ai-dashboard](https://github.com/chessarisilvio/ai-dashboard)`: Web-based telemetry stack for monitoring GPU/VRAM utilization and orchestrating local LLM workflows.
        *   *LLM Observability* -> `[llm-observability](https://github.com/chessarisilvio/llm-observability)`: FastAPI service aggregating Prometheus metrics from llama-server with real-time Plotly visualization.
        *   *Markitdown* -> `[markitdown](https://github.com/chessarisilvio/markitdown)`: ingestion pipeline converting PDF/DOCX/XLSX into vector embeddings for ChromaDB RAG systems.
        *   *FreeLLM API* -> `[freellmapi](https://github.com/chessarisilvio/freellmapi)`: Unified proxy gateway aggregating free cloud inference providers (Groq, Google, Cerebras) with fallback logic.

    *   **Project Section 3: Tools & Automation:**
        *   *bot-short* -> `[bot-short](https://github.com/chessarisilvio/bot-short)`: Telegram bot pipeline generating high-fidelity vector graphics (SVG/EPS) using local AI models.
        *   *Megatool* -> `[megatool](https://github.com/chessarisilvio/megatool)`: Multi-module OSINT suite featuring AI photo analysis (GPS/EXIF), dark web scraping, and automated HTML reporting.

    *   **Project Section 4: Embedded & Hardware:**
        *   *Controller Termico Proattivo ESP32* -> `[controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32)`: 1-Wire thermal management system for Tesla P40 using PWM fan control and IPMI communication.
        *   *Digital Thermal LCD* -> `[digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd)`: HID driver interfacing with 7-segment LCDs to display real-time system temperatures and load.
        *   *AI Model Selector Physical Controller* -> `[ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller)`: ESP32-based rotary controller with OLED display for switching local AI models via HID keyboard emulation.

    *   **GitHub Stats:** Standard image links (common placeholders are fine, or just the markdown syntax).

4.  **Refining and Formatting:**

    *   Check constraints: "No fluff", "English", "Technical".
    *   Slug generation:
        *   `cuda-sm61-compatibility-shim`
        *   `add-video-input-support-to-llamacpp-mtmd`
        *   `automated-exl2-conversion-validation-pipeline`
        *   `ai-dashboard`
        *   `llm-observability`
        *   `markitdown`
        *   `freellmapi`
        *   `bot-short`
        *   `megatool`
        *   `controller-termico-proattivo-esp32`
        *   `digital-thermal-lcd`
        *   `ai-model-selector-physical-controller`
    *   Line count check: Need to ensure it lands between 90 and 120.
    *   Structure check: Header -> Bio -> Table -> 4 Sections -> Stats.

5.  **Final Polish (Self-Correction during drafting):**
    *   *Bio:* Ensure the "Tesla P40" and "EAGLE/MTP" mentions are there as requested.
    *   *Descriptions:* Keep them tight. 1 line each.
    *   *Table:* Use standard markdown table syntax.
    *   *Stats:* Use `github-readme-stats` or similar visualizer placeholders as they are standard in tech READMEs.

    *(Self-Correction on layout)*: The prompt asks for "compact stack table". A 3-column table fits well.
    *(Self-Correction on content)*: Ensure "Silvio Chessari" is the user handle. The prompt implies the user is `chessarisilvio` based on the link requirement `https://github.com/chessarisilvio/slug`.

6.  **Constructing the Output (Mental Simulation):**

    ```markdown
    <div align="center">
    # Silvio Chessari
    ### Researching LLM Inference & Heterogeneous Computing 🚀 🔬
    </div>

    Specializing in speculative decoding (EAGLE/MTP) and MoE routing optimizations to maximize LLM performance on consumer hardware.
    Engineering compatibility shims for sm_61 architecture (Tesla P40) to run modern CUDA stacks on unsupported legacy GPUs.
    Architecting self-hosted AI infrastructure, RAG pipelines, and embedded control systems for thermal management and physical interfaces.

    ### Technical Stack
    | **Research** | **Infrastructure** | **Embedded** |
    | :--- | :--- | :--- |
    | PyTorch / llama.cpp | Docker / systemd | ESP32 / C++ |
    | EXL2 / GGUF quantization | FastAPI / Flask | HID / USB protocols |
    | MoE / Speculative Decoding | Prometheus / Grafana | 1-Wire / PWM |

    ### LLM Research
    [cuda-sm61-compatibility-shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim) - Compatibility layer enabling modern LLM CUDA kernels on Pascal sm_61 GPUs (Tesla P40).
    [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) - Multimodal extension for `llama.cpp` ingesting live webcam/video frames via CMake and Python bindings.
    [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) - C++/Python toolchain for Qwen3_5 MoE quantization to EXL2 with automated benchmarking.

    ### AI Infrastructure
    [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) - Local telemetry stack monitoring GPU VRAM, thermal states, and orchestrating LLM workloads.
    [llm-observability](https://github.com/chessarisilvio/llm-observability) - FastAPI service aggregating Prometheus metrics from `llama-server` with real-time Plotly visualizations.
    [markitdown](https://github.com/chessarisilvio/markitdown) - RAG ingestion pipeline converting PDF/DOCX/XLSX documents into