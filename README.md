<div align="center">

# Brayden Hoyle

**CS × Interaction Design · QUT · South East Queensland**

*Building things that are technically interesting and thoughtfully crafted — at the intersection of AI, software, and human-centred design.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Brayden%20Hoyle-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/brayden-hoyle-341106240)
[![Instagram](https://img.shields.io/badge/Photography-@braydenhphotography-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/braydenhphotography/)
[![GitHub](https://img.shields.io/badge/GitHub-Braydenh563-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Braydenh563)

</div>

---

> 🏆 **QUT Executive Dean's Commendation for Academic Excellence** — Faculty of Science, July 2024. Awarded for achieving a GPA of 6.5+ across Year 1 Semester 1.

---

## About

I'm a third-year Computer Science student concurrently studying Interaction Design at QUT — two disciplines that push and pull each other in ways I find genuinely energising. On the CS side, I'm drawn to AI/ML systems, fine-tuning pipelines, and software architecture. On the design side, I care about what it actually feels like to use the things I build.

Most of my personal projects live somewhere in between: local-first AI tools, creative coding experiments, and systems designed to remove friction for non-technical users.

Open to internships and collaborations in **AI, software development, and design**.

---

## 🎓 Education

### Queensland University of Technology — 2024–2027
**Bachelor of Information Technology (Computer Science)**
**Bachelor of Design (Interaction Design)**

<details>
<summary>View full coursework</summary>

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
| 2 | 2 | CAB202 | Microcontrollers & Digital Systems |
| 2 | 2 | DYB122 | Design Visualisations |
| 2 | 2 | DYB123 | Emerging Design Technologies |
| 2 | 2 | DYB124 | Design Consequences |

</details>

### Coomera Anglican College — 2009–2023
**Year 12 Graduate**

Mathematical Methods · General English · Digital Solutions · Design · Film, TV & New Media · Chemistry

Produced films and digital applications through Film/TV/New Media and Digital Solutions — where a genuine interest in making things started.

---

## 🚀 Projects

### 🤖 [Astraea — Prompt Architect](https://chatgpt.com/g/g-68ad0fff3c108191a9b9b05cd2e20584-astraea-prompt-architect)

A specialised AI agent that turns rough ideas into production-ready prompts for text, image, video, and code — routing structured output to ChatGPT, Claude, Gemini, Midjourney, DALL·E, Sora, and more.

<details>
<summary>System design & fine-tuning details</summary>

**System Design**
- Three operating modes: `DUAL` (quick answer + full prompt), `PROMPT-ONLY`, `ADVICE-ONLY`
- Three complexity tiers: `BASIC` · `STANDARD` · `EXPERT`
- 4D build process: Deconstruct → Diagnose → Develop → Deliver
- 7D rewrite framework, built-in Prompt Linter, Mini QA Gate, Assumption Ledger, and output Scorecard

**Fine-Tuning Pipeline**
- Base model: `Meta-Llama-3.1-8B-Instruct` (4-bit quantised via [Unsloth](https://github.com/unslothai/unsloth))
- Trained with HuggingFace TRL `SFTTrainer` on Google Colab (NVIDIA A100)
- LoRA: `r=64`, `lora_alpha=128`, RSLoRA — targeting `q/k/v/o/gate/up/down_proj`
- v10 (latest): ~2,693 training examples, refined using Claude Sonnet 4.5 / 4.6
- Exported as GGUF `q4_k_m` for local inference via llama.cpp, Ollama, Open WebUI, Jan
- Accompanied by a Python backend and HTML/CSS frontend (built as a hands-on learning exercise)

</details>

---

### 🧠 MemoryMap AI *(In Development)*

A local-first AI application with models bundled directly — no Ollama, LMStudio, or external setup required for end users.

- Researching RAG vs. Text-to-SQL for database access architecture
- Exploring fine-tuned models for specialised data retrieval
- Designing an interface that removes AI configuration friction entirely for non-technical users

---

### 🎨 [BH Creative Coding](https://github.com/Braydenh563/BH-CreativeCoding)

Generative and interactive visual experiments built with P5.js — exploring animation, colour, form, and interactivity. Feeding into a planned personal portfolio website.

---

### 🗞️ News Accuracy Checker *(Upcoming — University)*
Python-based application for evaluating the factual accuracy of news articles.

### 🏥 Hospital Management System *(Upcoming — University)*
C# system covering patient management, scheduling, and administrative workflows.

### 🌐 Personal Portfolio *(Planned)*
A digital portfolio integrating P5.js-inspired creative graphics alongside photography and design work.

---

## 🛠️ Skills & Tools

**Languages**

![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![Assembly](https://img.shields.io/badge/Assembly-6E4C13?style=flat-square&logoColor=white)
![Visual Basic](https://img.shields.io/badge/Visual%20Basic-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![P5.js](https://img.shields.io/badge/P5.js-ED225D?style=flat-square&logo=p5dotjs&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![HTML/CSS](https://img.shields.io/badge/HTML%2FCSS-E34F26?style=flat-square&logo=html5&logoColor=white)

**AI / ML**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Google Colab](https://img.shields.io/badge/Colab-F9AB00?style=flat-square&logo=googlecolab&logoColor=black)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logoColor=white)

Model fine-tuning (LoRA / SFT) · GGUF quantisation · Local LLM deployment · Unsloth · llama.cpp

**Systems & Hardware**

![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

**Platforms & Tools**

![Salesforce](https://img.shields.io/badge/Salesforce%20Flows-00A1E0?style=flat-square&logo=salesforce&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)
![Visual Studio](https://img.shields.io/badge/Visual%20Studio%202022-5C2D91?style=flat-square&logo=visualstudio&logoColor=white)
![IntelliJ IDEA](https://img.shields.io/badge/IntelliJ%20IDEA-000000?style=flat-square&logo=intellijidea&logoColor=white)

**Concepts & Practices**

Sorting & search algorithms · Hash tables & data structures · Object-relational mapping · Networking fundamentals · Database design · Cyber security principles · Discrete mathematics · Software engineering practices

---

## 🎨 Design & Creative Work

Studying Interaction Design at QUT — UX/UI principles, systems thinking, and human-centred design. Design experience from high school runs deeper than it sounds: Digital Solutions and Design subjects meant shipping actual things, not just sketching them.

**Adobe Creative Suite**

![Premiere Pro](https://img.shields.io/badge/Premiere%20Pro-9999FF?style=flat-square&logo=adobepremierepro&logoColor=white)
![Photoshop](https://img.shields.io/badge/Photoshop-31A8FF?style=flat-square&logo=adobephotoshop&logoColor=white)
![Illustrator](https://img.shields.io/badge/Illustrator-FF9A00?style=flat-square&logo=adobeillustrator&logoColor=white)
![InDesign](https://img.shields.io/badge/InDesign-FF3366?style=flat-square&logo=adobeindesign&logoColor=white)

**Photography** — Canon EOS R50. Landscape, street, portrait, and creative work.
[![Instagram](https://img.shields.io/badge/@braydenhphotography-E4405F?style=flat-square&logo=instagram&logoColor=white)](https://www.instagram.com/braydenhphotography/)

---

## 🔐 Cyber Security

- Completed a national **Cyber Security Work Experience Program** (1 week, 2023) — selected alongside participants from across Australia
- Studied **IFB240 Cyber Security** at QUT
- Member: **Australian Information Security Association (AISA)**
- Member: **Australian Computer Society (ACS)**

---

## 🏅 Awards & Achievements

| Award | Issued by | Date |
|-------|-----------|------|
| 🏆 Executive Dean's Commendation for Academic Excellence | QUT — Faculty of Science | Jul 2024 |
| 🎖️ iLR Award *(Imagine, Listen, Respect)* — awarded annually to one graduating student | Coomera Anglican College | Nov 2023 |
| 🥈 Duke of Edinburgh Silver Award | Duke of Edinburgh's International Award | 2023 |
| 🥉 Duke of Edinburgh Bronze Award | Duke of Edinburgh's International Award | 2021 |
| 🎵 AHEP Program — Vocal Ensemble | Queensland Griffith Conservatorium of Music | 2023 |

---

## 💼 Experience

**Associate** — Topgolf Gold Coast *(Jun 2024 – Present)*
Bay host role focused on delivering memorable guest experiences.

**Student IT Assistant** — Coomera Anglican College IT Department *(Dec 2022)*
Set up new student laptops via Windows Autopilot; provided general IT support.

---

<div align="center">

*QUT · Brisbane, QLD · Open to internships and collaborations in AI, software, and design.*

[![LinkedIn](https://img.shields.io/badge/Let's%20connect-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/brayden-hoyle-341106240)

</div>
