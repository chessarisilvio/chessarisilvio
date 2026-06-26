<h1 align="center">Silvio Chessari</h1>
<h3 align="center">LLM inference researcher · self-hosted AI infrastructure · embedded systems</h3>

Local-first LLM inference on unsupported GPUs (Tesla P40 / RTX 3050), speculative decoding, MoE routing, embedded AI dashboards, and full-stack automation.

<table>
<tr>
<td width="50%">

**Languages**
Python · Bash · C/C++ · CUDA · JavaScript · HTML/CSS

**Inference Stack**
llama.cpp · ExLlamaV2 · Ollama · Custom speculative decoding (EAGLE/MTP)

**Quantization**
GGUF · Q4_K_M · Q5_K_S · Mixed-precision EXL2

**Hardware**
NVIDIA Tesla P40 (sm_61) · RTX 3050 (8 GB) · Arduino R4 · ESP32

</td>
<td width="50%">

**Infra**
systemd · Docker · Tailscale · MQTT · Node.js · Flask

**DevOps**
GitHub Actions · systemd timers · watchdog CI · Bash orchestration

**Tools**
OpenClaw gateway · Whisper · Obsidian vault-driven automation · agent wrappers

**Embedded**
HID · OLED/SSD1306 · EXIF/GPS extraction · thermal ESP32 controllers

</td>
</tr>
</table>

## 🔬 LLM Research

- [benchmark-4-agent-wrappers-on-qwen3627b-llamacpp](https://github.com/chessarisilvio/benchmark-4-agent-wrappers-on-qwen3627b-llamacpp) — comparative benchmark of four agent wrappers on Qwen3.6-27B via llama.cpp  
- [automated-exl2-conversion-validation-pipeline](https://github.com/chessarisilvio/automated-exl2-conversion-validation-pipeline) — automated Qwen3_5MoeForC architecture fix → EXL2 conversion, mixed quantization, and benchmark validation  
- [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) — video input support for llama.cpp (mtmd): webcam/file frame acquisition for LLM inference  
- [nex2-mini-phase-twin-30b-lowvram-gguf-model](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model) — 30B parameter GGUF model quantized for low-VRAM local inference  
- [secure-llm-context-vault](https://github.com/chessarisilvio/secure-llm-context-vault) — encrypted archive for storing and retrieving LLM conversation contexts  

## 🖥️ AI Infrastructure

- [ai-gateway-in-prod-alternative-concrete-a-litellm](https://github.com/chessarisilvio/ai-gateway-in-prod-alternative-concrete-a-litellm) — evaluation of 10 concrete alternatives to LiteLLM for consumer GPU routing on P40 + RTX 3050 (20 GB RAM)  
- [openclaw](https://github.com/chessarisilvio/openclaw) — self-hosted Ollama gateway (Node.js) with model routing for local inference  
- [auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) — automated download → benchmark → GGUF quantization (Q4_K_M / Q5_K_S) on P40/3050 hardware  
- [sistema-di-benchmarking-automatizzato-per-nuovi-mo](https://github.com/chessarisilvio/sistema-di-benchmarking-automatizzato-per-nuovi-mo) — automated GGUF model benchmarking on P40 and RTX 3050 with auto-generated reports  
- [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) — local web dashboard (:9190) for GPU monitoring, AGENDA.md, worker subtask tracking, unified security scanning  

## ⚙️ Tools & Automation

- [voice-dictate](https://github.com/chessarisilvio/voice-dictate) — push-to-talk Whisper turbo GPU dictation for Claude Code supporting Italian language transcription  
- [automazione-bootwatchdog-ai-avanzato](https://github.com/chessarisilvio/automazione-bootwatchdog-ai-avanzato) — advanced llama-stack watchdog: process health, VRAM monitoring, token-rate anomaly detection, Telegram alerting, systemd auto-restart  
- [automazione-systemd-timer-per-html-minification-gi](https://github.com/chessarisilvio/automazione-systemd-timer-per-html-minification-gi) — systemd-driven HTML minification pipeline with automated GitHub Pages deployment  

## 🔌 Embedded & Hardware

- [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) — Arduino R4 WiFi + ESP32 hardware dashboard displaying P40/3050 stats (VRAM, tok/s, uptime) with local voice commands via MQTT/Tailscale  
- [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) — ESP32 rotary-encoder + OLED controller for hardware selection of local AI models via HID commands  
- [controller-termico-proattivo-esp32](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) — proactive ESP32 thermal management: predictive fan control + temperature sensor array  
- [digital-thermal-lcd](https://github.com/chessarisilvio/digital-thermal-lcd) — ThermalRight LCD temperature display interfaced via HID protocol  

<br clear="both" align="center"/>

---

<p align="center">
  <img height="150" src="https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=transparent&hide_title=true&count_private=true"/>
  <img height="150" src="https://github-readme-stats.vercel.app/api/top-langs/?username=chessarisilvio&layout=compact&theme=transparent&hide_title=true"/>
</p>