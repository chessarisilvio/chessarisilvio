<div align="center">

# 🔧 Silvio Chessari

</div>

Specialized in high-performance LLM inference on legacy GPU architectures and edge-deployed AI infrastructure. Focuses on CUDA sm_61 compatibility shims, MoE routing optimization, and multimodal speculative decoding. Builds custom embedded systems (ESP32) and automated toolchains for local AI stacks.

| Domain | Technologies |
|--------|--------------|
| **Inference** | llama.cpp, EXL2, Qwen2.5VL, Speculative Decoding |
| **Hardware** | Tesla P40 (Pascal), ESP32, CUDA, HID, 1-Wire |
| **Infrastructure** | FastAPI, Prometheus, Flask, Docker, Systemd |
| **Languages** | C++, Python, Node.js, CMake |

### LLM Research & Inference

*   [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) – Automated toolchain fixing Qwen3_5 Mixture-of-Experts architectures and quantizing checkpoints to EXL2.
*   [cuda-sm61-compatibility-shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim) – CUDA compatibility layer enabling LLM inference on unsupported Pascal GPUs (sm_61).
*   [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) – Integration of video input frames into llama.cpp via OpenCV for multimodal inference.
*   [ll