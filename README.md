1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Subject:** Silvio Chessari.
    *   **Goal:** Generate a GitHub profile README.md.
    *   **Requirements:**
        *   Output ONLY the final README.md (no preamble/analysis).
        *   Style: English, technical, precise, no fluff.
        *   Focus areas: LLM inference (EAGLE/MTP/speculative decoding/MoE routing), running LLMs on unsupported GPUs (Tesla P40 sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.
        *   Data Source: provided "VAULT DATA" (Obsidian-like notes).
        *   Structure:
            *   Centered header.
            *   3-line technical bio.
            *   Compact stack table.
            *   4 project sections: LLM Research, AI Infrastructure, Tools & Automation, Embedded & Hardware.
            *   GitHub stats (at the end).
            *   Project format: `[name](https://github.com/chessarisilvio/slug)` + 1-line description.
            *   Repo slugs: lowercase, hyphens (derived from names).
            *   Max 2 emojis total (header only).
            *   Length: 90–120 lines.

2.  **Analyze the Vault Data (Information Extraction & Categorization):**

    *   *Bio/Hardware Context:*
        *   Hardware: Tesla P40 (sm_61), RTX 3050, Arduino R4 WiFi, ESP32.
        *   LLM Stack: llama.cpp, GGUF, EXL2, Ollama, CUDA, Whisper.
        *   Techniques: Speculative decoding (implied by research interests in "EAGLE/MTP" mentioned in requirements, though explicit mention in vault is limited to "mtmd" and video input), Quantization (Q4_K_M, Q5_K_S), MoE (Qwen 3.5 MoE), Multimodal (Video input).
        *   Languages: C++, Python, Node.js, HTML/CSS.

    *   *Projects Extraction & Mapping:*

        *   **LLM Research:**
            *   *Add video input support to llama.cpp (mtmd)* -> [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd): Extends llama.cpp CMake/Video stubs for multi-modal inference.
            *   *Automated EXL2 Conversion & Validation Pipeline* -> [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline): C++/Python toolchain for fixing Qwen3.5 MoE architecture, EXL2 quantization, and mixed precision benchmarking.
            *   *Sistema di Benchmarking Automatizzato per Nuovi Modelli GGUF* -> [automated-gguf-benchmarking-system](https://github.com/chessarisilvio/automated-gguf-benchmarking-system): Automated GGUF benchmarking on P40/RTX3050 with comparative reporting.

        *   **AI Infrastructure:**
            *   *Openclaw* -> [openclaw](https://github.com/chessarisilvio/openclaw): Node.js Ollama gateway acting as the central hub for local AI services.
            *   *AI Dashboard + Agenda* -> [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard): Local web dashboard on port 9190 monitoring GPU metrics, services, and managing AGENDA.md integration.
            *   *Automazione Boot/Watchdog AI Avanzato* -> [advanced-ai-boot-watchdog](https://github.com/chessarisilvio/advanced-ai-boot-watchdog): systemd watchdog monitoring llama-stack VRAM/tok/s with auto-recovery and Telegram notifications.

        *   **Tools & Automation:**
            *   *Megatool* -> [megatool](https://github.com/chessarisilvio/megatool): OSINT suite in C++ with Flask web interface for AI-assisted photo analysis.
            *   *Reddit Monitor* -> [reddit-monitor](https://github.com/chessarisilvio/reddit-monitor): Python script tracking AI/tech subreddits to feed AGENDA.md with ideas.
            *   *Bot Short* -> [bot-short](https://github.com/chessarisilvio/bot-short): C++ Telegram bot generating AI vector graphics and SVG assets.
            *   *Bias personalizzato per Whisper locale* -> [custom-whisper-bias](https://github.com/chessarisilvio/custom-whisper-bias): Bias injection module for Whisper with LLM-based context correction.

        *   **Embedded & Hardware:**
            *   *AI Home Assistant HID Dashboard* -> [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard): Arduino R4 WiFi dashboard for P40/3050 telemetry controlled via MQTT/Tailscale.
            *   *AI Model Selector Physical Controller* -> [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller): ESP32 rotary encoder interface with OLED display for selecting local LLMs via HID.
            *   *CUDA sm_61 Compatibility Shim* -> [cuda-sm61-compatibility-shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim): Software compatibility layer to enable modern CUDA stacks on legacy Pascal Tesla P40 GPUs.

3.  **Drafting the Content (Iterative refinement for Technical precision):**

    *   *Header:* `<p align="center">...</p>`
    *   *Bio:*
        *   Line 1: Focus on edge inference and hardware optimization.
        *   Line 2: Mention the specific GPU hack (P40/sm_61) and low-level CUDA work.
        *   Line 3: Mention the embedded/integration aspect (Arduino/MQTT).
    *   *Stack Table:*
        *   Columns: Domain, Technologies.
        *   Rows: Inference, Infrastructure, Embedded.
    *   *Sections:*
        *   *LLM Research:* Focus on video input, EXL2 MoE, and benchmarking.
        *   *AI Infrastructure:* Focus on the Gateway (Openclaw), Dashboard, and Watchdog.
        *   *Tools & Automation:* Focus on the bots (Telegram/Reddit), OSINT, and Whisper mods.
        *   *Embedded & Hardware:* Focus on Arduino/ESP32 projects interacting with the stack, plus the CUDA shim.
    *   *Formatting:* Use code blocks for the table, markdown links for projects. Ensure slugs are correct (lowercase, hyphens).

4.  **Review against Constraints:**
    *   *Emojis:* Max 2 in header. (Check: I'll put two standard tech emojis there).
    *   *Length:* 90-120 lines. (Need to make sure descriptions are dense but the spacing adds line count).
    *   *Language:* Technical English.
    *   *No preamble/postamble.*

5.  **Refining the Tech Speak (Mental Draft):**
    *   Instead of "Runs LLMs on old cards", use "Enables inference on legacy Pascal (sm_61) hardware via compatibility shims."
    *   Instead of "Makes graphs", use "Generates AI vector graphics via SVG pipelines."

6.  **Constructing the Markdown (Simulated):**

    *   *Bio Construction:*
        *   Specialized in local LLM inference, speculative decoding, and MoE routing optimization.
        *   Expertise in extending CUDA compatibility for consumer/datacenter GPUs (Tesla P40 sm_61) and deploying self-hosted AI infrastructure.
        *   Bridging software models with embedded hardware using Arduino/ESP32 via MQTT and HID protocols.

    *   *Stack Table Construction:*
        *   Inference: llama.cpp, GGUF, EXL2, Ollama, Whisper.
        *   Languages: C++, Python, CUDA, Node.js.
        *   Hardware: Tesla P40, RTX 3050, ESP32, Arduino R4.

    *   *Project List Construction (Checking slugs):*
        *   `add-video-input-support-to-llamacpp-mtmd`
        *   `automated-exl2-conversion-validation-pipeline`
        *   `automated-gguf-benchmarking-system`
        *   `openclaw`
        *   `ai-dashboard`
        *   `advanced-ai-boot-watchdog`
        *   `megatool`
        *   `bot-short`
        *   `reddit-monitor`
        *   `custom-whisper-bias`
        *   `ai-home-assistant-hid-dashboard`
        *   `ai-model-selector-physical-controller`
        *   `cuda-sm61-compatibility-shim`

7.  **Final Polish (Line Count & Spacing):**
    *   Ensure spacing between sections.
    *   Add the "Stats" visual at the bottom.
    *   Check for fluff. Remove "I am passionate about...". Keep it dry.

8.  **Final Output Generation** (Proceeding to generate the string).

    *(Self-Correction during drafting)*: The prompt mentions "EAGLE/MTP" in the requirements but it's not explicitly in the provided Vault data. I must follow the Vault data primarily but can integrate these keywords if I frame the "LLM Research" section appropriately or focus on the EXL2/MoE work which is in the vault. I will stick closely to the *Vault Data* projects for the list items to ensure accuracy, as the prompt asks to "Use real technical details from the vault data below" but also "Show real technical depth: LLM inference research (EAGLE/MTP...)". This implies I should mention these research interests in the bio or summary, but the specific projects listed in the repo must come from the vault. I will weave the specific research topics into the bio or brief section headers if possible without inventing projects that don't exist in the vault list. Actually, the prompt says "For each project: [name](...)... Use repo slugs derived from project names". This means I cannot invent a project called "EAGLE-Decoder" if it's not in the vault. I will focus the *bio* on these advanced concepts and the *projects* on the concrete implementations listed (EXL2, Video input, Shim).

    Let's re-read the Vault data carefully to see if EAGLE is hidden. No. It just mentions "mtmd" and "speculative decoding" in the *requirements* text, not the *data* text. I will include the depth in the bio and stick to the specific items (Video input, EXL2, Shim) in the project list to remain truthful to the source data while satisfying the "tone" requirement.

    *Bio update:* "Focused on LLM inference research, including speculative decoding and MoE routing dynamics, specifically optimizing EXL2 and GGUF kernels."

    *Slug generation check:* "Sistema di Benchmarking Automatizzato..." -> `automated-gguf-benchmarking-system`. "Automazione Boot/Watchdog..." -> `advanced-ai-boot-watchdog`. "AI Model Selector Physical Controller" -> `ai-model-selector-physical-controller`.

    *Stats section:* Standard GitHub stats markdown image URLs.

    *Line Count Strategy:*
    - Header + Bio: ~8 lines.
    - Stack: ~5 lines.
    - Section Headers: ~8 lines.
    - Projects: ~13 projects * 2 lines = 26 lines.
    - Stats/Footer: ~5 lines.