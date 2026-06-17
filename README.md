1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Subject:** Silvio Chessari (GitHub profile README).
    *   **Source Material:** "Vault data" (Obsidian-style markdown notes about projects, research, and infrastructure).
    *   **Tone:** English, technical, precise, professional, no fluff.
    *   **Structure Requirements:**
        *   Centered header.
        *   3-line technical bio.
        *   Compact stack table.
        *   4 Project sections: LLM Research, AI Infrastructure, Tools & Automation, Embedded & Hardware.
        *   GitHub stats (visual).
        *   Project format: `[Name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
        *   Slugs: lowercase, hyphens.
        *   Emojis: Max 2 total (header only).
        *   Length: 90-120 lines.
    *   **Specific Content to Highlight (from Vault):**
        *   LLM Inference Research: EAGLE, MTP, speculative decoding, MoE routing.
        *   Running LLMs on unsupported GPUs: Tesla P40 (sm_61), CUDA workarounds.
        *   AI Infrastructure: Self-built.
        *   Embedded Systems: Arduino, ESP32, MQTT, HID.

2.  **Process the Vault Data (Extraction & Categorization):**

    *   *LLM Research & Modifiers:*
        *   `add-video-input-support-to-llamacpp-mtmd`: Video input patches for llama.cpp (C++/Python).
        *   `nex2-mini-phase-twin-30b-lowvram-gguf-model`: Low-VRAM GGUF model optimization.
        *   `auto-quantization-pipeline-gguf`: Automated benchmarking/quantization on P40/RTX3050.
        *   `automated-exl2-conversion-validation-pipeline`: EXL2 conversion, Qwen3.5 MoE fix, mixed quantization.
        *   `bias-personalizzato-per-whisper-locale`: Contextual bias/post-correction for Whisper.

    *   *AI Infrastructure:*
        *   `ai-dashboard`: Web dashboard (9190) for GPU/services/agenda.
        *   `automazione-bootwatchdog-ai-avanzato`: Systemd watchdog for llama-stack, Telegram alerts.
        *   `secure-llm-context-vault`: Secure context storage.
        *   `openclaw`: Ollama gateway (Node.js).
        *   `launcher-avanzato-per-llama-server`: Advanced server launcher.

    *   *Tools & Automation:*
        *   `megatool`: OSINT C++ + Flask web app + AI photo analysis.
        *   `bot-short`: C++ Telegram bot, SVG/EPS graphics generation via AI.
        *   `reddit-monitor`: Subreddit AI scraper for ideas/agenda.
        *   `silvioprint`: Telegram content bot service.
        *   `silvioprint-sito-web`: Static HTML/CSS/JS e-commerce.

    *   *Embedded & Hardware:*
        *   `ai-home-assistant-hid-dashboard`: Arduino R4 WiFi + LCD + MQTT/Tailscale + ESP32 audio.
        *   `controller-termico-proattivo-esp32`: ESP32 proactive fan control + sensors.
        *   `digital-thermal-lcd`: HID temperature display (Thermalright).
        *   `ai-model-selector-physical-controller`: ESP32 rotary controller + OLED + HID for model selection.
        *   `cuda-sm61-compatibility-shim`: CUDA sm_61 shim for legacy P40 support.

3.  **Drafting Content - Section by Section:**

    *   **Header:**
        *   `# Silvio Chessari`
        *   Emojis: 🔬 ⚡
    *   **Bio:**
        *   Focus on specific tech: LLM inference optimization, CUDA hacking (sm_61), speculative decoding, MoE routing, local AI infrastructure, embedded hardware integration.
        *   *Drafting:* Specialized in LLM inference acceleration and speculative decoding techniques (EAGLE/MTP) on consumer and legacy datacenter hardware. Engineer building autonomous local AI infrastructure, featuring automated benchmarking pipelines and CUDA compatibility shims for Tesla P40 (sm_61) GPUs. Integrates embedded systems (Arduino/ESP32) with backend services for physical control of AI workloads and thermal management.
    *   **Stack Table:**
        *   Columns: Core, Inference, Hardware, Automation.
        *   *Drafting:*
            *   Core: C++, Python, Node.js, CUDA
            *   Inference: llama.cpp, Ollama, ExLlamaV2, GGUF
            *   Hardware: Tesla P40, RTX 3050,Arduino R4, ESP32
            *   Automation: Systemd, Docker, Telegram API, MQTT
    *   **Projects - Section 1: LLM Research & Optimization**
        *   *Select:* `nex2-mini-phase-twin-30b-lowvram-gguf-model`, `add-video-input-support-to-llamacpp-mtmd`, `automated-exl2-conversion-validation-pipeline`, `bias-personalizzato-per-whisper-locale`.
    *   **Projects - Section 2: AI Infrastructure**
        *   *Select:* `automazione-bootwatchdog-ai-avanzato`, `cuda-sm61-compatibility-shim`, `ai-dashboard`, `auto-quantization-pipeline-gguf`.
    *   **Projects - Section 3: Tools & Automation**
        *   *Select:* `bot-short`, `megatool`, `reddit-monitor`, `openclaw`.
    *   **Projects - Section 4: Embedded & Hardware**
        *   *Select:* `ai-home-assistant-hid-dashboard`, `ai-model-selector-physical-controller`, `controller-termico-proattivo-esp32`, `digital-thermal-lcd`.
    *   **GitHub Stats:**
        *   Standard `github-readme-stats` or `anuraghazra` cards.

4.  **Refining and Formatting (Checking Constraints):**

    *   *Slugs:* Ensure they are lowercase and hyphens (e.g., `add-video-input-support-to-llamacpp-mtmd`).
    *   *Line Count:* Need to aim for 90-120 lines. I need to ensure the descriptions are concise but the list is substantial.
    *   *Tone Check:* "English, technical, precise — no fluff."
    *   *Specific Tech Check:* Mentions of sm_61, CUDA, EAGLE, MoE, Tesla P40, RTX 3050.

5.  **Drafting the Markdown (Mental or Scratchpad):**

    *   *Bio Refinement:*
        Focus on LLM inference acceleration (EAGLE/MTP) and MoE routing on heterogeneous hardware (Tesla P40 sm_61/RTX 3050). Architect of self-hosted AI stacks using CUDA workarounds for legacy GPUs and automated quantization pipelines (GGUF/EXL2).
        (Too long? Let's trim).
        *Final Bio:*
        Researcher focusing on LLM inference acceleration via speculative decoding (EAGLE/MTP) and MoE routing optimization on heterogeneous hardware. Architect of self-hosted AI infrastructure, featuring CUDA compatibility shims for unsupported GPUs (sm_61) and automated quantization pipelines for low-VRAM environments. Integrates embedded microcontrollers (ESP32/Arduino) for physical control and thermal management of distributed compute nodes.

    *   *Formatting Links:*
        https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model
        https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd
        etc.

6.  **Final Code Assembly (Simulated):**

    *   Header
    *   Bio
    *   Tech Stack
    *   Headers for 4 sections
    *   Lists of links + desc
    *   Stats

    *Self-Correction during assembly:* The prompt asks for "Max 2 emojis total (header only)". I need to remove emojis from the project sections or the bio.

    *Reviewing Slugs:*
    - `nex2-mini-phase-twin-30b-lowvram-gguf-model`
    - `add-video-input-support-to-llamacpp-mtmd`
    - `automated-exl2-conversion-validation-pipeline`
    - `bias-personalizzato-per-whisper-locale`
    - `automazione-bootwatchdog-ai-avanzato`
    - `cuda-sm61-compatibility-shim`
    - `ai-dashboard`
    - `auto-quantization-pipeline-gguf`
    - `bot-short`
    - `megatool`
    - `reddit-monitor`
    - `openclaw`
    - `ai-home-assistant-hid-dashboard`
    - `ai-model-selector-physical-controller`
    - `controller-termico-proattivo-esp32`
    - `digital-thermal-lcd`

    *Reviewing Descriptions:* Needs to be punchy.
    - `nex2...`: Optimized 30B parameter model with phase-twin architecture for low-VRAM GGUF inference.
    - `add-video...`: CMake patch and Python/C++ stubs enabling raw video frame ingestion into llama.cpp backends.
    - `automated-exl2...`: C++/Python pipeline to fix Qwen3.5 MoE architectures and generate mixed-precision EXL2 checkpoints.

7.  **Final Polish:** Ensure line counts look right. The stack table takes up space, the project lists take up space.

    *Text for "Stack":*
    ```markdown
    ### Technical Skills
    | Architecture | Inference | Hardware | Automation |
    | :--- | :--- | :--- | :--- |
    | **C++, Python, CUDA** | **llama.cpp, ExLlamaV2** | **Tesla P40 (sm_61), RTX 3050** | **Systemd, Docker, Tailscale** |
    | Node.js, Bash | GGUF, EXL2 | Arduino R4, ESP32 | MQTT, Telegram API |
    ```

    *Text for Stats:*
    ```markdown
    ![GitHub Stats](https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&hide_border=true&rank_icon=github)
    ```

8.  **Final Output Generation** (Proceeding to generate the markdown block).

    *Check:* Did I include *real technical depth*? Yes (sm_61, EAGLE, MTP, MoE).
    *Check:* Is it English? Yes.
    *Check:* Is it only the markdown? Yes.

    (Self-Correction on Slugs based on "real technical details from the vault"): The vault path uses underscores `add-video-input-support-to-llamacpp-mtmd`, the user prompt says "use repo slugs derived from project names (lowercase, hyphens)". I will adhere to the prompt's instruction for the GitHub slug format (lowercase, hyphens) but keep the name recognizable. E.g., `ai-home-assistant-hid-dashboard`.

    Let's double check the line count target. 16 projects x ~2 lines = 32 lines. Bio = 5 lines. Stack = 4 lines. Headers = 4 lines. Preamble/Stats = 10 lines. Total ~55. I need to expand descriptions slightly or ensure spacing is correct to