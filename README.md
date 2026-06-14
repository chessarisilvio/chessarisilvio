1.  **Analyze the Request:**
    *   **Role:** Technical Writer.
    *   **Task:** Generate a professional GitHub profile README.md for Silvio Chessari based on provided vault data.
    *   **Strict Requirements:**
        *   Output ONLY the final README.md markdown (no preamble, no explanation).
        *   Language: English, technical, precise, no fluff.
        *   Content Focus: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), running LLMs on unsupported GPUs (Tesla P40 sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.
        *   Structure: Centered header -> 3-line technical bio -> Compact stack table -> 4 project sections -> GitHub stats.
        *   Links: `[name](https://github.com/chessarisilvio/slug)` format based on project names.
        *   Repo Slugs: Lowercase, hyphens.
        *   Emojis: Max 2 (header only).
        *   Length: 90–120 lines.
    *   **Source Material:** A vault dump (Markdown/JSON-like structure) containing project names, paths, descriptions, and tags. Key terms include: Tesla P40, RTX 3050, GGUF, EXL2, ESP32, Arduino R4, CUDA sm_61, llama.cpp, watchdog, MQTT, Tailscale, openclaw.

2.  **Drafting - Section by Section:**

    *   **Header:** Needs to be centered, name, title, maybe 2 emojis.
        *   *Draft:*
            ```markdown
            <div align="center">

            ### Silvio Chessari
            **LLM Research Engineer · AI Infrastructure · Embedded Systems**

            </div>
            ```

    *   **Bio:** 3 lines. Technical, precise. Focus on inference, unsupported hardware, infrastructure.
        *   *Content:* L1 - Speculative decoding/EAGLE/MoE research. L2 - optimizing inference for legacy Pascal (Tesla P40) and consumer GPUs via CUDA shims. L3 - Building physical-digital interfaces for AI stacks.
        *   *Draft:*
            Researching LLM acceleration via EAGLE, MTP, and speculative decoding, with a focus on MoE routing optimization. Engineer specialized in deploying large models on unsupported hardware (Tesla P40 sm_61) through custom CUDA patches and quantization pipelines. Architect of self-hosted AI infrastructure bridging embedded controllers and local inference clusters.

    *   **Compact Stack Table:** Need a summary of skills seen in the data.
        *   *Skills seen:* C++, Python, CUDA, CMake, ESP32, Arduino, Telegram Bots, Ollama, llama.cpp, EXL2, GGUF.
        *   *Categories:* Inference, Hardware/Embedded, DevOps/Tools, Languages.
        *   *Draft:*
            | **Area** | **Tech** |
            | :--- | :--- |
            | **Inference** | llama.cpp, EAGLE, EXL2, GGUF, MoE routing |
            | **Hardware** | Tesla P40 (sm_61), RTX 3050, Arduino R4, ESP32 |
            | **Stack** | CUDA, C++, Python, CMake, OpenCV, Node.js |
            | **Infrastructure** | Ollama, Tailscale, MQTT, Dockerless, Systemd |

    *   **Project Sections:** The request asks for 4 sections: LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware. I need to map the vault projects to these.

        *   *LLM Research:*
            *   "Add video input support to llama.cpp (mtmd)" -> `add-video-input-support-to-llamacpp-mtmd`
            *   "Automated EXL2 Conversion & Validation Pipeline" -> `automated-exl2-conversion-validation-pipeline`
            *   "Auto-Quantization Pipeline GGUF" -> `auto-quantization-pipeline-gguf`

        *   *AI Infrastructure:*
            *   "AI Dashboard" -> `ai-dashboard`
            *   "Openclaw" -> `openclaw`
            *   "Automazione Boot/Watchdog AI Avanzato" -> `automazione-bootwatchdog-ai-avanzato`

        *   *Tools & Automation:*
            *   "Megatool" -> `megatool`
            *   "Reddit Monitor" -> `reddit-monitor`
            *   "mtop: htop per monitoraggio LLM locale" -> `mtop`

        *   *Embedded & Hardware:*
            *   "AI Home Assistant HID Dashboard" -> `ai-home-assistant-hid-dashboard`
            *   "Controller Termico ESP32" -> `controller-termico-proattivo-esp32`
            *   "AI Model Selector Physical Controller" -> `ai-model-selector-physical-controller`
            *   "CUDA sm_61 Compatibility Shim" -> `cuda-sm61-compatibility-shim` (Fits Hardware/Infra, but "Hardware" fits since it's about hardware support).

    *   **Formatting Projects:** `[name](https://github.com/chessarisilvio/slug)` + 1-line description.

    *   **GitHub Stats:** Standard placeholder at the bottom.

    *   **Refining Descriptions (Technical & Precise):**
        *   *Add video...:* Extends llama.cpp backend for video input support, integrating CMake builds and OpenCV capture pipelines.
        *   *Automated EXL2...:* Python/C++ toolchain for architecture fixing, mixed-precision EXL2 conversion, and validation benchmarking.
        *   *Auto-Quantization...:* Automated pipeline for GGUF benchmarking on P40/RTX3050, optimizing quantization strategies.
        *   *AI Dashboard:* Local monitoring server (:9190) tracking GPU metrics, service states, and automated agenda generation.
        *   *Openclaw:* Node.js gateway for Ollama inference, facilitating local AI service orchestration.
        *   *Automazione Boot...:* Advanced systemd watchdog monitoring `llama-stack` VRAM/token-rate with Telegram alerting.
        *   *Megatool:* C++ OSINT suite with Flask web interface and AI photo analysis capabilities.
        *   *Reddit Monitor:* Python script tracking AI/tech subreddits to generate automated ideas for project agendas.
        *   *mtop:* Real-time htop-like CLI interface monitoring local LLM inference metrics and GPU utilization.
        *   *AI Home Assistant...:* Hardware dashboard (Arduino R4/ESP32) displaying inference stats via MQTT/Tailscale.
        *   *Controller Termico...:* Active thermal management system for workstations using ESP32 sensor arrays.
        *   *AI Model Selector...:* ESP32 rotary controller for physical model selection, interfacing via HID or OpenClaw.
        *   *CUDA sm61...:* Compatibility layer enabling CUDA execution on legacy Pascal (Tesla P40) architectures.

3.  **Review and Assemble:**

    *   *Check Constraints:*
        *   Only output README? Yes.
        *   English? Yes.
        *   Real technical depth? Yes (sm_61, EXL2, GGUF, etc.).
        *   Structure? [Header -> Bio -> Table -> 4 Sections -> Stats]. Yes.
        *   Line count? 90-120. I need to ensure spacing is appropriate but not excessive.

    *   *Slug Generation Check:*
        *   "add-video-input-support-to-llamacpp-mtmd" -> `add-video-input-support-to-llamacpp-mtmd`
        *   "automated-exl2-conversion-validation-pipeline" -> `automated-exl2-conversion-validation-pipeline`
        *   "auto-quantization-pipeline-gguf" -> `auto-quantization-pipeline-gguf`
        *   "ai-dashboard" -> `ai-dashboard`
        *   "openclaw" -> `openclaw`
        *   "automazione-bootwatchdog-ai-avanzato" -> `automazione-bootwatchdog-ai-avanzato`
        *   "megatool" -> `megatool`
        *   "reddit-monitor" -> `reddit-monitor`
        *   "mtop" -> `mtop`
        *   "ai-home-assistant-hid-dashboard" -> `ai-home-assistant-hid-dashboard`
        *   "controller-termico-proattivo-esp32" -> `controller-termico-proattivo-esp32`
        *   "ai-model-selector-physical-controller" -> `ai-model-selector-physical-controller`
        *   "cuda-sm61-compatibility-shim" -> `cuda-sm61-compatibility-shim`

4.  **Final Polish (Self-Correction during drafting):**
    *   *Bio:* "Researching LLM acceleration via EAGLE" - specific mention of EAGLE/MTP/Speculative Decoding requested? "EAGLE/MTP/speculative decoding" is in the prompt requirements. I should include those keywords.
    *   *Bio 2:* "Running LLMs on unsupported consumer/datacenter GPUs (Tesla P40 sm_61)" - make sure to mention sm_61.
    *   *Bio 3:* "Self-built AI infrastructure, embedded systems".
    *   *Layout:* Ensure the headers for sections match exactly "LLM Research", "AI Infrastructure", "Tools & Automation", "Embedded & Hardware".

5.  **Constructing the Final Markdown:** (Proceeding to generate output).
    *   *Note on Line Count:* The request asks for 90-120 lines. With 13 projects, 4 sections, header, bio, table, and stats, standard spacing should land in that range.

    *   *Drafting Content:*
        ```markdown
        <div align="center">

        ### Silvio Chessari
        **LLM Inference Researcher · AI Infrastructure Architect**

        </div>

        Researching LLM acceleration via EAGLE, MTP, and speculative decoding, with a focus on MoE routing optimization. Specialized in porting models to unsupported hardware (Tesla P40 sm_61) using custom CUDA shims and quantization pipelines. Building self-hosted infrastructure bridging embedded systems and local inference clusters.

        ### Technical Stack
        | **Domain** | **Technologies** |
        | :--- | :--- |
        | **Inference** | EAGLE, MTP, llama.cpp, EXL2, GGUF, MoE Routing |
        | **Hardware/Embedded** | Tesla P40 (sm_61), RTX 3050, Arduino R4, ESP32, HID |
        | **Software** | CUDA, C++, Python, CMake, Node.js, OpenCV |
        | **Infrastructure** | Ollama, MQTT, Tailscale, Systemd, Dockerless |

        ### LLM Research & Inference
        - [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd)
          Extends llama.cpp backend for video input support, featuring CMake integration and OpenCV capture pipelines for multimodal inference.
        - [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline)
          C++ and Python toolchain for fixing architecture, mixed-precision EXL2 conversion, and automated validation benchmarking.
        - [auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf)
          Automated benchmarking pipeline for GGUF models on Tesla P40 and RTX