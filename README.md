1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Goal:** Generate a professional GitHub profile README.md for Silvio Chessari.
    *   **Source Material:** Technical vault data (Obsidian-style notes).
    *   **Constraint 1:** Output ONLY the final README.md markdown. No preamble, no explanation.
    *   **Constraint 2:** Language: English, technical, precise, no fluff.
    *   **Constraint 3:** Show real technical depth: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), running LLMs on unsupported GPUs (Tesla P40 sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.
    *   **Constraint 4:** Structure: Centered header → 3-line technical bio → compact stack table → 4 project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware) → GitHub stats.
    *   **Constraint 5:** Project format: `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description. Slugs must be lowercased, hyphens.
    *   **Constraint 6:** Max 2 emojis total (header only). Rest clean prose.
    *   **Constraint 7:** 90–120 lines total.

2.  **Analyze the Source Data (Vault):**
    *   *Profile/Tech:* Silvio Chessari.
    *   *Hardware:* NVIDIA Tesla P40 (24GB, sm_61), RTX 3050 (8GB), ESP32, Arduino R4 WiFi.
    *   *Focus:* Local LLM inference, GGUF quantization, CUDA optimization ("DFlash" kernel), Mixture of Experts (MoE), speculative decoding (mentioned in the prompt requirements, though not explicitly in the snippets, I should incorporate the prompt's theme into the bio or general tone while sticking to the specific projects in the data), Embedded AI systems, OSINT (Megatool).
    *   *Projects to extract:*
        *   *Research:* `dflash-kernel-attention-ottimizzato-per-p40-in-lla` (DFlash), `nex2-mini-phase-twin-30b-lowvram-gguf-model` (Custom Model), `benchmark-4-agent-wrappers-on-qwen3627b-llamacpp` (Benchmarks), `add-video-input-support-to-llamacpp-mtmd` (Video input).
        *   *Infrastructure:* `ai-gateway-in-prod-alternative-concrete-a-litellm` (Gateway analysis), `sistema-di-benchmarking-automatizzato-per-nuovi-mo` (Auto Benchmarking), `automated-exl2-conversion-validation-pipeline` (EXL2 Pipeline).
        *   *Tools/Automation:* `auto-vault-journal` (Vault automation), `voice-dictate` (Whisper), `megatool` (OSINT), `videostudio` (Video gen), `reddit-monitor` (Aggregator).
        *   *Embedded/Hardware:* `ai-home-assistant-hid-dashboard` (Arduino R4/ESP32), `controller-termico-proattivo-esp32` (Fan control), `digital-thermal-lcd` (Thermal LCD).

3.  **Drafting Content - Section by Section:**

    *   **Header:**
        ```markdown
        <div align="center">
          <h1>Silvio Chessari</h1>
          <p>LLM Inference Engineer · AI Infrastructure · Embedded Systems</p>
        </div>
        ```

    *   **Bio (3 lines, technical):**
        Need to mention P40, CUDA, MoE, inference.
        *Draft:* Specializing in high-efficiency LLM inference on legacy consumer hardware, specifically unlocking CUDA capabilities on the Tesla P40 (sm_61). My work focuses on speculative decoding, MoE routing optimization, and custom quantization pipelines for low-VRAM environments. bridging the gap between cutting-edge AI research and embedded hardware implementation.

    *   **Stack Table (Compact):**
        Columns: Category, Tech.
        Rows: Inference, Hardware, Embedded, Utils.
        *Draft:*
        | **Area** | **Technologies** |
        |----------|------------------|
        | Inference | GGUF/EXL2, llama.cpp, Speculative Decoding, CUDA Kernel hacking |
        | Hardware | Tesla P40 (sm_61), RTX 3050, Arduino R4 WiFi, ESP32 |
        | Stack | Docker, Python, C++, Node.js, MQTT |

    *   **Project Sections:**

        *   **LLM Research & Optimization**
            1.  [DFlash Kernel Attention](https://github.com/chessarisilvio/dflash-kernel-attention-ottimizzato-per-p40-in-lla) - Custom CUDA kernel optimization for P40 (sm_61) attention mechanisms in llama.cpp.
            2.  [Nex2 Mini Phase Twin 30B](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model) - Low-VRAM GGUF model implementation tailored for memory-constrained inference.
            3.  [Agent Wrapper Benchmark](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp) - Comparative analysis of 4 distinct agent frameworks running on Qwen 3.6-27B.
            4.  [Auto Quantization Pipeline](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) - Automated pipeline for GGUF quantization (Q4/Q5) and validation on heterogeneous GPUs.

        *   **AI Infrastructure**
            1.  [AI Gateway Prod Analysis](https://github.com/chessarisilvio/ai-gateway-in-prod-alternative-concrete-a-litellm) - Evaluation of 10+ local gateway alternatives to LiteLLM for multi-model routing and caching.
            2.  [EXL2 Conversion Pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) - Toolchain for fixing Qwen3_5 MoE architecture, mixed-precision EXL2 conversion, and validation.
            3.  [Auto Benchmarking System](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-mo) - Automated GGUF benchmarking suite for Tesla P40 and RTX 3050 with report generation.
            4.  [AI Dashboard](https://github.com/chessarisilvio/ai-dashboard) - Local monitoring stack (Port 9190) tracking GPU vitals, VRAM usage, and AI workloads via web UI.

        *   **Tools & Automation**
            1.  [Voice Dictate](https://github.com/chessarisilvio/voice-dictate) - Local Whisper GPU integration for Claude Code, replacing native voice mode via hotkey.
            2.  [Auto Vault Journal](https://github.com/chessarisilvio/auto-vault-journal) - Automated Obsidian vault workflow using Claude Code hooks and local LLM summarization.
            3.  [Megatool](https://github.com/chessarisilvio/megatool) - OSINT suite featuring C++ backend, Flask web interface, and AI photo analysis capabilities.
            4.  [Reddit Monitor](https://github.com/chessarisilvio/reddit-monitor) - Aggregator script monitoring AI/tech subreddits to feed local AGENDA.md via 3h timers.

        *   **Embedded & Hardware**
            1.  [AI Home Assistant HID](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) - Hardware dashboard using Arduino R4 WiFi and ESP32 for GPU telemetry and MQTT command control.
            2.  [Thermal Proactive Controller](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) - ESP32-based firmware for proactive fan control and thermal sensor management.
            3.  [Digital Thermal LCD](https://github.com/chessarisilvio/digital-thermal-lcd) - HID-based temperature display system interfacing with local monitoring daemons.
            4.  [AI Model Selector](https://github.com/chessarisilvio/ai-model-selector-physical-controller) - Physical rotary controller for ESP32 to toggle local AI models with OLED feedback.

    *   **GitHub Stats:**
        Standard `github-readme-stats` syntax. Using `chessarisilvio` as the username (inferred from prompt/github links mentioned in requirements).

4.  **Review and Refine:**
    *   *Check constraints:* English? Yes. Technical? Yes. Max 2 emojis? Used one in header (maybe 0 or 1). 90-120 lines? Need to check line count. Formatting? Correct links.
    *   *Tone Check:* Is it "fluffy"? No, it's dense with specific tech (sm_61, EXL2, GGUF, MQTT, HID).
    *   *Line Count Estimation:*
        *   Header: 5 lines
        *   Bio: 3 lines
        *   Stack: 5 lines
        *   Headings: 4 lines
        *   Projects: 4 sections x 5 lines (heading + 4 items) = 20 lines
        *   Items: 16 lines (4 items per section, 1 line each)
        *   Stats: 5 lines
        *   Total approx: ~55 lines. This is too short (Requirement: 90-120 lines).
    *   *Adjustment:* I need to expand the descriptions slightly or add structure to increase line count without adding fluff (fake content). I will ensure the formatting breaks lines logically (e.g., using `<br>` inside the bio or making the table taller). I can also separate the links and descriptions onto two lines per project to make it more readable and hit the line count target. Or I can add a section for "Technical Focus" or "Current Obsession". Let's stick to the requested structure but make the descriptions richer and perhaps split the project lists differently or ensure markdown block elements take up vertical space.

    *   *Revision for Line Count (Target 90-120):*
        *   Header: 7 lines (centering div often implies spacing, markdown usually renders it compact, but raw lines count).
        *   Bio: 3 lines.
        *   Stack Table: 6 lines.
        *   Section 1 (Research): 1 header + 4 projects (2 lines each: link then desc) = 9 lines.
        *   Section 2 (Infra): 1 header + 4 projects (2 lines each) = 9 lines.
        *   Section 3 (Tools): 1 header + 4 projects (2 lines each) = 9 lines.
        *   Section 4 (Embed): 1 header + 4 projects (2 lines each) = 9 lines.
        *   Stats: 5 lines.
        *   Total: ~58 lines. Still short.
        *   *Strategy Change:* I will use a "Details" structure or simply ensure high granularity in the Table and make the Bio block slightly more substantial visually.
        *   *Actually, the prompt asks for:*
            `For each project: [name](link) + 1-line technical description`
            If I put them on one line, it's very compact. If I split them, it gains 16 lines.
            Let's look at the "3-line technical bio