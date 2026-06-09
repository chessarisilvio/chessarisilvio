1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Output:** Professional GitHub Profile README.md.
    *   **Subject:** Silvio Chessari.
    *   **Source Data:** A "technical vault" containing Italian project descriptions (Panoramica Progetti).
    *   **Constraints:**
        *   Output *ONLY* the markdown.
        *   No preamble, no explanation.
        *   Language: English (technical, precise, no fluff).
        *   Content Depth: LLM inference research (speculative decoding/MoE), running LLMs on unsupported GPUs (Tesla P40, sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.
        *   Structure:
            1.  Centered header.
            2.  3-line technical bio.
            3.  Compact stack table.
            4.  4 Project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware).
            5.  GitHub stats.
        *   Project format: `[name](link)` + 1-line technical description.
        *   Slug generation: lowercase, hyphens (e.g., `cuda-sm61-compatibility-shim`).
        *   Emoji limit: Max 2 (header only).
        *   Length: 90–120 lines.
    *   **Specific Data Points to Extract:**
        *   *Bio/Background:* Running local AI, CUDA workarounds (sm_61), Tesla P40.
        *   *Projects:*
            *   *LLM Research:* `add-video-input-support-to-llamacpp-mtmd` (video input to llama.cpp).
            *   *AI Infrastructure:* `start-llama` (launcher), `openclaw` (gateway), `dashboard-telemetrica-ai-hardware` (telemetry).
            *   *Tools & Automation:* `ai-dashboard` (monitoring/automation), `update-github-profile` (auto-readme), `gguf-manager`.
            *   *Embedded & Hardware:* `controller-termico-proattivo-esp32` (P40 fan control), `digital-thermal-lcd` (HID display), `ai-model-selector-physical-controller`.

2.  **Drafting - Section by Section:**

    *   **Header:**
        Needs to be centered, professional, 2 emojis max.
        *   *Draft:*
            # Silvio Chessari
            *LLM Inference Research & High-Performance Infrastructure*

    *   **Bio:**
        3 lines. Needs to focus on hardware optimization, CUDA hackery, and local AI.
        *   *Draft:*
            Researching speculative decoding and MoE routing for efficient local LLM inference.
            Architecting self-hosted AI infrastructure to run modern models on legacy consumer and datacenter hardware via custom CUDA shims.
            Building embedded interfaces to bridge the physical world with large language models.

    *   **Stack Table:**
        Compact. Needs to reflect the tools mentioned.
        *   *Draft:*
            | Area | Tech |
            | :--- | :--- |
            | **Inference** | llama.cpp, Speculative Decoding, MoE Routing |
            | **Hardware** | CUDA sm_61 (Pascal), Tesla P40, ESP32, HID |
            | **Stack** | Node.js, Python, C++, OpenCV, systemd |

    *   **Project Section 1: LLM Research**
        *   Source: `add-video-input-support-to-llamacpp-mtmd`.
        *   Desc: Video input support, webcam/frame capture, CMake modifications.
        *   *Draft:*
            ### LLM Research
            - [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd)  
              Extends llama.cpp runtime with video input capabilities via CMake hooks and a Python OpenCV demo pipeline.

    *   **Project Section 2: AI Infrastructure**
        *   Sources: `start-llama`, `openclaw`, `dashboard-telemetrica-ai-hardware`, `gateway-telegram-multimodale-offline`, `freellmapi`.
        *   *Draft:*
            ### AI Infrastructure
            - [start-llama](https://github.com/chessarisilvio/start-llama)  
              Advanced launcher for `llama-server` managing hardware allocation and preset configurations for local deployment.
            - [openclaw](https://github.com/chessarisilvio/openclaw)  
              Multi-channel AI gateway (Telegram/Web) supporting tool use and session memory interfacing with the local stack.
            - [dashboard-telemetrica-ai-hardware](https://github.com/chessarisilvio/dashboard-telemetrica-ai-hardware)  
              Real-time Flask dashboard monitoring GPU/CPU thermal metrics and service health with Telegram alerts.

    *   **Project Section 3: Tools & Automation**
        *   Sources: `ai-dashboard`, `gguf-model-manager-cli`, `update-github-profile`.
        *   *Draft:*
            ### Tools & Automation
            - [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard)  
              Local web application integrating sprint tracking and idea generation via a 35B parameter backend.
            - [gguf-model-manager-cli](https://github.com/chessarisilvio/gguf-model-manager-cli)  
              Command-line utility for managing, indexing, and verifying GGUF model files for local inference.
            - [update-github-profile](https://github.com/chessarisilvio/update-github-profile)  
              Automated script leveraging local LLM APIs to dynamically generate and deploy project documentation.

    *   **Project Section 4: Embedded & Hardware**
        *   Sources: `controller-termico-proattivo-esp32`, `digital-thermal-lcd`, `ai-model-selector-physical-controller`.
        *   *Draft:*
            ### Embedded & Hardware
            - [controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32)  
              ESP32 firmware providing proactive thermal regulation for Tesla P40 via PWM fan control and 1-Wire sensors.
            - [digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd)  
              Thermalright LCD interface implementation to display real-time CPU/GPU telemetry via USB HID.
            - [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller)  
              Physical rotary controller with OLED integration for tactile selection of local AI models.

    *   **GitHub Stats:**
        Standard image links. Since I don't have the *actual* GitHub username URL structure for badges (though `chessarisilvio` is implied in the prompt), I will use standard placeholder structures or inferred ones.
        *   *Draft:*
            [![GitHub Stats](https://github-readme-stats.vercel.app/api?username=chessarisilvio&hide_title=false&hide_rank=true&show_icons=true&include_all_commits=true&count_private=true&disable_animations=true&theme=dracula)](https://github.com/chessarisilvio)
            [![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=chessarisilvio&layout=compact&langs_count=8&disable_animations=true&theme=dracula)](https://github.com/chessarisilvio)

3.  **Refining and Formatting:**

    *   Check constraints: 90-120 lines? The draft looks a bit short. I need to expand descriptions slightly or ensure spacing adds up without being fluff. I will ensure the descriptions are dense technical prose.
    *   *Self-Correction on Lines:* I need to be careful with the line count. I will use line breaks and spacing effectively in the markdown to hit the target, but keep it "clean".
    *   *Reviewing Technical Depth:* Make sure the CUDA sm_61 and P40 references are emphasized in the Bio and Stack.
    *   *Reviewing URLs:* Ensure slugs are correct (e.g., `controller-termico-proattivo-esp32`).

4.  **Final Polish of the Markdown Text:**

    *   *Header:* Add `<div align="center">`.
    *   *Bio:* Ensure "sm_61" and "Tesla P40" are prominent.
    *   *Projects:* Ensure the language is active ("Extends", "Architects", "Interface").
    *   *Stats:* Use standard stats components.

5.  **Constructing the final output string (simulated):**

    ```markdown
    <div align="center">

    # Silvio Chessari
    *Inference Engineer · Hardware Hacker · Local AI Infrastructure*

    </div>

    Specializing in LLM inference optimization, pushing modern models (MoE/Speculative Decoding) onto legacy hardware via custom CUDA workarounds. Architecting self-hosted AI platforms to bypass cloud dependency, hacking compatibility for GPUs like the Tesla P40 (sm_61). Developing embedded systems to physically control and monitor high-performance inference clusters.

    ### Technical Stack

    | Domain | Technologies |
    | :--- | :--- |
    | **AI & Inference** | llama.cpp, Speculative Decoding, MoE Routing, Diffusers |
    | **Systems** | CUDA (sm_61 shims), Docker, Python, Node.js, C++ |
    | **Embedded** | ESP32, HID Protocol, 1-Wire, PWM Control, OLED (SSD1306) |

    ### LLM Research
    Core experiments focused on extending model capabilities and inference efficiency.

    - [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd)  
      Extends `llama.cpp` inference engine to support direct video input streams, implementing CMake build hooks and an OpenCV-backed Python pipeline for webcam/frame processing.

    ### AI Infrastructure
    Robust tooling for deploying and monitoring local LLM stacks.

    - [start-llama](https://github.com/chessarisilvio/start-llama)  
      Advanced systemd-aware launcher wrapper for `llama-server`, managing hardware presets and initialization sequences for multiple model instances.
    - [openclaw](https://github.com/chessarisilvio/openclaw)  
      Multi-modal AI gateway (Telegram/Web) featuring tool use integration and persistent session memory, routing requests to local backends.
    - [dashboard-telemetrica-ai-hardware](https://github.com/chessarisilvio/dashboard-telemetrica-ai-hardware)  
      Flask-based telemetry dashboard providing real-time visualization of GPU VRAM, thermal loads, and service availability with Telegram alerting hooks.
    - [freellmapi](https://github.com/chessarisilvio/freellmapi)  
      Unified API proxy aggregating free-tier inference providers (Groq, Google, Cerebras) for fallback and hybrid cloud-local deployment strategies.

    ### Tools & Automation
    Utilities enhancing operational efficiency and model management.

    - [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard)  
      Centralized management hub for task tracking and automated idea generation, utilizing a local 35B parameter model backend.
    - [gguf-model-manager-cli](https://github.com/chessarisilvio/gguf-model-manager-cli)  
      Specialized CLI utility for indexing, verifying integrity, and managing version control of local GGUF model repositories.
    - [update-github-profile](https://github.com/chessarisilvio/update-github-profile