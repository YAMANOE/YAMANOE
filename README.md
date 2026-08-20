<p align="center">
  <img alt="Yaman Obiedat — AI Engineer, Amman, Jordan" src="./assets/hero.svg" width="100%" />
</p>

<p align="center">
  <b>B.Sc. Data Science &amp; Artificial Intelligence</b>, Yarmouk University · <b>AI Developer</b>, 9xAI Program @ HTU
</p>

<p align="center">
  <b>Multi-agent systems that refuse to guess</b> · Computer vision &amp; Arabic NLP<br/>
  Civic technology for the public sector · PostGIS · pgRouting · LLM agents
</p>

---

I build AI systems for the public sector in Jordan — the kind that have to survive a real audit, not just a demo.

My work sits where **LLM agents meet hard, verifiable data**: routable road networks, Arabic NLP, and computer vision. The engineering problem I care about most is **refusal** — designing systems that decline to answer when the evidence isn't there, instead of inventing a number. Everything I ship is bilingual and RTL-first, because the people using it read Arabic.

---

## Selected work

### 🚦 Traffic Intelligence Platform

*Hierarchical multi-agent transport planning · Amman*

Answers real planning questions — *"what happens if University Street closes?"* — over a routable OpenStreetMap graph in PostGIS + pgRouting (**135k car edges, 99k vertices**), with a corridor registry and Arabic street-name resolution.

Every response passes a critic layer that rejects any claim without evidence behind it. When the graph can't support an answer, the system says so and names the missing evidence rather than returning a plausible number.

```mermaid
flowchart LR
    Q["Planning question<br/>AR / EN"]:::input --> P["Planner"]:::agent

    P --> R["Routing<br/>agent"]:::agent
    P --> C["Corridor<br/>agent"]:::agent
    P --> N["Name<br/>resolution"]:::agent

    R --> G[("PostGIS · pgRouting<br/>135k edges · 99k vertices")]:::store
    C --> REG[("Corridor<br/>registry")]:::store
    N --> AR[("Arabic street-name<br/>index")]:::store

    G --> E["Evidence<br/>set"]:::evidence
    REG --> E
    AR --> E

    E --> K{"Critic"}:::gate
    K -->|backed| A["Answer, with<br/>its evidence"]:::good
    K -->|unsupported| X["Refuse, and name<br/>the missing evidence"]:::stop

    classDef input    fill:#475569,stroke:#475569,color:#ffffff;
    classDef agent    fill:#1F6FEB,stroke:#1F6FEB,color:#ffffff;
    classDef store    fill:#0E7490,stroke:#0E7490,color:#ffffff;
    classDef evidence fill:#0A66C2,stroke:#0A66C2,color:#ffffff;
    classDef gate     fill:#B45309,stroke:#B45309,color:#ffffff;
    classDef good     fill:#15803D,stroke:#15803D,color:#ffffff;
    classDef stop     fill:#9F1239,stroke:#9F1239,color:#ffffff;
```

`TypeScript` `NestJS` `PostgreSQL/PostGIS` `pgRouting` `Ollama`

---

### 🗣️ VOC-360 · صوت المواطن

*Citizen feedback intake and analysis · multi-ministry deployment*

An Arabic NLP pipeline over free-text citizen complaints — clustering and causal analysis behind cross-ministry role-based access.

Built around how the institution actually works: findings leave the system as Arabic PDF reports officials can circulate and file.

`React` `FastAPI` `PostgreSQL` `Arabic NLP` `Docker`

---

### 🛸 Aerial Traffic Analysis

*Drone footage to transport data · computer vision pipeline*

Detection, multi-object tracking, and zone occupancy from raw aerial footage.

Output is planning-grade rather than illustrative: origin–destination flows and speeds calibrated against ground truth, not raw pixel counts.

`Python` `Supervision` `YOLO` `OpenCV`

---

### 🌱 AgriBot AI

*Graduation Project · on-device crop intelligence*

Crop prediction and fertilizer recommendation from IoT sensor data, running on a Raspberry Pi rather than off-device.

On the project's sensor dataset, XGBoost reached 99% accuracy and Random Forest 94% — figures from the graduation evaluation, not a production deployment.

`Python` `XGBoost` `scikit-learn` `Raspberry Pi`

---

## Engineering stack

<p align="center">
  <sub><b>SYSTEMS &amp; DATA</b></sub><br/>
  <img alt="TypeScript, NestJS, FastAPI, PostgreSQL, Redis, Supabase, Docker, Linux" src="https://skillicons.dev/icons?i=ts,nestjs,fastapi,postgres,redis,supabase,docker,linux&perline=8" />
</p>

<p align="center">
  <sub><b>AI &amp; VISION</b></sub><br/>
  <img alt="Python, PyTorch" src="https://skillicons.dev/icons?i=python,pytorch&perline=8" />
</p>

<p align="center">
  <sub><b>INTERFACE</b></sub><br/>
  <img alt="React, Next.js, Tailwind CSS, Blender" src="https://skillicons.dev/icons?i=react,nextjs,tailwind,blender&perline=8" />
</p>

<p align="center">
  <sub>Beyond the icons — <b>PostGIS</b> · <b>pgRouting</b> · <b>Arabic NLP</b> · <b>YOLO / Supervision</b> · <b>Ollama</b> · <b>RTL interface design</b></sub>
</p>

---

## Contributions in 3D

<p align="center">
  <img alt="Contribution graph rendered as an animated seasonal 3D landscape" src="./profile-3d-contrib/profile-season-animate.svg" width="49%" />
  <img alt="Contribution graph rendered as animated 3D commit blocks" src="./profile-3d-contrib/profile-gitblock.svg" width="49%" />
</p>

<p align="center">
  <sub>Seasonal cycle · commit blocks — both animated, regenerated daily by GitHub Actions</sub>
</p>

<br/>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/YAMANOE/YAMANOE/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/YAMANOE/YAMANOE/output/github-snake.svg" />
    <img alt="snake eating my contributions" src="https://raw.githubusercontent.com/YAMANOE/YAMANOE/output/github-snake.svg" width="100%" />
  </picture>
</p>

---

## Contact

<p align="center">
  <a href="mailto:yamanobiedat5@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/yaman-obiedat"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://github.com/YAMANOE"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
</p>

<p align="center">
  <img alt="" src="./assets/footer.svg" width="100%" />
</p>
