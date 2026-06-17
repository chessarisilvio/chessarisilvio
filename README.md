1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Target:** GitHub Profile README.md for Silvio Chessari.
    *   **Source Material:** Provided "vault data" (Italian text describing projects, paths, and notes).
    *   **Tone/Style:** Professional, English, technical, precise, no fluff, max 2 emojis (header only).
    *   **Length:** 90–120 lines.
    *   **Structure:**
        *   Centered header.
        *   3-line technical bio.
        *   Compact stack table.
        *   4 project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware).
        *   GitHub stats.
    *   **Project Format:** `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.
    *   **Specific Content Requirements:** Focus on LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), running LLMs on unsupported consumer/datacenter GPUs (Tesla P40 sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.

2.  **Analyze the Source Data (Vault):**
    *   *Overview/Hardware:* Tesla P40 (sm_61), RTX 3050, Arduino R4 WiFi, ESP32.
    *   *LLM Research/Inference:*
        *   "Nex2 Mini Phase Twin 30B low‑VRAM GGUF model": Suggests model merging/creation for low VRAM.
        *   "auto-quantization-pipeline-gguf": Benchmarking GGUF on P40/3050, auto-selecting Q4_K_M vs Q5_K_S.
        *   "automated-exl2-conversion-validation-pipeline": Qwen3_5Moe fix, EXL2 conversion, mixed quantization.
        *   "add-video-input-support-to-llamacpp-mtmd": Adding video input to llama.cpp.
        *   "bias-personalizzato-per-whisper-locale": Whisper bias correction via local LLM.
    *   *AI Infrastructure/Tools:*
        *   "ai-dashboard": Local monitoring (:9190), AGENDA.md integration, worker sub-tasks.
        *   "automazione-bootwatchdog-ai-avanzato": Watchdog for `llama-stack`, VRAM monitoring, Telegram notifications, systemd restarts.
        *   "openclaw": Ollama Gateway, Node.js.
        *   "secure-llm-context-vault": Secure context storage.
    *   *Embedded/Hardware:*
        *   "ai-home-assistant-hid-dashboard": Arduino R4 WiFi (LCD stats), ESP32 (voice control), MQTT/Tailscale.
        *   "controller-termico-proattivo-esp32": Proactive fan control.
        *   "ai-model-selector-physical-controller": ESP32 rotary encoder, HID keyboard input for model selection.
    *   *Creative/Other:*
        *   "bot-short": C++ Telegram bot, SVG/AI graphics.
        *   "megatool": OSINT C++ + Flask + AI photo analysis.
        *   "videostudio": Higgsfield clips, storyboard LLM.
        *   "silvioprint": Various pipelines.

3.  **Drafting - Section by Section:**

    *   **Header:**
        *   Name: Silvio Chessari.
        *   Roles: Engineer specialized in LLM inference, custom AI hardware infrastructure, and embedded systems.
        *   Emojis: Use 2 max. Let's use a chip and a terminal or brain. `⚡` and `🤖` or similar. Let's go with `⚙️` and `🔌` to emphasize hardware/infrastructure. Actually, the prompt says "Max 2 emojis total (header only)". Let's keep it very professional. `🧪` and `⚡`.

    *   **Bio (3 lines):**
        *   Focus: LLM inference optimization, CUDA hacking (P40), embedded integration.
        *   Draft 1: Specializing in high-performance LLM inference on legacy and consumer hardware, particularly the Tesla P40 (sm_61). Expert in speculative decoding, MoE routing, and CUDA compatibility shims. Architect of autonomous local AI stacks integrating embedded controllers for physical interaction.
        *   Refining for precision: "Specializing in high-performance LLM inference on legacy hardware (Tesla P40 sm_61) via CUDA shimming and speculative decoding. Expert in GGUF/EXL2 quantization pipelines, MoE routing, and integrating embedded systems with local AI stacks. Engineer of autonomous GPU infrastructure and low-latency physical controllers."

    *   **Stack Table:**
        *   Columns: Category, Tech.
        *   Rows: Inference, Hardware, Embedded, Automation.
        *   Content: `llama.cpp`, `GGUF/EXL2`, `CUDA sm_61`, `Tesla P40`, `ESP32`, `Arduino R4`, `MQTT`, `Python/C++`.

    *   **Project Sections (Mapping source to target categories):**

        *   *LLM Research*
            *   Nex2 Mini Phase Twin -> `nex2-mini-phase-twin-30b-lowvram-gguf-model`. Desc: Low-VRAM GGUF model optimized for dense inference on constrained memory footprints.
            *   Auto Quantization -> `auto-quantization-pipeline-gguf`. Desc: Automated benchmarking pipeline on P40/3050 to determine optimal GGUF quantization points (Q4_K_M vs Q5_K_S).
            *   EXL2 Pipeline -> `automated-exl2-conversion-validation-pipeline`. Desc: C++/Python toolchain for Qwen3.5 MoE architecture fixing, EXL2 conversion, and mixed quantization validation.
            *   Add Video Input -> `add-video-input-support-to-llamacpp-mtmd`. Desc: Extension to llama.cpp enabling webcam/file video frame extraction for multimodal inference.

        *   *AI Infrastructure*
            *   AI Dashboard -> `ai-dashboard`. Desc: Web-based monitoring system (:9190) tracking GPU metrics, service health, and AGENDA.md task management.
            *   Boot Watchdog -> `automazione-bootwatchdog-ai-avanzato`. Desc: Advanced systemd watchdog monitoring `llama-stack` VRAM/token-per-second with Telegram-based anomaly alerts.
            *   OpenClaw -> `openclaw`. Desc: Node.js gateway for Ollama providing unified access to local inference endpoints.

        *   *Tools & Automation*
            *   Bot Short -> `bot-short`. Desc: C++ Telegram bot generating AI vector graphics and SVG files via Python pipelines.
            *   Megatool -> `megatool`. Desc: OSINT suite combining C++ data gathering with a Flask web interface and AI photo analysis.
            *   VideoStudio -> `videostudio`. Desc: Storyboard generator using local LLMs to create narrative scripts for Higgsfield AI video clips.
            *   Reddit Monitor -> `reddit-monitor`. Desc: Python script tracking AI/tech subreddits to aggregate ideas into the AGENDA.md workflow.

        *   *Embedded & Hardware*
            *   AI Home Assistant -> `ai-home-assistant-hid-dashboard`. Desc: Arduino R4 WiFi and ESP32 physical controller displaying P40/3050 stats via MQTT and Tailscale.
            *   Thermal Controller -> `controller-termico-proattivo-esp32`. Desc: Proactive fan control system utilizing sensor data and thermal prediction logic on ESP32.
            *   Model Selector -> `ai-model-selector-physical-controller`. Desc: Rotary encoder interface and OLED display switching local AI models via HID keyboard emulation.
            *   Bias Whisper -> `bias-personalizzato-per-whisper-locale`. Desc: Context-aware bias correction module for local Whisper transcription using JSON/TSV definitions.

    *   **GitHub Stats:**
        *   Standard placeholders? Or specific instructions? "GitHub stats" usually implies `github-readme-stats` images. I will generate the markdown for those badges.

4.  **Review and Formatting:**
    *   Check line count estimates.
    *   Header (5 lines)
    *   Bio (3 lines)
    *   Stack Table (10 lines)
    *   LLM Research section (5 lines title + 4 items = 9 lines)
    *   Infra section (5 lines title + 3 items = 8 lines)
    *   Tools section (5 lines title + 4 items = 9 lines)
    *   Embedded section (5 lines title + 4 items = 9 lines)
    *   Stats (5 lines)
    *   Total approx: ~58 lines.
    *   *Adjustment:* The user asked for 90-120 lines. I need to expand the content within the structure to meet the length constraint without adding fluff. I will add a "Highlights" or "Technical Deep Dive" section, or expand the project descriptions slightly to be more detailed (2 lines instead of 1) or add a specific "Hardware Specs" section, or use a wider layout.
    *   *Strategy Update:* I will expand the "Tech Stack" to be a grid with descriptions. I will make the Project Descriptions 2 lines each to add density. I will add a "Research Focus" section between Bio and Stack to detail the specific algorithms mentioned (EAGLE, MTP, MoE).

5.  **Rethinking the Structure to meet 90-120 lines:**

    *   *Header & Bio*: Keep tight.
    *   *Research Focus* (New): Bullet points on LLM Inference methods.
    *   *Tech Stack*: Grid layout.
    *   *Projects*: Use 2-line descriptions for depth.
    *   *Infrastructure Diagrams/Details*: Maybe a text-based representation of the stack topology? No, too much fluff.
    *   *Refined Plan*:
        1.  Header
        2.  Bio
        3.  **Research Interests** (3 bullets: Inference, Optimization, Hardware)
        4.  **Technical Stack** (Table)
        5.  **Projects** (4 sections)
        6.  stats

    *Let's try to count again with 2-line project descriptions.*
    *   Projects: 15 items total. 15 * 2 lines = 30 lines. 4 headers = 4 lines.
    *   Stack: ~8 lines.
    *   Header/Bio: ~8 lines.
    *   Interests: ~5 lines.
    *   Stats: ~5 lines.
    *   Total ~60. Still short.

    *I need to add more specific context or detail to the project descriptions or split the projects into more lists.*
    Let's verify the specific requirement: "For each project: [name](link) + 1-line technical description". Okay, I must stick to 1 line per project.
    Then I MUST add more content sections.
    I will add a **"Hardware Lab"** section describing the physical setup (P40, sm_61 specifics, thermals, CUDA versions) and a **"Current Focus"** section.

    *Revised Structure:*
    1.  Header
    2.  Bio
    3.  **Current Focus**: (EAGLE, sm_61, etc.)
    4.  **Tech Stack**: (Table)
    5.  **Hardware Lab**: (Text description of specs)
    6.  **Projects**: (4 sections)
    7.  **Stats**

    Let's write the content for "Hardware Lab": Focus on the Tesla P