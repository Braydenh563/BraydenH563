<div align="center">

# Brayden Hoyle

**CS × Interaction Design · QUT · Brisbane, Australia**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Brayden%20Hoyle-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/braydenh563/)
[![Instagram](https://img.shields.io/badge/Photography-@braydenhphotography-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/braydenhphotography/)
[![HuggingFace](https://img.shields.io/badge/HuggingFace-braydenh563-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)](https://huggingface.co/braydenh563)

</div>

---

I build software that sits at the intersection of code and design - from interactive creative-coding projects to practical tools and experiments, always with an eye on how something actually feels to use.

Third-year CS + Interaction Design student at QUT, where I try to make sure the software I write is as considered to use as it is technically interesting to build.

Most of what lives here spans creative coding, applied AI, and interface-driven projects: things built to actually be used, not just to demonstrate that they can exist.

---

## 🚀 Projects

<div align="center">

### 🧠 [MemoryMap AI](https://github.com/Braydenh563/MemoryMap-AI)

[![Latest release](https://img.shields.io/github/v/release/Braydenh563/MemoryMap-AI?style=flat-square&label=release)](https://github.com/Braydenh563/MemoryMap-AI/releases/latest)
[![Tests](https://img.shields.io/badge/tests-4%2C000%2B%20offline-2ea44f?style=flat-square)](https://github.com/Braydenh563/MemoryMap-AI/tree/main/tests)
[![Offline](https://img.shields.io/badge/100%25-offline-111827?style=flat-square)](https://github.com/Braydenh563/MemoryMap-AI#the-ai-and-life-without-it)
[![Licence](https://img.shields.io/badge/licence-AGPL--3.0-blue?style=flat-square)](https://github.com/Braydenh563/MemoryMap-AI/blob/main/LICENSE)

<a href="https://github.com/Braydenh563/MemoryMap-AI">
<img src="https://raw.githubusercontent.com/Braydenh563/MemoryMap-AI/main/docs/screenshots/graph.png" width="720" alt="MemoryMap AI: the knowledge graph, notes as glowing nodes linked by meaning" />
</a>

<sub>The Graph: every note as a node, linked by meaning, with the reason for each link written down.</sub>

**A local-first notebook with a local AI librarian.** You type a thought and the AI files it. You ask a question in plain English and get a conversational answer *and* the notes behind it, side by side, each sentence linked to the note it came from. The whole thing runs on your own machine: no account, no cloud, no telemetry, and it keeps working with no model installed at all.

</div>

**What makes it different**

- 🗺️ **Your notes as a map.** A force-directed graph coloured by category and linked by meaning; a timeline of everything by when it happened; a dashboard with your streak, digest and widgets.
- 🤖 **An agent that acts, and shows its work.** 58 tools to search, link, tag, remind, organise and place cards on a board; every step visible; anything destructive asks first. 20 built-in skills run multi-step jobs as a checklist.
- ✍️ **Long-form writing and a canvas.** A Markdown document editor with live view, version history and AI edits as diffs; a whiteboard for sketches, shapes and note cards that can become a mind map grown from your notes.
- 📚 **One Library for everything.** Notes, documents, chats, files, tags and the recycle bin. Every image read three ways: a caption, a vision-model transcription and OCR, all searchable. PDFs, spreadsheets and code imported with their text.
- 🧭 **Atlas.** An in-app guide that answers "how do I" from the app's own documentation, never from your notes.
- 🔐 **Private by construction.** Localhost only, no CDN assets, notes in a plain SQLite file, private notes encrypted at rest, web search opt-in and query-only.
- 🎨 **Designed, not assembled.** One design system enforced by lints; ten themes over colour palettes; responsive from a phone to a desktop; a packaged Windows installer and Linux build.

<details>
<summary><b>Under the hood</b></summary>

<br>

**Stack:** FastAPI · SQLAlchemy · SQLite · vanilla JS (no framework, no build step) · CodeMirror 6 for documents · a canvas graph renderer with a layout worker · Ollama or any OpenAI-compatible server (LM Studio, llama.cpp, Jan, vLLM) · `BAAI/bge-small-en-v1.5` for local semantic search · local Whisper dictation · Tesseract OCR

**Engineering:** 4,000+ pytest tests, all offline with every AI call faked · Playwright sweeps that measure the interface (console errors, contrast, touch targets, dock grammar) in both themes at four widths · CodeQL on every push · a release workflow that starts the packaged app before it publishes it

**Built with AI, deliberately.** MemoryMap was developed in collaboration with Claude (Claude Code) as an experiment in how far an AI-assisted solo project can go when the design decisions, the tests and the measurements stay human-owned. About 1,300 commits went into the 0.3.0 release alone.

**Models that work well** (`ollama pull <model>`): `llama3.2` · `granite4.1:3b` · `qwen3.5:2b` · `gemma4:e2b`

</details>

---

<div align="center">

### 🧬 [HELIXLABS](https://github.com/Braydenh563/HELIXLABS) - Microbiome Simulation

[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen?style=flat-square)](https://braydenh563.github.io/HELIXLABS/)
[![Download](https://img.shields.io/badge/download-v1.1.0-blue?style=flat-square)](https://github.com/Braydenh563/HELIXLABS/releases/tag/v1.1.0)

<a href="https://braydenh563.github.io/HELIXLABS/">
<img src="https://raw.githubusercontent.com/Braydenh563/HELIXLABS/main/metadata/HELIXLABS_Thumbnail.png" width="720" alt="HELIXLABS" />
</a>

An interactive microbiome simulator built with p5.js. Sequence alien base proteins to synthesise unique organisms, introduce them into a living petri-dish ecosystem, and watch emergent species behaviour unfold in real time - competing, coexisting, and evolving.

</div>

Started as the final assessment for QUT's DXB211 Creative Coding unit. Became one of my largest projects to date and was exhibited publicly at **The Lanes, Fortitude Valley, Brisbane (July 2026)** as part of QUT's Creative Coding exhibition, and also shown at the **Queensland Games Festival (June 2026)**.


> 🏆 Won the **DXB211 Tutor's Prize** for Creative Coding.

<details>
<summary><b>Features & technical details</b></summary>

<br>

**Core mechanics**
- **Procedural species generation** - 26 alien base proteins combine via `NodeClass.js` to produce organisms with distinct traits; no two sequences behave identically
- **Ecosystem simulation** - species interact, compete, and coexist dynamically; behaviour is fully determined by DNA sequence
- **Click & drag interaction** - physically move individual organisms around the environment
- **Randomise function** - instant random DNA sequence for quick experimentation

**UI & audio**
- **Species Index** - in-simulation encyclopedia cataloguing every species introduced
- **Ambient audio engine** - custom `BackgroundAmbienceManager.js` dynamically layers sound based on simulation state
- **Tutorial & hint popups** - built-in guided walkthrough for first-time players
- **FPS performance overlay** - real-time monitoring
- **Custom notification system** - via `Notification.js`

**Stack:** JavaScript · p5.js · p5.sound · GitHub Pages (auto-deploy via Actions)

**Controls**

| Input | Action |
|---|---|
| Type letters (A–Z) | Define your DNA sequence |
| Click environment | Spawn and introduce your species |
| Click & drag | Move individual organisms |
| Randomise button | Generate a surprise sequence |

**Platform support:** PC/Laptop (Windows & Linux)

</details>

---

### 🎨 [BH Creative Coding](https://github.com/Braydenh563/BH-CreativeCoding)

Generative and interactive visual experiments built with p5.js - animation, colour, form, and interactivity. Feeding into a planned personal portfolio site.

---

### 🤖 [Astraea - Prompt Architect](https://chatgpt.com/g/g-68ad0fff3c108191a9b9b05cd2e20584-astraea-prompt-architect)

A specialised AI agent for turning rough ideas into production-ready prompts - routing structured output across ChatGPT, Claude, Gemini, Midjourney, DALL·E, Sora, and more.

<details>
<summary><b>Fine-tuning & system design details</b></summary>

<br>

**System design**
- Three modes: `DUAL` · `PROMPT-ONLY` · `ADVICE-ONLY`
- Three complexity tiers: `BASIC` · `STANDARD` · `EXPERT`
- 4D build process: Deconstruct → Diagnose → Develop → Deliver
- 7D rewrite framework, Prompt Linter, Mini QA Gate, Assumption Ledger, output Scorecard

**Fine-tuning**
- Base: `Meta-Llama-3.1-8B-Instruct` (4-bit quantised via [Unsloth](https://github.com/unslothai/unsloth))
- Trained with HuggingFace TRL `SFTTrainer` on Google Colab (NVIDIA A100)
- LoRA: `r=64`, `lora_alpha=128`, RSLoRA - `q/k/v/o/gate/up/down_proj`
- v10: ~2,693 training examples, refined with Claude Sonnet 4.5 / 4.6
- Exported as GGUF `q4_k_m` for local inference via llama.cpp · Ollama · Open WebUI · Jan

</details>

---

### *(Upcoming - University)*

- **🗞️ News Accuracy Checker** - Python tool for evaluating factual accuracy of news articles
- **🏥 Hospital Management System** - C# system covering patient management, scheduling, and admin workflows
- **🌐 Personal Portfolio** - p5.js creative graphics + photography + design work

---

## 🛠️ Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![HTML/CSS](https://img.shields.io/badge/HTML%2FCSS-E34F26?style=flat-square&logo=html5&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![P5.js](https://img.shields.io/badge/P5.js-ED225D?style=flat-square&logo=p5dotjs&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![Assembly](https://img.shields.io/badge/Assembly-6E4C13?style=flat-square&logoColor=white)
![VB.NET](https://img.shields.io/badge/VB.NET-512BD4?style=flat-square&logo=.net&logoColor=white)

**AI / ML**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logoColor=white)
![Google Colab](https://img.shields.io/badge/Colab-F9AB00?style=flat-square&logo=googlecolab&logoColor=black)
![Claude Code](https://img.shields.io/badge/Claude%20Code-D97757?style=flat-square&logoColor=white)

LoRA / SFT fine-tuning · GGUF quantisation · Local LLM deployment · Unsloth · llama.cpp · Agentic workflows · AI-assisted engineering with tests and measurements as the gate

**Backend & tooling**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
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

**QUT - 2024–2027**
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
| 3 | 2 | CAB432 | Cloud Computing |
| 3 | 2 | DXB212 | Tangible Interaction Design |
| 3 | 2 | DXB111 | Introduction to Web Design |
| 3 | 2 | DYB102 | Impact Lab: Society and Systems |

</details>

**Coomera Anglican College - 2009–2023**
Year 12 Graduate · Mathematical Methods · Digital Solutions · Design · Film, TV & New Media · Chemistry

---

## 🏅 Awards

| Award | Issued by | Date |
|-------|-----------|------|
| 🏆 Executive Dean's Commendation for Academic Excellence | QUT - Faculty of Creative Industries, Education, and Social Justice | Jul 2026 |
| 🏆 DXB211 Creative Coding Tutor's Prize | QUT - Bachelor of Interaction Design | Jul 2026 |
| 🏆 Executive Dean's Commendation for Academic Excellence | QUT - Faculty of Science | Jul 2024 |
| 🥈 Duke of Edinburgh Silver Award | Duke of Edinburgh's International Award | 2023 |
| 🥉 Duke of Edinburgh Bronze Award | Duke of Edinburgh's International Award | 2021 |

---

## 🔐 Other

- Completed a national **Cyber Security Work Experience Program** (2023) - selected alongside participants from across Australia
- Member: **AISA** (Australian Information Security Association) · **ACS** (Australian Computer Society)
- **Associate**, Topgolf Gold Coast *(Jun 2024 – Present)*

---

<div align="center">

*Open to internships and collaborations in AI, software, and design.*

[![LinkedIn](https://img.shields.io/badge/Let's%20connect-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/braydenh563/)

</div>
</content>
