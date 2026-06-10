<h1 align="center">Silvio Chessari 🚀🤖</h1>

**Researcher in LLM inference, AI infrastructure engineer, embedded systems developer**  
**Focused on speculative decoding, MoE routing, and GPU‑compatibility hacks**  
**Building end‑to‑end pipelines from silicon to cloud‑scale inference**

| Layer | Technologies |
|-------|--------------|
| **Languages** | C++, Python, Rust, Bash, CUDA, CMake |
| **Frameworks** | PyTorch, TensorFlow, FastAPI, Flask, ComfyUI, llama.cpp, BeeLLama |
| **GPU / Compute** | NVIDIA Tesla P40 (sm_61), RTX 3050, CUDA 12.x, OpenCL, cuBLAS, TensorRT |
| **Embedded** | ESP32‑WROOM‑32, Arduino, OLED SSD1306, DS18B20, MOSFET PWM, USB‑HID |
| **Ops / CI** | Docker, Docker‑Compose, GitHub Actions, systemd, Prometheus, Grafana |
| **Tools** | OpenCV, CMake, Make, Git, FastAPI, MCP, JSON‑API, gguf, EXL2 |

---

## LLM Research

- **[eagle](https://github.com/chessarisilvio/eagle)** – Adaptive Early‑Exit Generation for LLMs using dynamic token pruning.  
- **[mtp](https://github.com/chessarisilvio/mtp)** – Multi‑Task Prompting framework supporting cross‑modal instruction tuning.  
- **[speculative-decoding](https://github.com/chessarisilvio/speculative-decoding)** – Implementation of speculative inference with a lightweight verification model to double throughput on consumer GPUs.  
- **[moe-routing](https://github.com/chessarisilvio/moe-routing)** – Hierarchical Mixture‑of‑Experts router with load‑balancing heuristics for sparse activation on Pascal GPUs.

---

## AI Infrastructure

- **[llm-stack](https://github.com/chessarisilvio/llm-stack)** – Self‑hosted inference stack (BeeLLama, vLLM fork, CUDA sm_61 shim) orchestrated via Docker‑Compose and Prometheus metrics.  
- **[mtop](https://github.com/chessarisilvio/mtop)** – Real‑time htop‑like monitor for local LLM inference, displaying GPU utilization, token latency, and KV‑cache pressure.  
- **[git-mcp-server](https://github.com/chessarisilvio/git-mcp-server)** – Model Context Protocol server exposing Git operations as JSON‑API for autonomous AI agents.  
- **[openclaw](https://github.com/chessarisilvio/openclaw)** – Node.js gateway translating Ollama calls to local LLM services with JWT authentication.

---

## Tools & Automation

- **[megatool](https://github.com/chessarisilvio/megatool)** – Integrated OSINT suite (C++ core, Flask UI) with AI‑enhanced image analysis pipelines.  
- **[automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline)** – End‑to‑end C++/Python pipeline for Qwen3‑MoE checkpoint fixing, EXL2 quantization, and benchmark validation.  
- **[add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd)** – CMake extensions and OpenCV stub enabling webcam/video frame streaming into llama.cpp for multimodal prompting.  
- **[cuda-sm61-compatibility-shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim)** – Runtime shim that patches CUDA driver calls, enabling Pascal (Tesla P40) GPUs to run CUDA >=11 binaries without recompilation.

---

## Embedded & Hardware

- **[controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32)** – ESP32 firmware that reads dual DS18B20 sensors on a Tesla P40 and drives a MOSFET‑based fan PWM loop for proactive thermal management.  
- **[digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd)** – USB‑HID driver and Python daemon displaying CPU/GPU temps on a Thermalright LCD panel with 7‑segment emulation.  
- **[ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller)** – Rotary encoder + OLED UI on ESP32 to switch local LLM checkpoints via HID keyboard shortcuts or OpenClaw gateway.  
- **[bot-short](https://github.com/chessarisilvio/bot-short)** – Telegram bot written in C++ that generates SVG/EPS graphics using local diffusion models and streams them to users.

---

### GitHub Stats

![Silvio's GitHub stats](https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=transparent)  
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=chessarisilvio&layout=compact&theme=transparent)  

---