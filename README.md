<div align="center">

# Brayden Hoyle

**CS × Interaction Design · QUT · Brisbane, Australia**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Brayden%20Hoyle-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/brayden-hoyle-341106240)
[![Instagram](https://img.shields.io/badge/Photography-@braydenhphotography-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/braydenhphotography/)
[![HuggingFace](https://img.shields.io/badge/HuggingFace-braydenh563-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)](https://huggingface.co/braydenh563)

</div>

---

I build AI-adjacent things — mostly local-first tools, generative experiments, and fine-tuned models.

I’m a third-year Computer Science + Interaction Design student at QUT, interested in building software that is both technically interesting and genuinely considered to use.

Most of what lives here sits at the intersection of AI/ML systems and human-facing design: things built to actually be used, not just to prove that they can exist.

---

## 🚀 Projects

### 🧠 [MemoryMap AI](https://github.com/Braydenh563/MemoryMap-AI) *(Active — Experimental)*

Local-first AI notebook where you type a thought, let a local LLM file it, and ask questions in plain English to get both an answer and the raw notes behind it.

100% offline. No account, no cloud, no telemetry. Your notes live in a plain SQLite file on your own machine.

> **Proof-of-concept** — largely vibe-coded in collaboration with Claude to rapidly explore what a genuinely private, local-AI-native notebook could feel like. The core ideas and architecture are deliberate; the speed of development was not.

<details>
<summary>What's inside</summary>

**Stack:** FastAPI backend · Vanilla JS frontend · SQLite · Ollama integration · `BAAI/bge-small-en-v1.5` for local semantic search

**Features across 6 tabs:**
- **Dashboard** — capture streak, AI weekly digest, activity heatmap, focus timer, rearrangeable layout
- **Notes** — auto-filing by meaning, tags, pins, threads, attachments, private encrypted notes, revision history, advanced search operators (`tag:`, `cat:`, `is:pinned`, `-exclude`, `"exact phrase"`)
- **Chat** — conversational access to your notebook with Agent mode and full tool-call timeline
- **Graph** — force-directed knowledge map with editable links and AI-suggested connections
- **Documents** — Markdown editor with live preview, PDF export, and AI-suggested edits shown as diffs
- **Reminders** — natural language scheduling

**Also:** command palette (`Ctrl/Cmd+K`), local Whisper dictation, read-aloud, opt-in web search with SearXNG support, themes and colour palettes, daily local backups, PWA, desktop window mode

**Privacy:** server binds to localhost, no CDN assets, and web search never sends note contents — only query terms

**Tests:** 547 pytest tests; AI calls are faked so the suite runs fully offline

</details>

**Models that work well with it:** `llama3.2` · `granite4.1:3b` · `qwen3.5:2b` · `gemma4:e2b` · `lfm2.5`

---

### 🧬 [HELIXLABS](https://github.com/Braydenh563/HELIXLABS) — Microbiome Simulation [![Live Demo](https://img.shields.io/badge/demo-live-brightgreen?style=flat-square)](https://braydenh563.github.io/HELIXLABS/)

Interactive microbiome simulator built with p5.js. Sequence alien base proteins to synthesise unique organisms, introduce them into a living petri-dish ecosystem, and watch emergent species behaviour unfold in real time.

Originally developed as the final assessment for QUT’s DXB211 Creative Coding unit, then exhibited publicly at **The Lanes, Fortitude Valley, Brisbane (July 2026)** as part of QUT’s Creative Coding exhibition and shown at the **Queensland Games Festival (June 2026)**.

> Won the **DXB211 Tutor’s Prize** for Creative Coding.

<details>
<summary>Features & technical details</summary>

**Core mechanics:**
- **Procedural species generation** — 26 alien base proteins combine to produce organisms with distinct traits
- **Ecosystem simulation** — species compete, coexist, and evolve dynamically
- **Direct interaction** — click and drag individual organisms around the environment
- **Randomise function** — instant random DNA sequence for experimentation

**UI & audio:**
- **Species Index** — in-simulation encyclopedia cataloguing introduced species
- **Ambient audio engine** — custom dynamic sound layering based on simulation state
- **Tutorial & hint popups** — guided onboarding for first-time players
- **FPS overlay** — real-time performance monitoring
- **Notification system** — custom in-app alerts

**Stack:** JavaScript · p5.js · p5.sound · GitHub Pages

**Controls:**
- Type letters `A–Z` to define a DNA sequence
- Click the environment to spawn and introduce a species
- Click and drag to move organisms
- Use the randomise button to generate a surprise sequence

**Platform support:** PC/Laptop (Windows & Linux) · Mac users should use the hosted web version  
[Download v1.1.0](https://github.com/Braydenh563/HELIXLABS/releases/tag/v1.1.0)

</details>

---

### 🎨 [BH Creative Coding](https://github.com/Braydenh563/BH-CreativeCoding)

Generative and interactive visual experiments built with p5.js — animation, colour, form, and interactivity.

This work feeds into a planned personal portfolio site spanning creative coding, design, and photography.

---

### 🤖 [Astraea — Prompt Architect](https://chatgpt.com/g/g-68ad0fff3c108191a9b9b05cd2e20584-astraea-prompt-architect)

Specialised AI agent for turning rough ideas into production-ready prompts across ChatGPT, Claude, Gemini, Midjourney, DALL·E, Sora, and more.

Built alongside a fine-tuning pipeline focused on prompt structure, rewrite quality, and reliable multi-model output formatting.

<details>
<summary>Fine-tuning & system design details</summary>

**System design**
- Three modes: `DUAL` · `PROMPT-ONLY` · `ADVICE-ONLY`
- Three complexity tiers: `BASIC` · `STANDARD` · `EXPERT`
- 4D process: Deconstruct → Diagnose → Develop → Deliver
- Prompt Linter, Mini QA Gate, Assumption Ledger, and output Scorecard

**Fine-tuning**
- Base: `Meta-Llama-3.1-8B-Instruct` (4-bit quantised via [Unsloth](https://github.com/unslothai/unsloth))
- Trained with HuggingFace TRL `SFTTrainer` on Google Colab (NVIDIA A100)
- LoRA: `r=64`, `lora_alpha=128`, RSLoRA across major projection layers
- v10 trained on ~2,693 examples
- Exported as GGUF `q4_k_m` for local inference via llama.cpp, Ollama, Open WebUI, and Jan

</details>

---

### 📚 Upcoming

- **🗞️ News Accuracy Checker** — Python tool for evaluating factual accuracy of news articles
- **🏥 Hospital Management System** — C# system covering patient management, scheduling, and admin workflows
- **🌐 Personal Portfolio** — creative coding, photography, and design work in one site

---

## 🛠️ Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![HTML/CSS](https://img.shields.io/badge/HTML%2FCSS-E34F26?style=flat-square&logo=html5&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![P5.js](https://img.shields.io/badge/P5.js-ED225D?style=flat-square&logo=p5dotjs&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![Assembly](https://img.shields.io/badge/Assembly-6E4C13?style=flat-square&logoColor=white)

**AI / ML**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logoColor=white)
![Google Colab](https://img.shields.io/badge/Colab-F9AB00?style=flat-square&logo=googlecolab&logoColor=black)

LoRA / SFT fine-tuning · GGUF quantisation · Local LLM deployment · Unsloth · llama.cpp · Agentic workflows

**Tools & Platforms**

![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Salesforce](https://img.shields.io/badge/Salesforce%20Flows-00A1E0?style=flat-square&logo=salesforce&logoColor=white)

**Design**

![Premiere Pro](https://img.shields.io/badge/Premiere%20Pro-9999FF?style=flat-square&logo=adobepremierepro&logoColor=white)
![Photoshop](https://img.shields.io/badge/Photoshop-31A8FF?style=flat-square&logo=adobephotoshop&logoColor=white)
![Illustrator](https://img.shields.io/badge/Illustrator-FF9A00?style=flat-square&logo=adobeillustrator&logoColor=white)
![InDesign](https://img.shields.io/badge/InDesign-FF3366?style=flat-square&logo=adobeindesign&logoColor=white)

Canon EOS R50 · Landscape, street, portrait, and creative photography  
[![Instagram](https://img.shields.io/badge/@braydenhphotography-E4405F?style=flat-square&logo=instagram&logoColor=white)](https://www.instagram.com/braydenhphotography/)

---

## 🎓 Education

**QUT — 2024–2027**  
Bachelor of Information Technology (Computer Science) / Bachelor of Design (Interaction Design)

<details>
<summary>Full coursework</summary>

| Year | Sem | Code | Unit |
|:----:|:---:|------|------|
| 1 | 1 | IFB102 | Introduction to Computer Systems |
| 1 | 1 | IFB103 | IT Systems Design |
| 1 | 1 | IFB104 | Building IT Systems |
| 1 | 1 | IFB105 | Database Management |
| 1 | 2 | CAB201 | Programming Principles |
| 1 | 2 | CAB222 | Networks |
| 1 | 2 | IFB240 | Cyber Security |
| 1 | 2 | QUT009 | Data Science for Society |
| 1 | 2 | QUT010 | People with Robots |
| 2 | 1 | IFB201 | Introduction to Enterprise Systems |
| 2 | 1 | CAB203 | Discrete Structures |
| 2 | 1 | CAB302 | Software Development |
| 2 | 1 | QUT008 | Thinking Like a Computer |
| 2 | 1 | QUT001 | Artificial Intelligence in the Real World |
| 2 | 2 | EGB202 | Microcontrollers & Digital Systems |
| 2 | 2 | DYB122 | Design Visualisations |
| 2 | 2 | DYB123 | Emerging Design Technologies |
| 2 | 2 | DYB124 | Design Consequences |
| 3 | 1 | CAB301 | Algorithms & Complexity |
| 3 | 1 | DXB211 | Creative Coding |
| 3 | 1 | DYB121 | Introduction to Design Fabrication |
| 3 | 1 | DYB101 | Impact Lab: Place and Context |

</details>

**Coomera Anglican College — 2009–2023**  
Year 12 Graduate · Mathematical Methods · Digital Solutions · Design · Film, TV & New Media · Chemistry

---

## 🏅 Awards

| Award | Issued by | Date |
|-------|-----------|------|
| 🏆 DXB211 Creative Coding Tutor’s Prize | QUT — Bachelor of Interaction Design | Jul 2026 |
| 🏆 Executive Dean’s Commendation for Academic Excellence | QUT — Faculty of Science | Jul 2024 |
| 🥈 Duke of Edinburgh Silver Award | Duke of Edinburgh’s International Award | 2023 |
| 🥉 Duke of Edinburgh Bronze Award | Duke of Edinburgh’s International Award | 2021 |

---

## 🔐 Other

- Completed a national **Cyber Security Work Experience Program** (2023) — selected alongside participants from across Australia
- Member: **AISA** (Australian Information Security Association) · **ACS** (Australian Computer Society)
- **Associate**, Topgolf Gold Coast *(Jun 2024 – Present)*

---

<div align="center">

*Open to internships and collaborations in AI, software, and design.*

[![LinkedIn](https://img.shields.io/badge/Let's%20connect-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/brayden-hoyle-341106240)

</div>
