1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Subject:** Silvio Chessari.
    *   **Source Material:** Technical vault data (Obsidian notes).
    *   **Requirements:**
        *   Output ONLY the README.md markdown file.
        *   No preamble, no explanation.
        *   Language: English, technical, precise, no fluff.
        *   Depth: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), running LLMs on unsupported GPUs (Tesla P40 sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.
        *   Structure: centered header -> 3-line technical bio -> compact stack table -> 4 project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware) -> GitHub stats.
        *   Project format: `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
        *   Repo slugs: derived from project names (lowercase, hyphens).
        *   Emojis: Max 2 total (header only).
        *   Length: 90–120 lines total.

2.  **Analyze the Source Data (Vault):**
    *   *Projects found:*
        *   *LLM Research:* Add video input support to llama.cpp (mtmd), Automated EXL2 Conversion & Validation Pipeline (Qwen3_5MoeForC fix, mixed quantization), Cuda sm61 Compatibility Shim (Tesla P40), Auto-Quantization Pipeline GGUF, Qwen Image Edit Inpainting Workflow.
        *   *AI Infrastructure:* AI Dashboard & Agenda, Automazione Boot/Watchdog AI Avanzato (llama-stack monitoring), Openclaw (Ollama gateway), Launcher avanzato per llama-server, Auto-quantization pipeline.
        *   *Tools & Automation:* Megatool (OSINT C++, Flask), bot-short (Telegram, AI SVG), Reddit Monitor, Silvioprint, Git MCP Server for AI Agents, mtop (htop-like for LLM), NLLB Self-Hosted, Open-source MCP bridge for local Claude Code.
        *   *Embedded & Hardware:* Controller Termico ESP32 (Tesla P40 Fan Control), digital-thermal-lcd (Thermalright display), AI Model Selector Physical Controller (ESP32, rotary, OLED), Edge Vision Node ESP32-S3 + moondream.

3.  **Drafting - Section by Section:**

    *   **Header:** Centered, name, title, max 2 emojis.
        *   *Draft:*
            ```markdown
            # <div align="center">Silvio Chessari</div>
            <div align="center">
            <b>AI Infrastructure Engineer</b> • <b>LLM Inference Researcher</b>
            </div>
            <div align="center">
            <img src="https://img.shields.io/badge/CUDA-11.x-black?style=flat&logo=nvidia" alt="CUDA">
            <img src="https://img.shields.io/badge/C++-00599C?style=flat&logo=c%2B%2B" alt="C++">
            <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python" alt="Python">
            <img src="https://img.shields.io/badge/Embedded_ESP32-E7352C?style=flat&logo=espressif" alt="ESP32">
            ```

    *   **Bio:** 3 lines, technical depth.
        *   *Keywords:* LLM inference, Tesla P40 (sm_61), CUDA workarounds, EAGLE/MTP, MoE, Embedded systems.
        *   *Draft:*
            Specializing in local LLM inference optimization and speculative decoding research (EAGLE/MTP). Expert at deploying large models on legacy hardware, including custom CUDA shims for Tesla P40 (sm_61) compatibility. Full-stack engineer bridging high-performance AI infrastructure with embedded automation systems.

    *   **Stack Table:** Compact.
        *   *Draft:*
            | Area | Technologies |
            | :--- | :--- |
            | **Inference** | llama.cpp, EXL2, vLLM, Speculative Decoding, MoE Routing |
            | **Infrastructure** | CUDA, Docker, Nginx, Systemd, Flask, Node.js |
            | **Embedded** | ESP32/ESP32-S3, C++, HID, 1-Wire, PWM, SSD1306 |
            | **Research** | Quantization (GGUF/EXL2), VRAM Management, Benchmarks |

    *   **Project Sections:**
        *   *Constraints:* 4 specific sections, `[name](url)` format, slug derivation.

        *   **1. LLM Research**
            *   *Project:* Automated EXL2 Conversion & Validation Pipeline -> `automated-exl2-conversion-validation-pipeline`
            *   *Project:* Add video input support to llama.cpp (mtmd) -> `add-video-input-support-to-llamacpp-mtmd`
            *   *Project:* CUDA sm_61 Compatibility Shim -> `cuda-sm61-compatibility-shim`
            *   *Project:* Auto-Quantization Pipeline GGUF -> `auto-quantization-pipeline-gguf`
            *   *Project:* Qwen Image Edit Inpainting Workflow -> `qwen-image-edit-inpainting-workflow`

        *   **2. AI Infrastructure**
            *   *Project:* AI Dashboard & Agenda -> `ai-dashboard`
            *   *Project:* Automazione Boot/Watchdog AI Avanzato -> `automazione-bootwatchdog-ai-avanzato`
            *   *Project:* Openclaw -> `openclaw`
            *   *Project:* Launcher avanzato per llama-server -> `launcher-avanzato-per-llama-server`
            *   *Project:* NLLB Self-Hosted per Testo Multilingua -> `nllb-self-hosted-per-testo-multilingua`

        *   **3. Tools & Automation**
            *   *Project:* bot-short -> `bot-short`
            *   *Project:* Megatool -> `megatool`
            *   *Project:* Reddit Monitor -> `reddit-monitor`
            *   *Project:* mtop: htop per monitoraggio LLM locale -> `mtop-htop-per-monitoraggio-llm-locale`
            *   *Project:* Git MCP Server for AI Agents -> `git-mcp-server-per-agenti-ai`
            *   *Project:* Open-source MCP bridge for local Claude Code -> `open-source-mcp-bridge-for-local-claude-code`
            *   *Project:* Silvioprint -> `silvioprint`

        *   **4. Embedded & Hardware**
            *   *Project:* Controller Termico ESP32 -> `controller-termico-proattivo-esp32`
            *   *Project:* AI Model Selector Physical Controller -> `ai-model-selector-physical-controller`
            *   *Project:* Digital Thermal LCD -> `digital-thermal-lcd`
            *   *Project:* Edge Vision Node ESP32-S3 + moondream -> `edge-vision-node-esp32-s3-moondream`

    *   **GitHub Stats:**
        *   *Draft:* Standard GitHub stats image or simple markdown. Since specific images aren't provided, I will use generic placeholders or standard stats URLs.

4.  **Refining and Formatting (Self-Correction):**
    *   *Constraint Check:* Max 2 emojis used? Yes, in header (actually badges aren't emojis, but I'll keep it clean). I will put emojis in the headers of the sections? No, requirement says "Max 2 emojis total (header only), rest is clean technical prose". Okay, I will use badges in the header and maybe 2 small emojis there if needed, but the prompt asks for emojis in the *header only*. I'll stick to standard badges.
    *   *Line Count Check:* I need 90-120 lines. I need to expand the descriptions slightly or use lists to ensure the length is sufficient without fluff. The list of projects is quite long, which helps.
    *   *Slug Generation:*
        *   `add-video-input-support-to-llamacpp-mtmd`
        *   `automated-exl2-conversion-validation-pipeline`
        *   `automazione-bootwatchdog-ai-avanzato`
        *   `controller-termico-proattivo-esp32`
        *   `mtop-htop-per-monitoraggio-llm-locale`
        *   `open-source-mcp-bridge-for-local-claude-code`
    *   *Tech Details:* Ensure "Tesla P40", "sm_61", "EXL2", "MoE", "speculative decoding" are mentioned in the bio or project descriptions.

5.  **Final Polish of the Markdown:**

    *   *Bio:* Specialized in LLM inference optimization via speculative decoding (EAGLE/MTP) and MoE routing. Developing custom CUDA shims to enable LLM deployment on unsupported legacy hardware (NVIDIA Tesla P40, sm_61). architecting self-hosted AI stacks and embedded control systems for edge automation.
    *   *Stack:* Group Inference, Infra, Embedded, Research.
    *   *Sections:* Ensure clear headers.

    *(Self-Correction during drafting project descriptions)*
    - `automated-exl2-conversion-validation-pipeline`: Fixes Qwen3_5MoeForC architecture, converts to EXL2, applies mixed quantization, and generates validation benchmarks.
    - `cuda-sm61-compatibility-shim`: Overrides GPU architecture checks to allow vLLM and PyTorch execution on Pascal-based GPUs like the Tesla P40.
    - `mtop-htop-per-monitoraggio-llm-locale`: htop-inspired CLI tool for real-time monitoring of local LLM inference metrics, including GPU load and token throughput.
    - `controller-termico-proattivo-esp32`: ESP32-based firmware providing proactive thermal regulation for Tesla P40 fans via 1-Wire sensors and PWM driver to prevent throttling.

6.  **Final Line Count Estimation:**
    *   Header: ~10 lines
    *   Bio: ~4 lines
    *   Stack: ~5 lines
    *   Projects (approx 5-6 per section * 6 lines spacing): ~30-40 lines
    *   Stats: ~5 lines
    *   Footer: ~2 lines
    *   Total might be around 70. I need to ensure the project descriptions are rich with technical details from the vault to reach 90+ lines. I will make sure the stack table uses bullet points or more rows to add substance, and the project descriptions are concise but packed. I will ensure the formatting (spacing) aligns with the 90-120 range.

    *Let's review the Vault data again for specifics to plump up descriptions.*
    - *Qwen Image Edit:* ComfyUI workflow.
    - *Openclaw:* Ollama Gateway.
    - *Megatool:* OSINT C++, Flask `:7788`, photo analysis.
    - *Reddit Monitor:* Timer 3h, AGENDA.md integration.
    - *Silvioprint:* systemd service, Telegram content.

7.  **Final Output Generation** (Proceeding to generate markdown).

    *Check Constraint:* "Output ONLY the final README.md markdown".
    *Check Constraint:* "English, technical, precise".

    Let's write.

    (Drafting content...)
    Header...
    Bio...
    Table...
    ### LLM