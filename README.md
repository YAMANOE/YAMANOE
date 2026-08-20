<p align="center">
  <img alt="Yaman — AI Engineer, Amman, Jordan" src="https://capsule-render.vercel.app/api?type=waving&color=0:0A66C2,100:1F6FEB&height=190&section=header&text=Yaman&fontColor=ffffff&fontSize=62&desc=AI%20Engineer%20%C2%B7%20Amman,%20Jordan&descSize=17&descAlignY=68&animation=fadeIn" />
</p>

<p align="center">
  <img alt="Multi-agent systems that refuse to guess · Computer vision + Arabic NLP · Civic technology for the public sector · PostGIS · pgRouting · LLM agents" src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=21&duration=3200&pause=900&color=1F6FEB&center=true&vCenter=true&width=620&lines=Multi-agent+systems+that+refuse+to+guess;Computer+vision+%2B+Arabic+NLP;Civic+technology+for+the+public+sector;PostGIS+%C2%B7+pgRouting+%C2%B7+LLM+agents" />
</p>

<p align="center">
  <img alt="9xAI Program at HTU" src="https://img.shields.io/badge/9xAI%20Program-HTU-1F6FEB?style=flat-square" />
  <img alt="Works in Arabic and English" src="https://img.shields.io/badge/Arabic-%2F%20English-0A66C2?style=flat-square" />
</p>

<p align="center">
  <b>B.Sc. Data Science &amp; Artificial Intelligence</b>, Yarmouk University · <b>AI Developer</b>, 9xAI Program @ HTU
</p>

---

I build AI systems for the public sector in Jordan — the kind that have to survive a real audit, not just a demo.

My work sits where **LLM agents meet hard, verifiable data**: routable road networks, Arabic NLP, and computer vision. The engineering problem I care about most is **refusal** — designing systems that decline to answer when the evidence isn't there, instead of inventing a number. Everything I ship is bilingual and RTL-first, because the people using it read Arabic.

---

## Selected work

### 🚦 Traffic Intelligence Platform — Amman

A hierarchical multi-agent system that answers real transport-planning questions: *"what happens if University Street closes?"*

It runs over a routable OpenStreetMap graph in PostGIS + pgRouting — **135k car edges, 99k vertices** — with a corridor registry and Arabic street-name resolution. Every answer passes a critic layer that rejects any claim without evidence behind it, so the system returns a refusal and names the gap rather than a plausible-looking number.

```mermaid
flowchart TB
    Q["Planning question<br/>Arabic or English"] --> P

    subgraph AGENTS["Hierarchical agent layer"]
      direction TB
      P["Planner<br/>decomposes the scenario"]
      P --> R["Routing agent"]
      P --> C["Corridor agent"]
      P --> N["Name resolution agent"]
    end

    subgraph DATA["Verifiable data layer"]
      direction TB
      G[("PostGIS · pgRouting<br/>135k edges · 99k vertices")]
      REG[("Corridor registry")]
      AR[("Arabic street-name index")]
    end

    R --> G
    C --> REG
    N --> AR

    G --> E["Evidence set"]
    REG --> E
    AR --> E

    E --> K{"Critic<br/>is every claim backed?"}
    K -->|backed| A["Answer, with its evidence"]
    K -->|unsupported| X["Refuse, and name what is missing"]

    classDef gate fill:#0A66C2,stroke:#0A66C2,color:#ffffff;
    classDef stop fill:#8B2635,stroke:#8B2635,color:#ffffff;
    classDef good fill:#1F6FEB,stroke:#1F6FEB,color:#ffffff;
    class K gate;
    class X stop;
    class A good;
```

`TypeScript` `NestJS` `PostgreSQL/PostGIS` `pgRouting` `Ollama`

---

### 🗣️ VOC-360 (صوت المواطن) — multi-ministry citizen feedback

A complaint intake and analysis platform serving Jordanian ministries. Arabic NLP pipeline, clustering, and causal analysis over free-text citizen complaints, behind cross-ministry role-based access, with Arabic PDF reporting for officials who need the output on paper.

`React` `FastAPI` `PostgreSQL` `Arabic NLP` `Docker`

### 🛸 Aerial Traffic Analysis

Turns raw drone footage into transport data: detection, multi-object tracking, zone occupancy, origin–destination flows, and speeds calibrated against ground truth.

`Python` `Supervision` `YOLO` `OpenCV`

### 🌱 AgriBot AI

Crop prediction and fertilizer recommendation from IoT sensor data, running on-device on a Raspberry Pi. XGBoost at 99% accuracy, Random Forest at 94%.

`Python` `XGBoost` `scikit-learn` `Raspberry Pi`

<sub>Public repositories for selected projects are in preparation.</sub>

---

## Stack

<p align="center">
  <img alt="Python, TypeScript, JavaScript, NestJS, FastAPI, React, Next.js, PostgreSQL, Redis, Docker, Git, Linux, PyTorch, Tailwind, Supabase, Blender" src="https://skillicons.dev/icons?i=python,ts,js,nestjs,fastapi,react,nextjs,postgres,redis,docker,git,linux,pytorch,tailwind,supabase,blender&perline=8" />
</p>

<p align="center">
  <sub>Beyond the icons — <b>PostGIS</b> · <b>pgRouting</b> · <b>Arabic NLP</b> · <b>YOLO / Supervision</b> · <b>Ollama</b> · <b>RTL interface design</b></sub>
</p>

---

## Contributions in 3D

<p align="center">
  <img alt="Contribution graph, night view" src="./profile-3d-contrib/profile-night-view.svg" width="49%" />
  <img alt="Contribution graph, animated seasons" src="./profile-3d-contrib/profile-season-animate.svg" width="49%" />
</p>

<p align="center">
  <img alt="Contribution graph, night rainbow" src="./profile-3d-contrib/profile-night-rainbow.svg" width="49%" />
  <img alt="Contribution graph, git block" src="./profile-3d-contrib/profile-gitblock.svg" width="49%" />
</p>

### 🐍 Snake

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/YAMANOE/YAMANOE/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/YAMANOE/YAMANOE/output/github-snake.svg" />
  <img alt="snake eating my contributions" src="https://raw.githubusercontent.com/YAMANOE/YAMANOE/output/github-snake.svg" />
</picture>

---

## Contact

<p align="center">
  <a href="mailto:yamanobiedat5@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/yaman-obiedat"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
</p>

<p align="center">
  <img alt="" src="https://capsule-render.vercel.app/api?type=waving&color=0:1F6FEB,100:0A66C2&height=100&section=footer" />
</p>
