1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Output:** GitHub `README.md` markdown file.
    *   **Constraint:** ONLY the final markdown (no preamble, no explanation).
    *   **Tone:** English, technical, precise, no fluff.
    *   **Key Content (Technical Depth):** LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), running LLMs on unsupported consumer/datacenter GPUs (Tesla P40 sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.
    *   **Source Material:** Provided "VAULT DATA" containing project details, paths, and descriptions in Italian/mixed English.
    *   **Structure:**
        1.  Centered header.
        2.  3-line technical bio.
        3.  Compact stack table.
        4.  4 Project sections (LLM Research, AI Infrastructure, Tools & Automation, Embedded & Hardware).
        5.  GitHub stats (images).
    *   **Project Format:** `[name](https://github.com/chessarisilvio/slug) + 1-line technical description`.
    *   **Slug Rule:** lowercase, hyphens.
    *   **Emoji Constraint:** Max 2 in the header only.
    *   **Length:** 90–120 lines total.

2.  **Process the Vault Data:**

    *   *Bio Sources:*
        *   `cuda-sm61-compatibility-shim`: Tesla P40 (sm_61), CUDA workarounds.
        *   `automated-exl2-conversion-validation-pipeline`: MoE, quantization, EXL2 conversion, benchmarking.
        *   `add-video-input-support-to-llamacpp-mtmd`: llama.cpp, video input, C++.
        *   `ai-dashboard`: Monitoring, AGENDA, 35B local LLM.
        *   `controller-termico-proattivo-esp32`: Tesla P40 fan control, ESP32, thermal management.

    *   *Project Mapping:*

        *   **LLM Research:**
            *   `automated-exl2-conversion-validation-pipeline` -> slug: `automated-exl2-conversion-validation-pipeline`. Desc: Toolchain for Qwen 3.5 MoE EXL2 conversion, quantization fix, and automated benchmarking.
            *   `add-video-input-support-to-llamacpp-mtmd` -> slug: `add-video-input-support-to-llamacpp-mtmd`. Desc: Patched llama.cpp for video input integration with OpenCV and CMake build tweaks.
            *   *Inferred:* `cuda-sm61-compatibility-shim` (Fits here or Infrastructure, but specifically mentions CUDA workarounds for P40). Let's put it in Research or Infrastructure. Given it's a "Compatibility Shim", it's low-level CUDA work. Research fits well.

        *   **AI Infrastructure:**
            *   `start-llama` -> slug: `start-llama`. Desc: YAML-configured launcher for llama-server with 5 presets and environment management.
            *   `llama-cpp-benchmark-suite` -> slug: `llama-cpp-benchmark-suite`. Desc: CLI benchmark suite validating token throughput and VRAM usage on consumer GPUs.
            *   `freellmapi` -> slug: `freellmapi`. Desc: High-performance proxy aggregating Kilo, Groq, Google, and Cerebras endpoints.
            *   `markitdown` (from llm-stack) -> slug: `markitdown`. Desc: CLI ingestion pipeline converting office docs to ChromaDB embeddings for RAG.

        *   **Tools & Automation:**
            *   `ai-dashboard` -> slug: `ai-dashboard`. Desc: Local web dashboard for GPU telemetry, service monitoring, and AGENDA-driven automation.
            *   `reddit-monitor` -> slug: `reddit-monitor`. Desc: Python script scraping AI/tech subreddits to feed ideas into local AGENDA tasks.
            *   `openclaw` -> slug: `openclaw`. Desc: Multi-channel AI gateway with skills, session memory, and tool use integration.
            *   `megatool` -> slug: `megatool`. Desc: OSINT suite profiling entities via vision AI, EXIF data analysis, and Tor crawling.

        *   **Embedded & Hardware:**
            *   `controller-termico-proattivo-esp32` -> slug: `controller-termico-proattivo-esp32`. Desc: ESP32 firmware for proactive Tesla P40 thermal management via sensor-driven PWM.
            *   `digital-thermal-lcd` -> slug: `digital-thermal-lcd`. Desc: Python HID interface driving Thermalright LCD for real-time CPU/GPU metric visualization.
            *   `ai-model-selector-physical-controller` -> slug: `ai-model-selector-physical-controller`. Desc: ESP32 rotary controller navigating local models with OLED feedback and HID commands.

3.  **Drafting the Content (Iterative refinement for constraints):**

    *   *Header:* Standard align center, name, title.
    *   *Bio:* Needs to cover LLM inference, CUDA sm_61, automation.
        *   *Draft:* Researching optimized LLM inference (speculative decoding, EXL2 MoE routing). Building custom local AI infrastructure and CUDA compatibility layers for legacy compute (sm_61). Architecting embedded control systems for thermal management and hardware automation.
    *   *Stack Table:* Languages (C++, Python), Infra (FastAPI, Node, Flask), Hardware (ESP32, CUDA), AI (llama.cpp, ExLlamaV2).
    *   *Projects:*
        *   Format: `[name](url)`: Description.
    *   *Stats:* Standard GitHub images (Top langs, stats card).

4.  **Refining the Markdown & Slugs:**

    *   `automated-exl2-conversion-validation-pipeline` is long, fits the line length.
    *   `cuda-sm61-compatibility-shim`: `cuda-sm61-compatibility-shim`.
    *   `add-video-input-support-to-llamacpp-mtmd`: `add-video-input-support-to-llamacpp-mtmd`.

5.  **Writing the actual file (Mental check of lines):**

    *   The target is 90-120 lines. If I use 2 projects per section (8 total) + bio + header + table + padding, I need to be concise but descriptive.
    *   Let's ensure the specific details (Tesla P40, specific tools) are prominent.

6.  **Final Polish of Descriptions:**
    *   *Research:*
        *   `automated-exl2-conversion-validation-pipeline`: Fixes Qwen3_5 MoE arch, converts to EXL2, runs mixed-precision quantization benchmarks.
        *   `add-video-input-support-to-llamacpp-mtmd`: Adds video capture pipeline to llama.cpp via CMake and OpenCV for multimodal inference.
        *   `cuda-sm61-compatibility-shim`: Enables running modern CUDA code on unsupported Pascal GPUs (Tesla P40/sm_61).
    *   *Infra:*
        *   `start-llama`: Advanced launcher for `llama-server` with YAML preset management and port allocation.
        *   `llama-cpp-benchmark-suite`: Python/C++ suite measuring tok/s, TTFT, and VRAM footprint on consumer hardware.
    *   *Tools:*
        *   `ai-dashboard`: Flask dashboard aggregating GPU telemetry, system status, and sprint AGENDA integration.
        *   `megatool`: OSINT platform combining image analysis (Ollama/Qwen2.5VL), EXIF GPS parsing, and dark web crawling.
    *   *Embedded:*
        *   `controller-termico-proattivo-esp32`: ESP32 1-Wire thermal management system controlling Tesla P40 fan speeds via PWM.
        *   `digital-thermal-lcd`: HID driver for Thermalright LCD to visualize real-time thermal metrics on hardware.

7.  **Line Count Adjustment:**
    *   Need to ensure formatting (empty lines, headers) fits the 90-120 range.
    *   I will use standard markdown spacing.

8.  **Final Review against requirements:**
    *   English: Yes.
    *   Technical depth: Yes (MoE, sm_61, Tesla P40, EXL2).
    *   Structure: Head -> Bio -> Stack -> 4 Sections -> Stats.
    *   Max 2 emojis (Header): Yes.
    *   Slugs: Lowercase, hyphens.
    *   Output ONLY markdown.

**(Self-Correction during drafting)**: The prompt asks for "Show real technical depth: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing)...". The vault doesn't explicitly mention EAGLE or MTP in the project descriptions, but mentions "MoE routing" in the requirements (to be shown). I must infer or verify if I can include EAGLE/MTP. The vault mentions "35B locale", "Qwen3.5MoE", "EXL2". The prompt says "Show real technical depth... (EAGLE/MTP...)". It implies I should mention these concepts if relevant to the persona, but strictly use the vault data for projects. I will weave EAGLE/MTP into the *Bio* or *Technical focus* without inventing a project for them if they aren't in the vault, or attribute them to the *intent* of the research if implied. However, the prompt says "Use real technical details from the vault data below". The vault data *doesn't* mention EAGLE or MTP explicitly, but the prompt asks to "Show real technical depth: ... (EAGLE/MTP/speculative decoding/MoE routing)". I will prioritize the Vault data for the project descriptions but ensure the *Bio* reflects the prompt's required persona description of expertise in these areas (perhaps implied by the "LLM Research" section and the specific EXL2 work). Wait, looking closely at the prompt: "Show real technical depth: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing)". It lists specific topics. I should check if I can map these.
*   Vault: `automated-exl2-conversion-validation-pipeline` -> Qwen3_5Moe. (MoE is there).
*   Vault: `add-video-input-support-to-llamacpp-mtmd` -> llama.cpp (often supports spec decoding, mtmd might refer to Multi-Task Multi-Modal? Or just a branch name).
*   I will stick strictly to the vault content for the specific project descriptions to be accurate (as per "Use real technical details from the vault data"), but I will ensure the *Bio* establishes the expertise context requested.

Let's execute.

*   Bio line 1: Researching LLM inference optimization, including speculative decoding, MoE routing, and EXL2 quantization techniques.
*   Bio line 2: Architecting custom CUDA compatibility layers (sm_61) for deploying modern LLMs on legacy datacenter hardware (Tesla P40).
*   Bio line 3: Building self-hosted AI infrastructure, automated pipelines, and embedded control systems for hardware automation.

*   Stack Table:
    *   Languages: C ++, Python, JavaScript
    *   AI / ML: llama.cpp, ExLlamaV2, Ollama, ChromaDB
    *   Hardware: CUDA (sm_61), ESP32, 1-Wire, HID
    *   Systems: FastAPI, Flask, Node.js, systemd

*   Project sections and links.

*   Stats