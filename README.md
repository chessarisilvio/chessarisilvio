<div align="center">
  <h1>Silvio Chessari</h1>
  <h3>Technical Architect | AI Infrastructure Researcher</h3>
</div>

Specializing in LLM inference research into speculative decoding and MoE routing across heterogeneous compute. Focused on self-hosted AI stacks and CUDA workarounds for legacy datacenter hardware (e.g., Tesla P40 sm_61). Bridges embedded systems (ESP32) with high-performance inference clusters via custom automation and HID protocols.

### 🛠️ Technical Stack
| Layer | Technologies |
|-------|--------------|
| **Languages** | C++, Python, Bash, CMake, Node.js |
| **AI/Inference** | llama.cpp, EXL2, GGUF, Whisper, Qwen, MoE, OpenCV |
| **Infrastructure** | Docker, Systemd, Ollama, Flask, IPMI, MQTT |
| **Hardware** | NVIDIA Tesla P40, ESP32-S3, DS18B20, HID, OLED SSD1306 |
| **Protocols** | MCP (Model Context Protocol), Telegram API, HTTP/REST |

---

### 🧠 LLM Research
[Automated EXL2 Conversion & Validation Pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline)
> Toolchain for fixing Qwen3_5 MoE architectures, applying mixed-precision EXL2 quantization, and generating local hardware benchmarks.

[Add Video Input Support to llama.cpp (mtmd)](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd)
> Implementation of video capture pipelines (webcam/file) feeding frames into llama.cpp for multimodal model inference via Python stubs.

[Auto-Quantization Pipeline GGUF](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf)
> Automated workflow for downloading LLM checkpoints, benchmarking on Pascal/Ada GPUs, and selecting optimal GGUF quantization layouts.

[Bias Personalizzato per Whisper Locale](https://github.com/chessarisilvio/bias-personalizzato-per-whisper-locale)
> Custom bias injection module (JSON/TSV) for Whisper, enhanced by local GGUF models for contextual post-processing and correction.

---

### 🏗️ AI Infrastructure
[AI Dashboard + Agenda](https://github.com/chessarisilvio/ai-dashboard)
> Local web stack (`:9190`) monitoring GPU metrics/services, integrated with a local 35B model for automated daily agenda and idea generation.

[Automazione Boot/Watchdog AI Avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato)
> Advanced watchdog daemon monitoring `llama-stack` VRAM and token-throughput, ensuring automatic recovery via systemd and Telegram alerts.

[Open-source MCP Bridge for Local Claude Code](https://github.com/chessarisilvio/open-source-mcp-bridge-for-local-claude-code)
> MIT-licensed HTTP bridge acting as an MCP server to integrate local development environments and tools with Claude Code agents.

[CUDA sm_61 Compatibility Shim](https://github.com/chessarisilvio/cuda-sm61-compatibility-shim)
> Compatibility layer enabling modern CUDA toolchains to execute inference workloads on legacy Pascal architecture (Tesla P40).

---

### ⚙️ Tools & Automation
[Git MCP Server for AI Agents](https://github.com/chessarisilvio/git-mcp-server-per-agenti-ai)
> MCP server exposing raw Git operations