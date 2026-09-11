We need to output only README.md, no preamble. Structure: centered header → 3-line technical bio → compact stack table → 4 project sections (LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware) → GitHub stats.

We need to use real technical details from vault. Must include LLM inference research (EAGLE/MTP/speculative decoding/MoE routing), running LLMs on unsupported consumer/datacenter GPUs (Tesla P40 sm_61, CUDA workarounds), self-built AI infrastructure, embedded systems.

Need project entries: each project: [name](https://github.com/chessarisilvio/slug) + 1-line technical description. Use repo slugs derived from project names (lowercase, hyphens).

We need max 2 emojis total (header only). So we can include maybe a rocket or star in header. Rest must be clean technical prose.

90-120 lines total.

We need to produce final markdown.

We'll need to infer some projects from vault. There are many project names; we need to choose some for each section.

We need to include centered header: maybe using HTML <div align="center"> or using markdown centered? Usually you can use <p align="center">. We'll do:

<div align="center">
# Silvio Chessari
...
</div>

But header only can have max 2 emojis; we can put maybe 🚀 and 🔧.

Then 3-line technical bio: short lines.

Compact stack table: maybe a markdown table with two columns: Language, Tools etc.

Then sections: each with heading and list of projects.

Finally GitHub stats: maybe using shields.io or just plain text: GitHub Stats: ... We'll just put something like:

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=chessarisilvio&show_icons=true&theme=dark) but that's an image, not emoji; but it's okay? The restriction only about emojis, not images. Probably fine.

But we need to keep within 90-120 lines. We'll aim around 100 lines.

We need to derive slugs: lower case, hyphens.

We'll need to pick projects from vault that match categories:

LLM Research: add-video-input-support-to-llamacpp-mtmd, auto-quantization-pipeline-gguf, auto-tuning-dinamico-per-gemma-4-26b-su-p40, ai-model-selector-physical-controller? maybe more research: maybe speculative decoding? Not in vault but we can mention EAGLE/MTP etc from research. However we need to show real technical depth from vault data; we can mention that he researched EAGLE/MTP etc. But we need to reference actual projects? Could include a project named "llm-research-eagle-mtp" but not in vault. Might be okay if we infer from research tag? There's a folder "ricerca/" in taxonomy. But we don't have specific project names. We could still list a project like "llm-research-eagle-mtp" with slug. But we need to ensure it's derived from project names (lowercase, hyphens). Since we don't have explicit name, maybe we should not invent. Better to stick to actual listed projects.

Thus LLM Research section can include projects like "add-video-input-support-to-llamacpp-mtmd", "auto-quantization-pipeline-gguf", "auto-tuning-dinamico-per-gemma-4-26b-su-p40", maybe "ai-model-selector-physical-controller" (though that's more hardware). Also "ai-gateway-in-prod-alternative-concrete-a-litellm" maybe infrastructure.

AI Infrastructure: llm-stack (mentioned in taxonomy), ai-home-assistant-hid-dashboard, ai-dashboard, maybe ai-gateway-in-prod-alternative-concrete-a-litellm.

Tools & Automation: auto-vault-journal, voice-dictate, blender-3d-generation? maybe that's more creative. Also barocco-digital (website). Also ai-influencer.

Embedded & Hardware: ai-home-assistant-hid-dashboard (also embedded), ai-model-selector-physical-controller, voice-dictate? maybe not. Also maybe "blender-3d-generation" not embedded. We'll put hardware.

We need to keep each project entry as "[name](https://github.com/chessarisilvio/slug)" plus one-line description.

We need to ensure we don't exceed emojis: only header can have up to 2 emojis.

Let's craft.

First line: maybe:

<div align="center">
# Silvio Chessari 🚀🔧
...

But that's 2 emojis.

Then bio lines: maybe three lines:

> LLM inference researcher | AI systems engineer | Embedded hardware tinkerer  
> Specialize in EAGLE/MTP speculative decoding, MoE routing, and running LLMs on Tesla P40 (sm_61) via CUDA workarounds  
> Builder of self‑hosted AI infrastructure on consumer GPUs and open‑source toolchains

That's three lines.

Then compact stack table: maybe a table with Languages, Frameworks, Hardware.

We'll do:

| Category | Tech |
|----------|------|
| Languages | C++, Python, Rust, Bash |
| Frameworks | llama.cpp, ComfyUI, Astro, Tailwind, MQTT, Tailscale |
| Hardware | NVIDIA Tesla P40 (sm_61), RTX 3050, Arduino R4 WiFi, ESP32, GGUF quantized models |

That's a compact table.

Now sections.

We'll need to create headings: maybe `## LLM Research`, etc.

Under each heading, list items like:

- [add-video-input-support-to-llamacpp-mtmd](https://github.com/chessarisilvio/add-video-input-support-to-llamacpp-mtmd) – Enables webcam/video frame ingestion for llama.cpp inference pipelines.

We need to ensure slug matches project name lowercased with hyphens. The project name as given: "add-video-input-support-to-llamacpp-mtmd" already matches. Good.

Similarly "auto-quantization-pipeline-gguf".

"auto-tuning-dinamico-per-gemma-4-26b-su-p40" (note includes accent? we keep as is but slug should be lowercase hyphens; it's already lower case and hyphens, but includes accent? Actually "dinamico" no accent, "per", "gemma-4-26b-su-p40". It's fine.

"ai-model-selector-physical-controller".

"ai-home-assistant-hid-dashboard".

"ai-dashboard".

"ai-gateway-in-prod-alternative-concrete-a-litellm".

"blender-3d-generation".

"barocco-digital".

"ai-influencer".

"auto-vault-journal".

"voice-dictate".

We need to allocate to sections.

Let's decide:

LLM Research:
- add-video-input-support-to-llamacpp-mtmd
- auto-quantization-pipeline-gguf
- auto-tuning-dinamico-per-gemma-4-26b-su-p40
- ai-model-selector-physical-controller (maybe borderline but okay)

AI Infrastructure:
- llm-stack (not a specific repo? but we can infer slug "llm-stack")
- ai-home-assistant-hid-dashboard
- ai-dashboard
- ai-gateway-in-prod-alternative-concrete-a-litellm

Tools & Automation:
- auto-vault-journal
- voice-dictate
- blender-3d-generation
- barocco-digital

Embedded & Hardware:
- ai-home-assistant-hid-dashboard (already used) maybe move to embedded; but we can't duplicate. Let's decide: AI Infrastructure includes llm-stack, ai-dashboard, ai-gateway... Embedded & Hardware includes ai-home-assistant-hid-dashboard, ai-model-selector-physical-controller (maybe), voice-dictate? Actually voice-dictate is a tool. We'll keep embedded separate.

We need 4 sections exactly: LLM Research / AI Infrastructure / Tools & Automation / Embedded & Hardware.

Thus allocate:

LLM Research: as above.

AI Infrastructure: llm-stack, ai-dashboard, ai-gateway-in-prod-alternative-concrete-a-litellm, maybe ai-home-assistant-hid-dashboard? but that is more embedded. Let's put ai-home-assistant-hid-dashboard in Embedded & Hardware.

Thus AI Infrastructure: llm-stack, ai-dashboard, ai-gateway-in-prod-alternative-concrete-a-litellm, maybe something else like "ai-influencer"? No that's tools. We'll just have three? Need maybe four items each section? Not required but we can have variable.

Tools & Automation: auto-vault-journal, voice-dictate, blender-3d-generation, barocco-digital, ai-influencer.

Embedded & Hardware: ai-home-assistant-hid-dashboard, ai-model-selector-physical-controller, maybe also something like "blender-3d-generation"? No.

We need to ensure each project appears only once.

Let's list all projects we will include:

LLM Research:
- add-video-input-support-to-llamacpp-mtmd
- auto-quantization-pipeline-gguf
- auto-tuning-dinamico-per-gemma-4-26b-su-p40
- ai-model-selector-physical-controller (maybe but it's hardware; maybe move to embedded. Let's keep it in embedded.)

Better: LLM Research: add-video-input-support-to-llamacpp-mtmd, auto-quantization-pipeline-gguf, auto-tuning-dinamico-per-gemma-4-26b-su-p40.

AI Infrastructure: llm-stack, ai-dashboard, ai-gateway-in-prod-alternative-concrete-a-litellm.

Tools & Automation: auto-vault-journal, voice-dictate, blender-3d-generation, barocco-digital, ai-influencer.

Embedded & Hardware: ai-home-assistant-hid-dashboard, ai-model-selector-physical-controller.

That covers all.

Now we need to ensure we have real technical details from vault for each description.

Let's extract details:

- add-video-input-support-to-llamacpp-mtmd: from vault: "Add video input support to llama.cpp (mtmd)". Objective: adding video input support to llama.cpp, enabling acquisition of frames from webcam or video file and sending to server for LLM inference. Provides CMake modifications, stub of video input, example Python script.

- auto-quantization-pipeline-gguf: pipeline to download new LLM checkpoints, run benchmarks on local hardware (Tesla P40 and RTX 3050), evaluate best GGUF quantization point (Q4_K_M vs Q5_K_S), generate GGUF files ready for production, update vault docs.

- auto-tuning-dinamico-per-gemma-4-26b-su-p40: tool for dynamic auto-tuning monitoring VRAM and CPU of Tesla P40 during Gemma-4-26B-A4B-heretic execution, adapting GPU_LAYERS, CTX_SIZE, batch size to maximize throughput without OOM. Includes monitor module src/monitor.py collecting