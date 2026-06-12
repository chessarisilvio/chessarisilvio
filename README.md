1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Subject:** Silvio Chessari.
    *   **Source Material:** "Technical vault data" (Obsidian notes style, Italian content but English code/technical terms).
    *   **Goal:** Generate a professional GitHub profile `README.md`.
    *   **Constraints:**
        *   Output ONLY the final markdown.
        *   No preamble, no explanation.
        *   English, technical, precise, no fluff.
        *   Show real technical depth (LLM inference, CUDA workarounds, self-built infrastructure, embedded).
        *   Structure:
            1.  Centered header (name + emojis, max 2).
            2.  3-line technical bio.
            3.  Compact stack table.
            4.  4 project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware).
            5.  GitHub stats (standard image).
        *   Project format: `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
        *   Slug derivation: lowercase, hyphens.
        *   Length: 90–120 lines total.

2.  **Analyze the Source Data (Vault Data):**
    *   *Language:* Italian notes, needs to be converted to English/Technical.
    *   *Projects identified:*
        *   **Sistema di Benchmarking Automatizzato (Auto-Quantization Pipeline GGUF):** Benchmark GGUF on P40/RTX3050, automated reports.
        *   **AI Dashboard:** Web dashboard (:9190), AGENDA.md integration, worker tasks.
        *   **bot-short:** Telegram bot, C++, SVG pipeline.
        *   **Controller Termico ESP32:** Proactive fan control + sensors.
        *   **Digital Thermal LCD:** HID display for temperature.
        *   **Megatool:** OSINT C++, Flask web app (:7788), AI photo analysis.
        *   **Reddit Monitor:** Scraper, feeds AGENDA.md.
        *   **Automazione Boot/Watchdog AI Avanzato:** Watchdog for llama-stack, Telegram notifications, systemd.
        *   **CUDA sm61 Compatibility Shim:** Shim for Pascal GPU (Tesla P40) to run new CUDA/LLM software.
        *   **Add video input support to llama.cpp (mtmd):** CMake mods, stub video input, Python OpenCV demo.
        *   **AI Model Selector Physical Controller:** ESP32, rotary encoder, OLED, HID.
        *   **Automated EXL2 Conversion & Validation Pipeline:** Fix architecture (Qwen3.5MoE), conversion, mixed quantization.
        *   **NLLB Self-Hosted:** Offline translation NLLB-200, OCR+MT pipeline.
        *   **mtop:** htop-like monitor for LLM inference (GPU metrics).
        *   **Git MCP Server:** MCP server for Git ops.
        *   **Qwen Image Edit Inpainting Workflow:** ComfyUI workflow.
    *   *Hardware mentioned:* Tesla P40 (sm_61), RTX 3050.
    *   *Techs mentioned:* CUDA, GGUF, EXL2, Ollama, Llama.cpp, ESP32, C++, Python, Flask, ComfyUI, Telegram Bot API.

3.  **Drafting Content - Step by Step:**

    *   **Header:** Silvio Chessari. Emojis: 🛠️ 🧠 (or similar, max 2).
    *   **Bio (3 lines):** Needs to cover LLM inference, CUDA hacks, embedded systems, and self-built infrastructure.
        *   *Draft:* Focus on LLM inference research (speculative decoding/exl2), running models on legacy data-center/consumer hardware via custom CUDA shims, and full-stack AI automation from embedded firmware to high-level orchestration.
    *   **Stack Table:** Languages, Infra, Hardware.
        *   *C++/Python/CMake*
        *   *CUDA/LLM/llama.cpp*
        *   *ESP32/Embedded*

    *   **Projects Section 1: LLM Research**
        *   *Add video input support to llama.cpp (mtmd)* -> `add-video-input-support-to-llamacpp-mtmd`
        *   *Automated EXL2 Conversion & Validation Pipeline* -> `automated-exl2-conversion-validation-pipeline`
        *   *Bias personalizzato per Whisper locale* -> `bias-personalizzato-per-whisper-locale`

    *   **Projects Section 2: AI Infrastructure**
        *   *CUDA sm61 Compatibility Shim* -> `cuda-sm61-compatibility-shim`
        *   *Sistema di Benchmarking Automatizzato* (Auto-Quantization Pipeline GGUF) -> `auto-quantization-pipeline-gguf`
        *   *mtop* -> `mtop-htop-per-monitoraggio-llm-locale`

    *   **Projects Section 3: Tools & Automation**
        *   *AI Dashboard* -> `ai-dashboard`
        *   *Automazione Boot/Watchdog AI Avanzato* -> `automazione-bootwatchdog-ai-avanzato`
        *   *Git MCP Server* -> `git-mcp-server-per-agenti-ai`

    *   **Projects Section 4: Embedded & Hardware**
        *   *Controller Termico ESP32* -> `controller-termico-proattivo-esp32`
        *   *AI Model Selector Physical Controller* -> `ai-model-selector-physical-controller`
        *   *Digital Thermal LCD* -> `digital-thermal-lcd`

4.  **Refining and Formatting:**

    *   *Constraint Check:* Are the links correct format? `https://github.com/chessarisilvio/slug`.
    *   *Constraint Check:* Are descriptions 1 line, technical?
    *   *Constraint Check:* Line count (90-120).

5.  **Writing the README (Iterative refinement):**

    *   *Header:* Simple.
    *   *Bio:* "Specializing in LLM inference optimization and speculative decoding techniques. Extensive experience deploying LLMs on unsupported hardware (Tesla P40 sm_61) via CUDA workarounds and custom shims. Build end-to-end AI infrastructure, from embedded firmware to automated orchestration pipelines."
    *   *Stack:*
        *   `Deep Learning | C++ / CUDA / Python | CMake / Bash`
        *   `LLM Ops | llama.cpp / GGUF / EXL2 / Ollama`
        *   `Hardware | NVIDIA Tesla P40 / ESP32 / Raspberry Pi`

    *   *Descriptions:*
        *   *mtop:* "htop-like CLI monitor for local LLM inference, visualizing real-time GPU utilization and token throughput."
        *   *CUDA shim:* "Compatibility layer enabling modern CUDA toolchains on legacy Pascal architecture (sm_61) Tesla P40 GPUs."
        *   *Controller:* "Proactive thermal management system for Tesla P40 using PID logic and custom ESP32 firmware."

6.  **Final Polish (Simulated):**

    *   *Header:* # Silvio Chessari 🛠️ 🧠
    *   *Bio:* Focus on the specific technical points requested: EAGLE/MTP (inferred from "mtmd"/inference research), speculative decoding (EXL2 implies inference optimization), unsupported hardware (Tesla P40).
    *   *Projects:* Ensure strictly 4 sections.
        *   *LLM Research:* `add-video-input-support-to-llamacpp-mtmd`, `automated-exl2-conversion-validation-pipeline`, `qwen-image-edit-inpainting-workflow`.
        *   *AI Infrastructure:* `cuda-sm61-compatibility-shim`, `auto-quantization-pipeline-gguf`, `mtop-htop-per-monitoraggio-llm-locale`.
        *   *Tools & Automation:* `ai-dashboard`, `automazione-bootwatchdog-ai-avanzato`, `git-mcp-server-per-agenti-ai`.
        *   *Embedded & Hardware:* `controller-termico-proattivo-esp32`, `ai-model-selector-physical-controller`, `digital-thermal-lcd`.

    *   *Formatting:* Use standard markdown tables. Use headers clearly.

7.  **Line Count Management:**
    *   Intro + Bio: ~10 lines.
    *   Stack: ~5 lines.
    *   Projects: 4 sections x ~6 lines = ~24 lines.
    *   Stats: ~5 lines.
    *   Total might be low, need to ensure spacing is appropriate but not excessive fluff. I will use standard markdown headers and consistent spacing. I will ensure the project descriptions are dense to add "technical weight" without word count.

8.  **Final Code Assembly (Mental Verification against "No preamble"):**
    *   Start directly with `#`.

    *(Self-Correction during drafting)*: The prompt mentions "EAGLE/MTP/speculative decoding" in the requirements but they aren't explicitly in the snippet, except "mtmd" (Multi-Modal?). The prompt says "Use real technical details from the vault data below". The *Requirements* section says "Show real technical depth: LLM inference research (EAGLE/MTP...)". I should stick to the vault data for the *projects*, but I can use the *bio* to summarize the intent if supported by the data. Actually, looking closer at the vault, "mtmd" is in the filename `add-video-input-support-to-llamacpp-mtmd`. "MTP" isn't explicitly defined, but speculative decoding is strongly implied by EXL2/Llama.cpp focus. I will stick to the vault data for the project details to ensure accuracy, as "Show real technical details from the vault data below" is a specific instruction overriding the generic requirement list if there's a conflict. I will focus on what *is* there: CUDA shims, EXL2 pipeline, watchdog, video input.

    *Re-reading Prompt constraints:* "Use real technical details from the vault data below".
    Okay, I will use the specific project names and technical descriptions found in the Italian text.

    *Translating specific terms:*
    - "Sistema di Benchmarking Automatizzato per Nuovi Modelli GGUF" -> `gguf-benchmark-system` (or `sistema-di-benchmarking-automatizzato...`) -> I'll use English slugs where possible or exact hyphenated lowercase of the title. The prompt says "derived from project names (lowercase, hyphens)".
    - "cuda-sm61-compatibility-shim" (already mostly English).
    - "automazione-bootwatchdog-ai-avanzato" -> "automazione-bootwatchdog-ai-avanzato"

    Let's refine the Bio to be very strong based on the "Tesla P40", "sm_61", "CUDA workaround" themes.

    *Bio draft 2:*
    Deep focus on LLM inference optimization and experimental feature implementation (video input, MoE routing). Expert in enabling modern AI stacks on legacy data-center hardware (Tesla P40 sm_61) through custom CUDA shims and build system manipulation. Architect of self-hosted AI infrastructure integrating embedded controllers, automated watchdogs, and orchestration pipelines.

    *Stack:*
    Languages: C++ (STL/Bot), Python (Automation/Scripts), CMake
    Inference: llama.cpp, GGUF, EXL2, Ollama
    Hardware: NVIDIA Tesla P40 (Pascal), ESP32, OpenCL

    Let's generate.

    *Structure:*
    1. Header
    2. Bio