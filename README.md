<div align="center">

# Silvio Chessari

**AI/GPU Inference Optimization · Embedded Systems · Linux**

[![GitHub followers](https://img.shields.io/github/followers/chessarisilvio?style=flat-square&color=blue)](https://github.com/chessarisilvio)
[![Profile views](https://komarev.com/ghpvc/?username=chessarisilvio&style=flat-square&color=grey)](https://github.com/chessarisilvio)

</div>

---

## Chi sono

Sviluppatore specializzato in due aree che mi appassionano:

**AI/GPU Inference** — Ottimizzo l'esecuzione di modelli linguistici su hardware consumer e datacenter. Il mio setup è una **Tesla P40 (24 GB VRAM)** + **RTX 3050** su cui faccio girare LLM quantizzati in produzione. Mi occupo di speculative decoding (EAGLE, MTP), routing multi-GPU, kernel CUDA su architetture non supportate (sm_61), integrazione con llama.cpp ed ExLlamaV2, e gestione avanzata di modelli GGUF.

**Embedded & Hardware** — Progetto firmware per ESP32, driver kernel Linux per periferiche (display TFT, SPI), PCB custom con KiCad e sistemi IoT con logica AI locale. Mi piace arrivare fino all'hardware.

---

## Stack

```
AI/ML      Python · CUDA · llama.cpp · ExLlamaV2 · GGUF/EXL2 · PyTorch · EAGLE/MTP
Backend    Node.js · FastAPI · Python · systemd
Embedded   ESP32 · Raspberry Pi · C/C++ · ESPHome · KiCad
Sistemi    Linux (Ubuntu) · Bash · Docker · Git
```

---

## Progetti principali

### 🤖 AI & GPU Inference

| Progetto | Descrizione |
|----------|-------------|
| [**gguf-model-manager-cli**](https://github.com/chessarisilvio/gguf-model-manager-cli) | CLI Python per gestire modelli GGUF: download HuggingFace con SHA256, catalogo JSON, stima VRAM, dedup |
| [**router-cuda-exllamav2-p40**](https://github.com/chessarisilvio/router-cuda-dinamico-exllamav2-p40-rtx3050) | Intercetta i `no kernel image` su P40 (sm_61) e fallback automatico su RTX 3050 (sm_86) |
| [**proxy-anthropic-openai**](https://github.com/chessarisilvio/proxy-anthropic-openai-con-safety-hooks) | Gateway Node.js con hook LLM configurabili (Pre-Bash, Post-Edit, Memory) per Anthropic/OpenAI |
| [**correction-net-speculative-decoding**](https://github.com/chessarisilvio/correction-net-per-speculative-decoding) | Correction network per aumentare l'acceptance rate di EAGLE/MTP su P40 |
| [**dashboard-telemetrica-ai**](https://github.com/chessarisilvio/dashboard-telemetrica-ai-hardware) | Dashboard real-time GPU/CPU con alert Telegram quando VRAM > 85% o temp > 75°C |
| [**gateway-telegram-multimodale**](https://github.com/chessarisilvio/gateway-telegram-multimodale-offline) | Bot Telegram completamente offline: pipeline Whisper + Moondream per audio e immagini |

### ⚡ Embedded & Hardware

| Progetto | Descrizione |
|----------|-------------|
| [**mpi3501-kernel-6.12-driver**](https://github.com/chessarisilvio/mpi3501-kernel-6.12-driver) | Device Tree overlay per display TFT ILI9486 (MPI3501) su Raspberry Pi con kernel 6.12+ |
| [**controller-termico-esp32**](https://github.com/chessarisilvio/controller-termico-proattivo-esp32) | Firmware ESP32 che legge la temperatura P40 via IPMI e regola proattivamente le ventole |
| [**pcb-esp32-nrf24**](https://github.com/chessarisilvio/pcb-esp32-nrf24) | PCB custom per ESP32 + moduli NRF24L01 multipli su banda 2.4 GHz |
| [**garden-irrigator-esp32**](https://github.com/chessarisilvio/garden-irrigator-esp32) | Sistema di irrigazione smart: ESP32 con sensori DHT22, notifiche Telegram in tempo reale |

---

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=dark&hide_border=true&include_all_commits=true)
&nbsp;
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=chessarisilvio&layout=compact&theme=dark&hide_border=true&langs_count=6)

</div>
