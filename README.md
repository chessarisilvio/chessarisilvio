<div align="center">

# Silvio Chessari
## 🔧 🧠

</div>

Specializing in LLM inference optimization, speculative decoding, and MoE routing architectures.  
Architecting self-built AI infrastructure running on consumer/datacenter GPUs via manual CUDA workarounds.  
Bridging high-level models with embedded systems through MQTT, HID, and custom hardware controllers.

| Focus | Language | Infrastructure | Hardware |
|-------|----------|----------------|----------|
| LLM Inference | Python, C++, CUDA | llama.cpp, GGUF, EXL2 | Tesla P40 (sm_61), RTX 3050 |
| Embedded | C/C++, MicroPython | MQTT, Tailscale, Systemd | Arduino R4, ESP32, OLED |
| Automation | Bash, Node.js | Ollama, Docker | Custom Sensors, Thermal Arrays |

---

## 🔬 LLM Research

**[nex2-mini-phase-twin-30b-lowvram-gguf-model](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model)**
Custom 30B parameter model quantized into a low-VRAM GGUF format for deployment on constrained consumer hardware.

**[add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd)**
Extended llama.cpp backend to support direct video frame ingestion for multimodal LLM inference pipelines.

**[automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline)**
Toolchain for fixing Qwen3.5 MoE architecture, converting to EXL2 with mixed quantization, and validating output benchmarks.

**[benchmark-4-agent-wrappers-on-qwen3627b-llamacpp](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp)**
Comparative analysis of four agent wrappers on Qwen3.6-27B, measuring latency, VRAM footprint, and response quality.

---

## 🏗️ AI Infrastructure

**[automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato)**
Advanced Systemd watchdog monitoring llama-stack health, VRAM utilization, and token throughput with Telegram alerting.