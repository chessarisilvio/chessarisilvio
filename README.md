1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **User:** Silvio Chessari.
    *   **Input:** Vault data (Obsidian markdown) containing project details, taxonomy, and technical specificities.
    *   **Output:** `README.md` file content ONLY. No preamble, no explanation.
    *   **Style/Tone:** English, technical, precise, no fluff.
    *   **Key Technical Focus:** LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), running LLMs on unsupported/consumer GPUs (Tesla P40 sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.
    *   **Structure:**
        1.  Centered header.
        2.  3-line technical bio.
        3.  Compact stack table.
        4.  4 Project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware).
        5.  GitHub stats section (standard placeholder).
    *   **Project Format:** `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
    *   **Constraints:** Max 2 emojis (header only), real technical details, specific slug style, 90–120 lines total.

2.  **Analyze the Vault Data (Source Extraction):**
    *   *User:* Silvio Chessari.
    *   *Tech Focus:* "sm_61", "Tesla P40", "RTX 3050", "Speculative decoding", "MoE", "CUDA", "GGUF", "EXL2", "llama.cpp", "Video input".
    *   *Biography elements:* Local AI inference, hardware optimization, embedded systems integration.
    *   *Projects:*
        *   *LLM Research:*
            *   `add-video-input-support-to-llamacpp-mtmd`: Video input for llama.cpp (CMake, stub, Python/OpenCV).
            *   `automated-exl2-conversion-validation-pipeline`: EXL2 conversion, mixed quantization, Qwen3_5MoeForC architecture fix.
            *   `sistema-di-benchmarking-automatizzato-per-nuovi-mo` (GGUF Benchmarking): GGUF benchmarking on P40/3050, auto reports.
            *   `auto-quantization-pipeline-gguf`: Automated GGUF quantization pipeline.
        *   *AI Infrastructure:*
            *   `ai-home-assistant-hid-dashboard`: Arduino R4 WiFi, ESP32, MQTT/Tailscale, monitoring P40/3050 status.
            *   `automazione-bootwatchdog-ai-avanzato`: Watchdog for llama-stack (process, VRAM, t/s metrics), Telegram alerts.
            *   `ai-dashboard`: Web dashboard (:9190), GPU panels, local agenda integration.
        *   *Tools & Automation:*
            *   `mtop-htop-per-monitoraggio-llm-locale`: htop-like monitor for LLM inference (real-time metrics).
            *   `nllb-self-hosted-per-testo-multilingua`: Offline NLLB-200, OCR+MT pipeline.
            *   `bot-short`: Telegram bot (C++), AI vector graphics, SVG pipeline.
        *   *Embedded & Hardware:*
            *   `cuda-sm61-compatibility-shim`: Compatibility shim for Pascal GPUs (Tesla P40).
            *   `ai-model-selector-physical-controller`: ESP32, rotary encoder, OLED, HID input for model selection.
            *   `controller-termico-proattivo-esp32`: ESP32 fan control + sensors.
            *   `digital-thermal-lcd`: LCD temp display via HID.

3.  **Drafting the Content:**

    *   **Header:** Centered, name, maybe "AI Systems Engineer" or "Research Engineer".
    *   **Bio:** Needs to be 3 lines, high-level technical.
        *   *Draft:* Specializing in local LLM inference optimization and speculative decoding research on legacy hardware. Building self-hosted AI infrastructure and embedded interfaces for distributed computing. Deep focus on CUDA workarounds (sm_61), MoE routing, and custom tooling for unsupported GPUs.
    *   **Stack Table:** Needs to be compact. Languages: C++, Python, Cuda. Frameworks: llama.cpp, PyTorch. HW: ESP32, Tesla P40, Arduino.
    *   **Project Sections (Mapping to requested structure):**
        *   *Section 1: LLM Research & Optimization* -> `add-video-input...`, `automated-exl2...`, `sistema-di-benchmarking...`.
        *   *Section 2: AI Infrastructure & Orchestration* -> `automazione-bootwatchdog...`, `ai-home-assistant...`, `ai-dashboard`.
        *   *Section 3: Tools & Automation* -> `mtop-htop...`, `nllb-self-hosted...`, `bot-short`.
        *   *Section 4: Embedded & Hardware* -> `cuda-sm61...`, `ai-model-selector...`, `controller-termico...`.
    *   **Refining Project Descriptions (1 line, technical):**
        *   *Video:* CMake integration and Python demo enabling video frame streaming into llama.cpp inference.
        *   *EXL2:* CLI pipeline for Qwen MoE architecture fixes and mixed-precision EXL2 conversion.
        *   *Benchmarking:* Automated GGUF validation on Tesla P40/RTX 3050 with auto-generated reporting.
        *   *Watchdog:* Advanced systemd supervisor monitoring VRAM and throughput for llama-stack with Telegram alerts.
        *   *HID Dashboard:* Arduino R4/ESP32 hardware interface monitoring P40 state via MQTT/Tailscale.
        *   *Dashboard:* Web-based local AI stack monitor featuring GPU telemetry and sprint integration.
        *   *mtop:* htop-derived CLI utility for real-time token throughput and GPU utilization tracking.
        *   *NLLB:* Self-hosted NLLB-200 pipeline combining offline OCR and multilingual machine translation.
        *   *Bot Short:* C++ Telegram bot generating AI vector graphics via SVG pipelines.
        *   *CUDA Shim:* Compatibility layer enabling Pascal (sm_61) support for modern CUDA toolchains.
        *   *Model Selector:* ESP32 rotary controller with HID emulation for physical LLM model switching.
        *   *Thermal Ctrl:* PID-based fan control and sensor array integration for thermal management.

4.  **Formatting & Constraints Check:**
    *   *Emojis:* Only in header. Let's use ⚡️ or 🧠. Let's go with minimal technical icon.
    *   *Slugs:*
        *   `add-video-input...` -> `llamacpp-video-input`
        *   `automated-exl2...` -> `exl2-pipeline`
        *   `sistema-di-benchmarking...` -> `gguf-benchmark-p40`
        *   `automazione-bootwatchdog...` -> `llama-stack-watchdog`
        *   `ai-home-assistant...` -> `hid-dashboard-arduino`
        *   `ai-dashboard` -> `ai-stack-dashboard`
        *   `mtop...` -> `mtop-llm-monitor`
        *   `nllb...` -> `nllb-offline-ocr`
        *   `bot-short` -> `bot-short-svg`
        *   `cuda-sm61...` -> `cuda-sm61-shim`
        *   `ai-model-selector...` -> `esp32-model-selector`
        *   `controller-termico...` -> `esp32-thermal-controller`
    *   *Links:* `https://github.com/chessarisilvio/[slug]`
    *   *Line Count:* Needs to be 90-120. I need to ensure the layout has enough spacing/structure to hit this, or the list is robust enough.

5.  **Constructing the Markdown (Iterative Refinement):**

    *   *Bio Tuning:* "Specializing in LLM inference research (EAGLE/MTP) and speculative decoding on unsupported consumer hardware." -> "Architecting local AI inference pipelines with a focus on speculative decoding, MoE routing, and CUDA optimization for legacy hardware (sm_61)." -> "Building self-hosted intelligence infrastructure and embedded systems interfaces for real-time monitoring and control."

    *   *Stack:*
        | C++ | Python | CUDA | CMake | Bash |
        | :--- | :--- | :--- | :--- | :--- |
        | llama.cpp | PyTorch | OpenCV | ESP-IDF | Arduino |

    *   *Stats:* Standard GitHub stats image links.

6.  **Final Polish (Simulating the Output):**

    ```markdown
    <h1 align="center">Silvio Chessari</h1>
    <p align="center">⚡️ AI Systems Engineer & Hardware Optimization Specialist</p>

    Architecting local AI inference pipelines with a focus on speculative decoding, MoE routing, and CUDA optimization for ...
    ```

    *Let's check specific project details from the notes for the descriptions.*
    *   `add-video-input...`: "Input video per llama.cpp: CMake, stub video input, script demo Python con OpenCV" -> Implements video input ingestion for llama.cpp, including CMake configuration and OpenCV-based demo scripts.
    *   `cuda-sm61...`: "Shim di compatibilità CUDA sm_61 per GPU Pascal (Tesla P40)" -> Compatibility layer enabling modern CUDA toolchains to execute on Pascal-based Tesla P40 GPUs (sm_61).

    *Line count estimation:*
    Header: 2
    Bio: 3
    Stack: 2
    Section Headers: 4
    Projects: 12
    Stats: 2
    Blank lines: ~15-20.
    Total lines approx 40-50. I need to pad the spacing or add more detail to descriptions (without being fluff) or ensure formatting takes up vertical space (standard markdown lists). Wait, the requirement is 90-120 lines. I need to ensure the content is dense or the spacing is generous but within "compact stack table".
    *Actually, let's make the bio tighter and maybe split the stack into a cleaner table.*
    *Re-evaluating line count:* A standard README with 12 projects and a stack table usually hits 70-90 lines. To hit 90-120, I will ensure standard markdown spacing (double newlines between sections) and ensure the bio is distinct lines.

    *Self-Correction on Links:* The prompt asks for `https://github.com/chessarisilvio/slug`. I will use the slugs I derived.

    *Bio Text Finalization:*
    Specializing in local LLM inference research focusing on speculative decoding (EAGLE/MTP) and MoE routing on unsupported hardware.
    Developer of self-hosted AI infrastructure, including automated quantization pipelines and custom CUDA workarounds for Tesla P40 (sm_61).
    Integrating embedded systems (ESP32/Arduino) with high-performance computing stacks via HID/MQTT interfaces for physical computing control.

7.  **Final Code Generation:** (Proceeding to generate the markdown block).

    *   *Section 1: LLM Research & Optimization*
    *   *Section 2: AI Infrastructure & Orchestration*
    *   *Section 3: Tools & Automation*
    *   *Section 4: Embedded & Hardware*

    *Checking the specific "no fluff" rule:* Descriptions must be technical.
    *   `sistema-di-benchmarking...`: Automated GGUF benchmarking suite targeting Tesla P40 and RTX 3050