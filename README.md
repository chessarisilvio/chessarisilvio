We need to output only the final README.md markdown, no preamble. Must be English, technical, precise, no fluff. Show real technical depth: LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), running LLMs on unsupported consumer/datacenter GPUs (Tesla P40 sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.

Structure: centered header → 3-line technical bio → compact stack table → 4 project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware) → GitHub stats.

For each project: `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.

Use repo slugs derived from project names (lowercase, hyphens).

Max 2 emojis total (header only), rest is clean technical prose.

90–120 lines total.

We need to base on vault data. We have a lot of project names. Need to pick representative projects for each section.

We need to produce a GitHub profile README.md for Silvio Chessari.

We need to include a centered header (maybe using HTML <div align="center"> or using markdown with <p align="center">). Use max 2 emojis in header only.

Then 3-line technical bio: short lines.

Then compact stack table: maybe a markdown table with columns: Language, Framework, Tools.

Then 4 project sections each with heading and list of projects.

Then GitHub stats: maybe using shields.io or just plain text.

We need to keep lines 90-120.

We must not include any extra text outside the markdown.

Let's craft.

First, header: maybe:

```markdown
<div align="center">
# Silvio Chessari
</div>
```

But need max 2 emojis in header only. Could add maybe a computer and a gear emoji? But we can avoid emojis to be safe. Use none.

But requirement: max 2 emojis total (header only). So we can have zero.

We'll do:

```markdown
<div align="center>
# Silvio Chessari
</div>
```

But need correct syntax: `<div align="center">`.

Now 3-line technical bio: maybe:

```
LLM inference researcher | AI systems builder | Embedded hardware engineer
Focus: speculative decoding, MoE routing, GPU kernel tuning for legacy NVIDIA architectures
Self-hosted LLM stack on Tesla P40 (sm_61) & RTX 3050, Arduino/R4 WiFi, ESP32 HID controllers
```

That's three lines.

Now compact stack table: maybe a table with two columns: Category and Technologies.

We'll do:

```
| Category | Technologies |
|----------|--------------|
| Languages | C++, Python, Rust, Bash |
| Frameworks | llama.cpp, TensorRT-LLM, PyTorch, ComfyUI |
| GPU/Accelerators | Tesla P40 (CUDA 11.8, sm_61), RTX 3050 (CUDA 12.x) |
| Embedded | Arduino R4 WiFi, ESP32, ESP-IDF, PlatformIO |
| Tools | Docker, systemd, MQTT/Tailscale, Obsidian vault, GitHub Actions |
```

That's maybe 6 rows.

Now sections:

### LLM Research
List projects: from vault: "Add video input support to llama.cpp (mtmd)", "AI Gateway in prod: alternative concrete a LiteLLM", "Auto-Quantization Pipeline GGUF", "Nex2 Mini Phase Twin 30B low‑VRAM GGUF model", maybe "AI Model Selector Physical Controller" (though that's embedded). Also "AI Influencer" is more media.

We'll pick 4-5 projects per section? Probably each section list a few.

We need to output each as `[name](https://github.com/chessarisilvio/slug)` + 1-line technical description.

We need to derive slugs: lowercase, hyphens.

Examples:

- "Add video input support to llama.cpp (mtmd)" -> slug: `add-video-input-support-to-llamacpp-mtmd`
- "AI Gateway in prod: alternative concrete a LiteLLM" -> slug: `ai-gateway-in-prod-alternative-concrete-a-litellm`
- "Auto-Quantization Pipeline GGUF" -> slug: `auto-quantization-pipeline-gguf`
- "Nex2 Mini Phase Twin 30B low‑VRAM GGUF model" -> slug: `nex2-mini-phase-twin-30b-lowvram-gguf-model`
- "AI Model Selector Physical Controller" -> slug: `ai-model-selector-physical-controller`
- "AI Dashboard" -> slug: `ai-dashboard`
- "AI Home Assistant HID Dashboard" -> slug: `ai-home-assistant-hid-dashboard`
- "Voice Dictate — dettatura locale Whisper per Claude Code" -> slug: `voice-dictate-dettatura-locale-whisper-per-claude-code` maybe too long; we can shorten: `voice-dictate-whisper-claude`
- "Auto Vault Journal" -> slug: `auto-vault-journal`
- "Blender 3D Generation" -> slug: `blender-3d-generation`
- "Barocco Digital" -> slug: `barocco-digital`
- "AI Influencer" -> slug: `ai-influencer`

We need to keep lines count 90-120. Let's estimate.

We'll produce sections with maybe 3-4 projects each.

Now GitHub stats: maybe a line with shields or plain text: `GitHub: @chessarisilvio | Public repos: 27 | Followers: 12` etc. But we don't have actual numbers; we can approximate or leave generic? Should be based on vault? Not provided. We can just put placeholder like `GitHub: @chessarisilvio` and maybe a line with `📊` but that's emoji; we can avoid emojis. Use plain text.

We need to keep total lines 90-120. Let's draft and count.

We'll write markdown.

Let's start constructing.

Line count includes empty lines? Usually yes. We'll aim for about 100 lines.

We'll write:

```
<div align="center">
# Silvio Chessari
</div>

LLM inference researcher | AI systems builder | Embedded hardware engineer
Focus: speculative decoding, MoE routing, GPU kernel tuning for legacy NVIDIA architectures
Self-hosted LLM stack on Tesla P40 (sm_61) & RTX 3050, Arduino/R4 WiFi, ESP32 HID controllers

| Category | Technologies |
|----------|--------------|
| Languages | C++, Python, Rust, Bash |
| Frameworks | llama.cpp, TensorRT-LLM, PyTorch, ComfyUI |
| GPU/Accelerators | Tesla P40 (CUDA 11.8, sm_61), RTX 3050 (CUDA 12.x) |
| Embedded | Arduino R4 WiFi, ESP32, ESP-IDF, PlatformIO |
| Tools | Docker, systemd, MQTT/Tailscale, Obsidian vault, GitHub Actions |

## LLM Research
- [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) – Enables real‑time video frame ingestion for llama.cpp inference pipelines.
- [ai-gateway-in-prod-alternative-concrete-a-litellm](https://github.com/chessarisilvio/ai-gateway-in-prod-alternative-concrete-a-litellm) – Comparative study of LiteLLM alternatives for local OpenAI‑compatible routing on P40/3050.
- [auto-quantization-pipeline-gguf](https://github.com/chessarisilvio/auto-quantization-pipeline-gguf) – Automated GGUF quantization benchmarking Q4_K_M vs Q5_K_S on Tesla P40.
- [nex2-mini-phase-twin-30b-lowvram-gguf-model](https://github.com/chessarisilvio/nex2-mini-phase-twin-30b-lowvram-gguf-model) – Low‑VRAM GGUF port of Nex2 Mini Phase Twin 30B for 24 GB P40.

## AI Infrastructure
- [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) – Web UI at :9190 monitoring GPU, services, agenda and security scans.
- [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) – Arduino R4 WiFi + ESP32 HID dashboard showing VRAM, tok/s, uptime via MQTT/Tailscale.
- [auto-vault-journal](https://github.com/chessarisilvio/auto-vault-journal) – Hook‑driven Obsidian vault updater and session journal for Claude Code.
- [voice-dictate-whisper-claude](https://github.com/chessarisilvio/voice-dictate-whisper-claude) – Space‑bar Whisper turbo GPU dictation plug‑in for Claude Code terminal.

## Tools & Automation
- [blender-3d-generation](https://github.com/chessarisilvio/blender-3d-generation) – Procedural asset pipeline on RTX 3050 using CC0 models and HDRI lighting.
- [barocco-digital](https://github.com/chessarisilvio/barocco-digital) – Astro+Tailwind v4 agency site with Cloudflare Pages deploy and accessibility audit.
- [ai-influencer](https://github.com/chessarisilvio/ai-influencer) – LoRA‑tuned SDXL pipeline for consistent face generation (character “Aria”).
- [ai-model-selector-physical-controller](https://github.com/chessarisilvio/ai-model-selector-physical-controller) – ESP32 rotary encoder + OLED HID controller for local model switching.

## Embedded & Hardware
- [ai-home-assistant-hid-dashboard](https://github.com/chessarisilvio/ai-home-assistant-hid-dashboard) – Duplicate? Already listed; maybe move to Embedded & Hardware only. Let's adjust: we can have it only in Embedded & Hardware, and remove from AI Infrastructure. Let's restructure.

We need 4 sections: LLM Research, AI Infrastructure, Tools & Automation, Embedded & Hardware.

We'll move the dashboard to Embedded & Hardware.

Let's recraft sections.

### LLM Research (as above)

### AI Infrastructure
- [ai-dashboard](https://github.com/chessarisilvio/ai-dashboard) – Web UI at :9190 monitoring GPU, services, agenda and security scans.
- [auto-vault-journal](https://github.com/chessarisilvio/auto-vault-journal) – Hook‑driven Obsidian vault updater and session journal for Claude Code.
- [voice-dictate-whisper-claude](https://github.com/chessarisilvio/voice-dictate-whisper-claude) – Space‑bar Whisper turbo GPU dictation plug‑in for Claude Code terminal.
- [ai-gateway-in