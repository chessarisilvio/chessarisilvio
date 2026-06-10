1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Subject:** Silvio Chessari.
    *   **Input:** Vault data describing various projects (LLM stack, embedded systems, research, tools).
    *   **Output Format:** `README.md` markdown only. No preamble/explanation.
    *   **Tone/Style:** English, technical, precise, no fluff. Show real technical depth.
    *   **Key Technical Themes:** LLM inference research (EAGLE, MTP, speculative decoding, MoE routing), unsupported GPUs (Tesla P40 sm_61, CUDA workarounds), AI infrastructure, embedded systems.
    *   **Structure:**
        *   Centered header.
        *   3-line technical bio.
        *   Compact stack table.
        *   4 Project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware).
        *   GitHub stats.
    *   **Project Format:** `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
    *   **Slug Format:** Lowercase, hyphens.
    *   **Length Constraint:** 90–120 lines.
    *   **Emoji Constraint:** Max 2, in header only.

2.  **Analyze the Vault Data (Information Extraction & Mapping):**

    *   *Bio Info:* Not explicitly provided as a bio, but inferred from projects. Focuses on LLM optimization, custom hardware integration (Tesla P40), and infrastructure.

    *   *Project Categories:*
        *   **LLM Research:**
            *   `cuda-sm61-compatibility-shim` (Running LLMs on unsupported Pascal GPUs).
            *   `gguf-per-cohere-30b-a3b-su-p40` (Specific focus on sm_61 optimization, offloading).
            *   `automated-exl2-conversion-validation-pipeline` (MoE quantization/conversion).
            *   `add-video-input-support-to-llamacpp-mtmd` (Multimodal expansion).
            *   `llm-inference-research` (Inferred from prompt mentioning EAGLE/MTP, though specific files in vault describe general stack).
        *   **AI Infrastructure:**
            *   `ai-dashboard` (Web monitoring at port 9190, AGENDA.md integration).
            *   `mtop` (h-top like for LLM inference).
            *   `open-source-mcp-bridge-for-local-claude-code` (Claude connectivity).
            *   `git-mcp-server-per-agenti-ai` (Git MCP).
            *   `openclaw` (Ollama gateway, Node.js).
        *   **Tools & Automation:**
            *   `megatool` (OSINT C++ + Flask web app).
            *   `reddit-monitor` (Subreddit monitoring -> AGENDA).
            *   `silvioprint` (Telegram bot content).
            *   `bot-short` (Telegram SVG).
            *   Note: `bot-short` and `megatool` are tools. `reddit-monitor` is automation.
        *   **Embedded & Hardware:**
            *   `controller-termico-proattivo-esp32` (Tesla P40 fan control, DS18B20, PWM).
            *   `digital-thermal-lcd` (Thermalright LCD HID).
            *   `ai-model-selector-physical-controller` (ESP32 model selector).
            *   `edge-vision-node-esp32-s3-moondream` (ESP32-S3 + moondream vision).
            *   `nllb-self-hosted-per-testo-multilingua` (OCR+MT pipeline).

3.  **Drafting Content - Step-by-Step:**

    *   **Header:** `Silvio Chessari` with emojis (limit 2).
    *   **Bio:** Needs to cover inference optimization (Pascal GPUs), MoE/Quantization, and custom infra/Embedded integration.
    *   **Stack Table:** Needs to be compact. Categories: Compute, Languages, Frameworks/Protocols, Hardware.
        *   *Compute:* CUDA (sm_61), EXL2, GGUF.
        *   *Languages:* C, C++, Python, ESP-IDF.
        *   *Frameworks:* llama.cpp, ExLlamaV2, ComfyUI, Node.js, Flask.
        *   *Hardware:* Tesla P40, ESP32/ESP32-S3, Sensors (DS18B20).

    *   **Section 1: LLM Research & Optimization**
        *   *Project:* `cuda-sm61-compatibility-shim` -> enabling Pascal (P40) for modern CUDA workflows.
        *   *Project:* `gguf-per-cohere-30b-a3b-su-p40` -> BeeLLama fork, sm_61 inference + embedding offload.
        *   *Project:* `automated-exl2-conversion-validation-pipeline` -> Qwen3.5 MoE architecture fix + quantization workflows.
        *   *Project:* `add-video-input-support-to-llamacpp-mtmd` -> llama.cpp video input integration (OpenCV).

    *   **Section 2: AI Infrastructure**
        *   *Project:* `open-source-mcp-bridge-for-local-claude-code` -> HTTP bridge for Claude Code MCP.
        *   *Project:* `git-mcp-server-per-agenti-ai` -> JSON API Git orchestration for agents.
        *   *Project:* `ai-dashboard` -> Local monitoring dashboard (GPU/Services) + AGENDA generation.
        *   *Project:* `mtop-htop-per-monitoraggio-llm-locale` -> Specialized process viewer for inference metrics.

    *   **Section 3: Tools & Automation**
        *   *Project:* `megatool` -> OSINT C++ engine + Flask analytics.
        *   *Project:* `reddit-monitor` -> AI/Tech subreddit scraping to AGENDA.md.
        *   *Project:* `bot-short` -> Telegram AI SVG generation pipeline.
        *   *Project:* `nllb-self-hosted-per-testo-multilingua` -> Offline NLLB-200 OCR + translation.

    *   **Section 4: Embedded & Hardware Integration**
        *   *Project:* `controller-termico-proattivo-esp32` -> Tesla P40 active thermal management (1-Wire/PWM).
        *   *Project:* `edge-vision-node-esp32-s3-moondream` -> ESP32-S3 moondream inference over Tailscale.
        *   *Project:* `ai-model-selector-physical-controller` -> Rotary encoder OLED HID selection.
        *   *Project:* `digital-thermal-lcd` -> USB HID display driver for Thermalright cooler.

    *   **GitHub Stats:** Standard placeholder `![github-stats](...)`.

4.  **Refining & Formatting:**
    *   *Check Line Count:* I need to keep it compact to hit 90-120 lines.
    *   *Check Slugs:* `cuda-sm61-compatibility-shim`, `gguf-per-cohere-30b-a3b-su-p40`, `automated-exl2-conversion-validation-pipeline`, `add-video-input-support-to-llamacpp-mtmd`, `open-source-mcp-bridge-for-local-claude-code`, `git-mcp-server-per-agenti-ai`, `ai-dashboard`, `mtop-htop-per-monitoraggio-llm-locale`, `megatool`, `reddit-monitor`, `bot-short`, `nllb-self-hosted-per-testo-multilingua`, `controller-termico-proattivo-esp32`, `edge-vision-node-esp32-s3-moondream`, `ai-model-selector-physical-controller`, `digital-thermal-lcd`.
    *   *Bio Draft:* Focused on LLM inference optimization, specifically porting stacks to legacy/architectures like Tesla P40 (sm_61), automated MoE quantization, and building self-hosted AI infrastructure with embedded hardware control interfaces.

5.  **Final Code Construction (Mental Sandbox):**

    *   *Header:*
        ```markdown
        <h1 align="center"> ⚡ Silvio Chessari 🛠️ </h1>
        ```
    *   *Bio:*
        ```markdown
        <p align="center">
        System Engineer focused on edge inference, speculative decoding, and legacy GPU optimization.
        Building self-hosted AI infrastructure, custom CUDA workarounds (sm_61), and integrated hardware control systems.
        </p>
        ```
    *   *Stack Table:* Use `markdown` table syntax.
    *   *Sections:* Use bold headers. Bullet points for projects. Ensure links look correct.

6.  **Reviewing against Constraints:**
    *   Output ONLY markdown? Yes.
    *   English? Yes.
    *   Structure correct? Yes.
    *   Max 2 emojis (header)? Yes.
    *   Line count check?
        *   Header/Bio: ~5 lines.
        *   Table: ~6 lines.
        *   4 Sections (~4 projects each): ~16 projects * 2 lines = 32 lines.
        *   Headers/Spacing: ~10 lines.
        *   Stats: ~2 lines.
        *   Total: < 60 lines currently. I need to flesh out descriptions or add structure to reach 90-120 lines without fluff. I will add a "Technical Focus" list or slightly more detailed descriptions (still 1 line but technical). Or perhaps add a small "Experience/Hardware" breakdown section. Let's stick to the structure requested but ensure the content is dense and spacing is clean.

    *   *Refining Descriptions for Technical Depth:*
        *   Instead of "Fan control," use "1-Wire sensor array + PWM MOSFET driver for Tesla P40 thermal management."
        *   Instead of "Runs on P40," use "Fork of llama.cpp optimized for Pascal architecture (sm_61) with embedding offload."

    *   *Re-calculating Lines:*
        *   Header/Bio: 5 lines.
        *   Stats (putting here or at bottom? Request says at bottom).
        *   Stack Table: 8 lines.
        *   Heading + 4 items * 4 sections: (1 header + 4 lines) * 4 = 20 lines.
        *   Vertical spacing: ~20 lines.
        *   Total is around 53 lines. Too short for 90-120.
    *   *Strategy Extension:* I will include a "Technical Scope" section between the Bio and the Stack. Or I will split the Projects into subsections within the 4 main categories or just ensure the list is populated with strictly technical items. Actually, the prompt asks for "Structure... -> 4 project sections". I will add a small "Hardware & Environment" context block or "Research Highlights" to fill the gap meaningfully without fluff.
    *   *Alternative:* Just spacing and perhaps standard badges for stats? No, badges are fluff. I will expand the Stack table to be very comprehensive (Compute, Languages, Frameworks, Embedded, Protocols). I will ensure the GitHub stats section and the footer take some space.
    *   *Better approach:* The prompt implies content density. Let's double the detail in the Bio (3 lines, I can make them longer/wrapped) and maybe add a "Core Competencies" small list or expand the "Stack" to be two columns or just very detailed rows.
    *   Let's stick to the prompt structure strictly but perhaps the prompt implies "90-120 lines *max*" or "target"? "90–120 lines total". This is