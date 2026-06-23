<div align="center">

# Silvio Chessari
## AI Systems Engineer & Inference Researcher

</div>

Specializing in high-performance LLM inference on consumer and datacenter hardware. Expertise in speculative decoding (EAGLE/MTP), MoE routing optimization, and CUDA shims for sm_61 (Tesla P40). Building resilient local AI infrastructure, automated quantization pipelines, and embedded telemetry systems.

### Technical Stack

| Category | Technologies |
|----------|--------------|
| **Compute** | Tesla P40 (sm_61), RTX 3050, ESP32, Arduino R4 WiFi |
| **Inference** | llama.cpp, EXL2, GGUF, Speculative Decoding, vLLM |
| **Languages** | Python, C++, Bash, OpenCV, Node.js, Rust |
| **Systems** | Docker, systemd, Tailscale, MQTT, HID protocols |

---

### LLM Research & Optimization

*   [Nex2 Mini Phase Twin 30B low-VRAM GGUF model](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model)
    Production-ready GGUF model optimized for low-VRAM constraints through advanced quantization techniques.
*   [Benchmark 4 agent wrappers on Qwen3.6‑27B (llama.cpp)](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp)
    Comparative analysis of agent wrappers (Pi, OpenCode, Hermes) measuring latency and VRAM footprint on constrained hardware.
*   [Add video input support to llama.cpp (mtmd)](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd)
    CMake integration and stubs extending llama.cpp backend to accept direct webcam/video frame inputs for multimodal tasks.
*   [Bias personalizzato per Whisper locale](https://github.com/chessarisilvio/bias-personalizado-per-whisper-locale)
    Post-processing module applying JSON/TSV biases and LLM-driven context correction to improve local Whisper transcription accuracy.

### AI Infrastructure & Pipelines

*   [Automated EXL2 Conversion & Validation Pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline)
    C++ and Python toolchain for fixing Qwen3_5Moe architectures, executing mixed-bit EXL2 conversion, and validation benchmarking.
*   [Auto-Quantization Pipeline GGUF](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf)
    Orchestration script for automated checkpoint downloading, Q4_K_M vs Q5_K_S efficiency testing, and production GGUF generation.
*   [Automated GGUF Benchmarking System](https://github.com/chess