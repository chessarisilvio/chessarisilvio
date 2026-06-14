1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Target Audience:** GitHub users, technical recruiters, peers.
    *   **Subject:** Silvio Chessari.
    *   **Input:** "Technical Vault Data" (Obsidian-style notes in Italian).
    *   **Constraints:**
        *   Output ONLY the final README.md markdown.
        *   No preamble, no explanation.
        *   Language: English, technical, precise, no fluff.
        *   Focus on: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), running LLMs on unsupported GPUs (Tesla P40 sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.
        *   Structure: Centered header -> 3-line technical bio -> Compact stack table -> 4 project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware) -> GitHub stats.
        *   Project Format: `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
        *   Slugs: Lowercase, hyphens.
        *   Emojis: Max 2 total (header only).
        *   Length: 90–120 lines total.

2.  **Extract & Translate Key Data (from Italian vault):**

    *   *Bio Concept:* LLM inference researcher specializing in speculative decoding and MTP; self-hosted AI infrastructure on legacy hardware (Tesla P40); embedded systems integration.

    *   *Projects Mapping:*

        *   *Category: LLM Research / Core Engine Modifications*
            *   `add-video-input-support-to-llamacpp-mtmd`: Add video input support to llama.cpp (mtmd). Needs video frame capture & inference.
            *   `automated-exl2-conversion-validation-pipeline`: Fix Qwen3_5 MoE arch, convert to EXL2, mixed quantization benchmarking.

        *   *Category: AI Infrastructure / Hardware Optimization*
            *   `auto-quantization-pipeline-gguf`: Automated GGUF quantization, benchmarking local hardware (P40, RTX 3050), auto-reporting.
            *   `cuda-sm61-compatibility-shim`: CUDA sm_61 compatibility shim for Pascal GPUs (Tesla P40). This is huge (running on unsupported hardware).
            *   `nllb-self-hosted-per-testo-multilingua`: Offline NLLB-200 translation, OCR+MT pipeline.
            *   `mtop-htop-per-monitoraggio-llm-locale`: `mtop`: htop-like real-time inference monitor (GPU, tokens/s).

        *   *Category: Tools & Automation*
            *   `ai-dashboard`: Web dashboard (port 9190) for GPU/services/agenda, local LLM idea generation.
            *   `automazione-bootwatchdog-ai-avanzato`: Advanced watchdog for llama-stack, monitors VRAM/tok/s, Telegram alerts, systemd integration.
            *   `bot-short`: Telegram C++ bot generating AI vector graphics (SVG pipeline).
            *   `git-mcp-server-per-agenti-ai`: Git MCP Server for AI agents. (Implied from "Sviluppati" list, need to infer technical description).

        *   *Category: Embedded & Hardware*
            *   `ai-home-assistant-hid-dashboard`: Arduino R4 WiFi + LCD dashboard for local AI status, MQTT/Tailscale integration.
            *   `ai-model-selector-physical-controller`: ESP32 + Rotary encoder for local model selection, HID input, OLED display.
            *   `controller-termico-proattivo-esp32`: Proactive fan control + sensors on ESP32.
            *   `digital-thermal-lcd`: LCD temperature display via HID.

3.  **Refine & Select Projects (fitting the constraints):**
    I need to select projects that demonstrate the "real technical depth" requested (inference research, unsupported GPUs, embedded).

    *   *LLM Research:*
        1.  `add-video-input-support-to-llamacpp-mtmd` (multimodal integration)
        2.  `automated-exl2-conversion-validation-pipeline` (MoE quantization/exl2)

    *   *AI Infrastructure:*
        1.  `cuda-sm61-compatibility-shim` (The Tesla P40 unsupported GPU story)
        2.  `auto-quantization-pipeline-gguf` (Benchmarking pipeline)

    *   *Tools & Automation:*
        1.  `mtop-htop-per-monitoraggio-llm-locale` (Real-time metrics)
        2.  `automazione-bootwatchdog-ai-avanzato` (Process monitoring/Telegrams)

    *   *Embedded & Hardware:*
        1.  `ai-home-assistant-hid-dashboard` (R4 + MQTT)
        2.  `ai-model-selector-physical-controller` (ESP32 + Model selection)

4.  **Drafting Content (Iterative refinement for tone):**

    *   *Header:* simple, centering.
    *   *Bio:*
        Specializing in LLM inference optimization and speculative decoding research (MTP/EAGLE) on legacy datacenter hardware. Experienced in building self-hosted AI infrastructure, CUDA shims for unsupported GPUs, and robust embedded automation systems. Bridging the gap between theoretical inference gains and practical deployment on consumer and edge devices.

    *   *Stack Table:* Needs to be compact.
        *   LLMs: llama.cpp, EXL2, GGUF
        *   Infra: Docker, Tailscale, MQTT, systemd
        *   Hardware: Tesla P40 (sm_61), ESP32, Arduino R4
        *   Lang: C++, Python, Bash

    *   *Drafting Project Descriptions (Technical & Precise):*
        *   *Add Video Input:* Extends llama.cpp to accept video frames via OpenCV stubs, enabling multimodal inference pipelines directly in C++.
        *   *Automated EXL2 Pipeline:* Fixes Qwen 3.5 MoE architectures and automates EXL2 quantization with mixed precision and validation benchmarks.
        *   *CUDA sm_61 Shim:* Implements compatibility layer to run modern LLM inference stacks on NVIDIA Tesla P40 (Pascal architecture/sm_61).
        *   *Auto Quantization:* Orchestrates GGUF conversion and benchmarking on heterogeneous hardware (RTX 3050 / P40) to determine optimal quantization points.
        *   *Mtop:* htop-inspired CLI tool providing real-time monitoring of GPU VRAM, utilization, and token generation speed for local inference.
        *   *Boot Watchdog:* Systemd-integrated watchdog for llama-stack monitoring process health, VRAM leaks, and throughput metrics with Telegram alerting.
        *   *AI Home Assistant:* Physical dashboard built on Arduino R4 WiFi exposing local GPU status and model metrics via MQTT and Tailscale.
        *   *Model Selector:* Embedded ESP32 controller using rotary encoders and HID emulation to switch active LLM models on the host machine.

5.  **Formatting & Sizing:**
    *   Check line count. Needs to be 90-120 lines.
    *   Ensure "Center alignment" (HTML tags or standard markdown alignment hacks). Usually plain markdown doesn't center strictly without HTML. I will use `<div align="center">`.
    *   Check slugs: `add-video-input-support-to-llamacpp-mtmd`, `automated-exl2-conversion-validation-pipeline`, `cuda-sm61-compatibility-shim`, `auto-quantization-pipeline-gguf`, `mtop-htop-per-monitoraggio-llm-locale`, `automazione-bootwatchdog-ai-avanzato`, `ai-home-assistant-hid-dashboard`, `ai-model-selector-physical-controller`.

6.  **Final Polish (Self-Correction during drafting):**
    *   *Critique:* The bio needs to be punchy. "LLM inference researcher..." is good.
    *   *Critique:* Make sure the Tesla P40 sm_61 and CUDA workarounds are highlighted.
    *   *Critique:* Check emoji limit. Only in header. "⚙️ 🚀" or similar.
    *   *Critique:* Verify project links match the requested format.

7.  **Generating the Markdown (Mental Draft to Final):**

    *   *Header:* Silvio Chessari, Technical details.
    *   *Bio:* 3 lines.
    *   *Stack:* Columns.
    *   *Sections:* Headers, projects with links.
    *   *Stats:* Standard `pics` or `stats` image placeholders.

    *(Self-Correction on specific data points)*:
    - "EAGLE/MTP" mentioned in requirements -> Not explicitly in the vault data provided *in detail*, but the prompt says "Show real technical depth: LLM inference research (EAGLE/MTP...)". I will weave this into the bio and perhaps a relevant project note if possible, or keep it in the bio since the vault data supports "Inference" and "Benchmarking" and "speculative decoding" context is implied by "mtmd" (Multimodal Token Mediated Decoding? or similar). Wait, `mtmd` in the filename `add-video-input-support-to-llamacpp-mtmd` likely refers to the specific fork or patch. The prompt *requires* me to mention EAGLE/MTP/speculative decoding. I will put this in the bio to establish the persona based on the prompt instructions, even if specific project notes are brief.
    - "Tesla P40 sm_61" -> definitely in `cuda-sm61-compatibility-shim` and `auto-quantization-pipeline-gguf`.

    Let's assemble.

    *Lines estimation:*
    Header: 5
    Bio: 5
    Stack: 10
    Section 1: 10
    Section 2: 10
    Section 3: 10
    Section 4: 10
    Stats: 5
    Footer: 2
    Total: ~65-70. Need to expand slightly with details or spacing to hit 90-120 range without fluff. I will use comments or slightly more detailed technical descriptions. Actually, the prompt asks for "compact stack table" and "1-line technical description".
    To hit the line count with strict "no fluff", I might need to add a specific "Methodology" or "Focus" section, or just ensure the markdown structure (spacing/badges) fills it out reasonably. However, the requirements are strict on structure:
    "Structure: centered header → 3-line technical bio → compact stack table → 4 project sections → GitHub stats".
    I can make the bio rich, the stack detailed, and the project descriptions dense.

    *Refined Plan for Line Count:*
    - Bio: 3 dense lines.
    - Stack: Technical categories (Inference, Edge, DevOps).
    - Project sections: I will add a small sub-header description for the *category* if space permits, or just keep it tight. Let's stick to the requested structure: header, bio, stack, sections, stats.
    - I will use technical badges (shields.io) to bulk up the visual density and line count without adding "fluff" text. This is standard technical writing.

    *Wait, prompt says:* "Max 2 emojis total (header only)". I cannot use emojis in badges.
    I will use text-based categorization in the stack table.

    Let's write it out.

    *Bio Draft:*
    Focused on LLM inference optimization, speculative decoding (EAGLE/MTP), and quantization strategies for mixed-M