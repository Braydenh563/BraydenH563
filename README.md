<div align="center">

# Brayden Hoyle

**Computer Science + Interaction Design at QUT · Brisbane, Australia**

I design and build software people actually want to use: local-first AI tools, interactive simulations and creative-coding work.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Brayden%20Hoyle-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/braydenh563/)
[![Photography](https://img.shields.io/badge/Photography-@braydenhphotography-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/braydenhphotography/)
[![Hugging Face](https://img.shields.io/badge/Hugging%20Face-braydenh563-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)](https://huggingface.co/braydenh563)

</div>

---

### Right now

- Shipping **MemoryMap AI**, a local-first AI notebook with tested Windows and Linux releases
- Third year of a double degree: Computer Science and Interaction Design at QUT
- Open to internships in software engineering, applied AI and product design

---

## Featured work

### [MemoryMap AI](https://github.com/Braydenh563/MemoryMap-AI)

**A notebook that files itself. Local AI, your machine, nothing sent anywhere.**

[![Latest release](https://img.shields.io/github/v/release/Braydenh563/MemoryMap-AI?style=flat-square&label=release)](https://github.com/Braydenh563/MemoryMap-AI/releases/latest)
[![CI](https://github.com/Braydenh563/MemoryMap-AI/actions/workflows/ci.yml/badge.svg)](https://github.com/Braydenh563/MemoryMap-AI/actions/workflows/ci.yml)
[![Tests](https://img.shields.io/badge/tests-9%2C000%2B-2ea44f?style=flat-square)](https://github.com/Braydenh563/MemoryMap-AI/tree/main/tests)
[![Offline](https://img.shields.io/badge/runs-100%25%20offline-111827?style=flat-square)](https://github.com/Braydenh563/MemoryMap-AI#privacy)
[![Website](https://img.shields.io/badge/website-memorymap-4c8bf5?style=flat-square)](https://braydenh563.github.io/MemoryMap-AI/)

<a href="https://github.com/Braydenh563/MemoryMap-AI">
<img src="https://raw.githubusercontent.com/Braydenh563/MemoryMap-AI/main/docs/screenshots/graph.png" width="760" alt="MemoryMap AI's graph view: notes drawn as a map, coloured by category and linked by meaning" />
</a>

Type a thought and a local model files it, tags it and links it to what you already wrote. Ask a question later and get an answer with every sentence cited to the note it came from. It runs entirely on your machine: no account, no cloud, no telemetry, and it still works with no model installed.

- **Files itself, honestly.** A category, tags and links for every note, with a certainty that never claims 100%.
- **Answers you can check.** Ask in plain English; each sentence links to its source note.
- **An agent that shows its work.** 65 tools and 21 multi-step skills, every step visible, anything destructive asks first.
- **More than notes.** A document editor, whiteboards, mind maps, a knowledge graph, a timeline and reminders in one app.
- **Private by construction.** One SQLite file, encrypted private notes, HTTPS for other devices, and no network use until you allow it.

<details>
<summary><b>How it's built</b></summary>

<br>

**Stack:** Python · FastAPI · SQLAlchemy · SQLite · vanilla JavaScript (no framework, no build step) · CodeMirror 6 · D3 · Ollama or any OpenAI-compatible local server · local Whisper and OCR

**Engineering:** 9,000+ offline tests with every AI call faked · 49 end-to-end Playwright tests of the real flows on every push · interface sweeps that measure contrast, touch targets and layout at four widths in both themes · CodeQL on every push · a Windows installer that CI builds, installs, upgrades and uninstalls before release

**AI-assisted, human-owned.** Built with Claude Code over ~1,800 commits. I own the product, the design decisions and the bar: nothing ships until the tests and measurements say so.

</details>

---

### [HELIXLABS](https://github.com/Braydenh563/HELIXLABS): microbiome simulation

[![Live demo](https://img.shields.io/badge/demo-live-brightgreen?style=flat-square)](https://braydenh563.github.io/HELIXLABS/)
[![Download](https://img.shields.io/badge/download-v1.1.0-blue?style=flat-square)](https://github.com/Braydenh563/HELIXLABS/releases/tag/v1.1.0)

<a href="https://braydenh563.github.io/HELIXLABS/">
<img src="https://raw.githubusercontent.com/Braydenh563/HELIXLABS/main/metadata/HELIXLABS_Thumbnail.png" width="760" alt="HELIXLABS: organisms in a living petri dish" />
</a>

Sequence alien proteins into a DNA string, release the organism into a living petri dish, and watch species compete, coexist and evolve in real time. Built in p5.js.

- **Won the DXB211 Tutor's Prize** for Creative Coding at QUT
- **Exhibited** at QUT's Creative Coding exhibition, The Lanes, Fortitude Valley (July 2026), and at the Queensland Games Festival (June 2026)

<details>
<summary><b>Features and technical detail</b></summary>

<br>

- **Procedural species:** 26 base proteins combine into organisms with distinct traits; behaviour is set entirely by the sequence
- **Ecosystem simulation:** species interact, compete and coexist with emergent behaviour
- **Species Index:** an in-game encyclopedia of every species introduced
- **Adaptive ambient audio:** sound layered from the state of the simulation
- **Guided onboarding:** tutorial and hint popups, plus a performance overlay

| Input | Action |
|---|---|
| Type A to Z | Write the DNA sequence |
| Click the dish | Release your species |
| Click and drag | Move an organism |
| Randomise | Generate a surprise sequence |

**Stack:** JavaScript · p5.js · p5.sound · GitHub Pages via Actions · Windows and Linux

</details>

---

### [Astraea, prompt architect](https://chatgpt.com/g/g-68ad0fff3c108191a9b9b05cd2e20584-astraea-prompt-architect)

A specialised agent that turns rough ideas into production-ready prompts for ChatGPT, Claude, Gemini, Midjourney, DALL·E and Sora, backed by my own fine-tuned local model.

<details>
<summary><b>System design and fine-tuning</b></summary>

<br>

- **Modes:** dual, prompt-only and advice-only, across basic, standard and expert tiers
- **Pipeline:** deconstruct, diagnose, develop, deliver, with a prompt linter, a QA gate, an assumption ledger and a scorecard
- **Model:** Llama 3.1 8B Instruct, 4-bit via Unsloth, trained with Hugging Face TRL's SFTTrainer on an A100
- **LoRA:** r=64, alpha=128, RSLoRA on all attention and MLP projections; about 2,700 curated training examples
- **Deployment:** GGUF q4_k_m for local inference through llama.cpp, Ollama, Open WebUI and Jan

</details>

---

### [Creative coding](https://github.com/Braydenh563/BH-CreativeCoding)

Generative and interactive experiments in p5.js: animation, colour, form and interaction. The groundwork for a portfolio site that brings code, photography and design together.

**Next up:** a news accuracy checker (Python) · a hospital management system (C#) · the portfolio site

---

## Toolkit

**Languages**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![HTML/CSS](https://img.shields.io/badge/HTML%2FCSS-E34F26?style=flat-square&logo=html5&logoColor=white)
![p5.js](https://img.shields.io/badge/p5.js-ED225D?style=flat-square&logo=p5dotjs&logoColor=white)
![VB.NET](https://img.shields.io/badge/VB.NET-512BD4?style=flat-square&logo=.net&logoColor=white)
![Assembly](https://img.shields.io/badge/Assembly-6E4C13?style=flat-square&logoColor=white)

**AI and ML**
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logoColor=white)
![Colab](https://img.shields.io/badge/Colab-F9AB00?style=flat-square&logo=googlecolab&logoColor=black)
![Claude Code](https://img.shields.io/badge/Claude%20Code-D97757?style=flat-square&logoColor=white)
<br><sub>LoRA and SFT fine-tuning · GGUF quantisation · local LLM deployment · agentic workflows · evaluation-driven AI engineering</sub>

**Backend and tooling**
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white)
![Salesforce](https://img.shields.io/badge/Salesforce%20Flows-00A1E0?style=flat-square&logo=salesforce&logoColor=white)

**Design**
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white)
![Photoshop](https://img.shields.io/badge/Photoshop-31A8FF?style=flat-square&logo=adobephotoshop&logoColor=white)
![Illustrator](https://img.shields.io/badge/Illustrator-FF9A00?style=flat-square&logo=adobeillustrator&logoColor=white)
![InDesign](https://img.shields.io/badge/InDesign-FF3366?style=flat-square&logo=adobeindesign&logoColor=white)
![Premiere Pro](https://img.shields.io/badge/Premiere%20Pro-9999FF?style=flat-square&logo=adobepremierepro&logoColor=white)
<br><sub>Photography on a Canon EOS R50: landscape, street and portrait · <a href="https://www.instagram.com/braydenhphotography/">@braydenhphotography</a></sub>

---

## Recognition

| | | |
|---|---|---|
| Executive Dean's Commendation for Academic Excellence | QUT, Faculty of Creative Industries, Education and Social Justice | 2026 |
| DXB211 Creative Coding Tutor's Prize | QUT, Bachelor of Interaction Design | 2026 |
| Executive Dean's Commendation for Academic Excellence | QUT, Faculty of Science | 2024 |
| Duke of Edinburgh Silver Award | Duke of Edinburgh's International Award | 2023 |
| Duke of Edinburgh Bronze Award | Duke of Edinburgh's International Award | 2021 |

Selected for a national **Cyber Security Work Experience Program** (2023) · Member of **AISA** and the **ACS**

**Work:** Associate, Topgolf Gold Coast (June 2024 to present)

---

## Education

**Queensland University of Technology** · 2024 to 2027
Bachelor of Information Technology (Computer Science) / Bachelor of Design (Interaction Design)

<details>
<summary>Coursework</summary>

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
| 2 | 2 | EGB202 | Microcontrollers and Digital Systems |
| 2 | 2 | DYB122 | Design Visualisations |
| 2 | 2 | DYB123 | Emerging Design Technologies |
| 2 | 2 | DYB124 | Design Consequences |
| 3 | 1 | CAB301 | Algorithms and Complexity |
| 3 | 1 | DXB211 | Creative Coding |
| 3 | 1 | DYB121 | Introduction to Design Fabrication |
| 3 | 1 | DYB101 | Impact Lab: Place and Context |
| 3 | 2 | CAB432 | Cloud Computing |
| 3 | 2 | DXB212 | Tangible Interaction Design |
| 3 | 2 | DXB111 | Introduction to Web Design |
| 3 | 2 | DYB102 | Impact Lab: Society and Systems |

</details>

**Coomera Anglican College** · Graduated 2023
Mathematical Methods · Digital Solutions · Design · Film, TV and New Media · Chemistry

---

<div align="center">

**Open to internships and collaborations in software, applied AI and design.**

[![Let's connect](https://img.shields.io/badge/Let's%20connect-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/braydenh563/)

</div>
