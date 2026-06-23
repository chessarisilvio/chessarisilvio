<h1 align="center">Silvio Chessari 🚀🤖</h1>

**Researcher in LLM inference optimization (EAGLE, MTP, speculative decoding, MoE routing).**  
**Engineer building AI stacks on legacy GPUs (Tesla P40 sm_61, CUDA compatibility shim).**  
**Embedded‑systems hobbyist integrating AI with Arduino, ESP32, and custom dashboards.**  

---

| Category            | Primary Tools & Libraries                              |
|---------------------|--------------------------------------------------------|
| LLM Inference       | llama.cpp, gguf, EXL2, speculative decoding, MoE routing |
| GPU Compatibility   | CUDA sm_61 shim, NVCC patches, Tesla P40, RTX 3050      |
| AI Stack            | systemd, Docker, OpenClaw, MQTT, Tailscale             |
| Embedded            | Arduino R4 WiFi, ESP32‑S2, HID, OLED/ LCD displays      |
| Automation & Ops   | Bash, Python 3.11, CMake, Flask, C++                    |

---

## LLM Research  

- **[add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd)**  
  *Extends llama.cpp with CMake‑driven video frame ingestion and a Python demo pipeline for multimodal inference.*  

- **[benchmark-4-agent-wrappers-on-qwen3627b-llamacpp](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp)**  
  *Compares latency, VRAM usage and output quality of four agent wrappers on Qwen 3.6‑27B (Q4 gguf) on Tesla P40 & RTX 3050.*  

- **[auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf)**  
  *Automates checkpoint download, rapid hardware‑specific GGUF quantization (Q4_K_M vs Q5_K_S) and documentation update.*  

- **[automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline)**  
  *C++/Python toolchain that fixes Qwen3_5MoeForC architecture, converts to EXL2, applies mixed‑precision quantization and runs validation benchmarks.*  

- **[secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault)**  
  *Encrypted storage for prompt/context vectors with per‑model access controls, enabling safe multi‑tenant inference.*  

- **[noema-atlas-rete-p2p-per-modelli-llm](https://github.com/chessarisilvio/noema-atlas-rete-p2p-per-modelli-llm)**  
  *Peer‑to‑peer network for distributing LLM weights across heterogeneous nodes, reducing central bandwidth requirements.*  

---

## AI Infrastructure  

- **[openclaw](https://github.com/chessarisilvio/openclaw)**  
  *Node.js gateway that bridges local LLM services with Ollama, exposing REST & WebSocket endpoints.*  

- **[ai-dashboard](https://github.com/chessarisilvio/ai-dashboard)**  
  *Local web UI (http://localhost:9190) showing GPU metrics, service health, agenda items and a 35B idea‑generator worker.*  

- **[ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard)**  
  *Arduino R4 WiFi + ESP32 HID panel displaying P40/RTX3050 status and accepting voice commands via MQTT/Tailscale.*  

- **[automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato)**  
  *systemd‑based watchdog for llama‑stack that monitors VRAM, token‑per‑second and auto‑restarts with Telegram alerts.*  

- **[llm-stack](https://github.com/chessarisilvio/llm-stack)**  
  *Self‑hosted stack configuration (docker‑compose, NVIDIA‑driver patches, model serving) for multi‑GPU inference on consumer hardware.*  

- **[sistema-di-benchmarking-automatizzato-per-nuovi-mo](https://github.com/ch