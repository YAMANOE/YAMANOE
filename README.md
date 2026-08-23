<p align="center">
  <img alt="Yaman Obiedat — AI Systems · Geospatial Intelligence · Computer Vision. Evidence-grounded systems for real-world infrastructure." src="./assets/hero.svg" width="100%" />
</p>

<table>
<tr>
<td width="56%" valign="top">
<p>I build AI systems for the public sector in Jordan — the kind that have to survive a real audit, not just a demo.</p>
<p>My work sits where <b>LLM agents meet hard, verifiable data</b>: routable road networks, Arabic NLP, and computer vision. The engineering problem I care about most is <b>refusal</b> — designing systems that decline to answer when the evidence isn't there, instead of inventing a number.</p>
<p>Everything I ship is bilingual and RTL-first, because the people using it read Arabic.</p>
</td>
<td width="44%" valign="top">
<p><b>B.Sc. Data Science &amp; Artificial Intelligence</b><br/><sub>Yarmouk University</sub></p>
<p><b>AI Developer — 9xAI Program</b><br/><sub>Al-Hussein Technical University (HTU)</sub></p>
<p><b>Amman, Jordan</b><br/><sub>Arabic · English · RTL-first engineering</sub></p>
</td>
</tr>
</table>

## ▍Flagship — Traffic Intelligence Platform

<table>
<tr>
<td width="25%" valign="top"><sub><b>PROBLEM</b></sub><br/>Planners need to know what a road closure does to the network <i>before</i> it happens.</td>
<td width="25%" valign="top"><sub><b>APPROACH</b></sub><br/>A hierarchical multi-agent system answering in Arabic or English over a routable OpenStreetMap graph.</td>
<td width="25%" valign="top"><sub><b>SCALE</b></sub><br/><b>135k</b> routable car edges<br/><b>99k</b> graph vertices</td>
<td width="25%" valign="top"><sub><b>GUARANTEE</b></sub><br/>A critic gates every response. No claim ships without evidence behind it.</td>
</tr>
</table>

<p align="center">
  <img alt="Request pipeline: a planning question in Arabic or English reaches a planner, which dispatches routing, corridor and name-resolution agents against verified data sources — PostGIS and pgRouting at 135k edges and 99k vertices, a corridor registry, and an Arabic street-name index. Results form an evidence set that a critic gates: backed claims return an answer with its evidence, unsupported claims return a refusal naming what is missing." src="./assets/architecture.svg" width="100%" />
</p>

> *“What happens if University Street closes?”* — the system resolves the street name in Arabic, re-routes across the corridor registry, and either answers **with the evidence attached**, or refuses and **names the evidence it does not have**. It never fills the gap with a plausible number.

<p><sub><code>TypeScript</code> · <code>NestJS</code> · <code>PostgreSQL</code> · <code>PostGIS</code> · <code>pgRouting</code> · <code>Ollama</code></sub></p>

## ▍Selected systems

<table>
<tr>
<td width="33%" valign="top"><b>🗣️ VOC-360 · صوت المواطن</b><br/><sub><b>ARABIC NLP · CIVIC PLATFORM</b></sub></td>
<td width="33%" valign="top"><b>🛸 Aerial Traffic Analysis</b><br/><sub><b>COMPUTER VISION · TRANSPORT</b></sub></td>
<td width="33%" valign="top"><b>🌱 AgriBot AI</b><br/><sub><b>EDGE ML · GRADUATION PROJECT</b></sub></td>
</tr>
<tr>
<td valign="top">Complaint intake and analysis for Jordanian ministries.</td>
<td valign="top">Raw drone footage turned into usable transport data.</td>
<td valign="top">Crop and fertilizer recommendation from IoT sensor data.</td>
</tr>
<tr>
<td valign="top"><sub>Clustering and causal analysis sit behind cross-ministry role-based access — and the findings leave the system as Arabic PDF reports officials can circulate and file.</sub></td>
<td valign="top"><sub>Detection, multi-object tracking and zone occupancy produce origin–destination flows and speeds calibrated against ground truth, not raw pixel counts.</sub></td>
<td valign="top"><sub>Runs on-device on a Raspberry Pi. XGBoost 99% and Random Forest 94% on the project's sensor dataset — graduation evaluation figures, not a production deployment.</sub></td>
</tr>
<tr>
<td valign="top"><sub><code>React</code> <code>FastAPI</code> <code>PostgreSQL</code> <code>Docker</code></sub></td>
<td valign="top"><sub><code>Python</code> <code>YOLO</code> <code>Supervision</code> <code>OpenCV</code></sub></td>
<td valign="top"><sub><code>Python</code> <code>XGBoost</code> <code>scikit-learn</code></sub></td>
</tr>
</table>

## ▍Engineering capability

<table>
<tr>
<td width="20%" valign="top"><b>SYSTEMS &amp; DATA</b></td>
<td valign="top"><code>TypeScript</code> <code>NestJS</code> <code>FastAPI</code> <code>PostgreSQL</code> <code>Docker</code> <code>Raspberry Pi</code><br/><sub>Service architecture, relational modelling, containerised and on-device deployment.</sub></td>
</tr>
<tr>
<td valign="top"><b>GEOSPATIAL</b></td>
<td valign="top"><code>PostGIS</code> <code>pgRouting</code> <code>OpenStreetMap</code><br/><sub>Routable graph construction and shortest-path analysis over a 135k-edge road network.</sub></td>
</tr>
<tr>
<td valign="top"><b>AI &amp; VISION</b></td>
<td valign="top"><code>Ollama</code> <code>Arabic NLP</code> <code>YOLO</code> <code>Supervision</code> <code>OpenCV</code> <code>XGBoost</code> <code>scikit-learn</code><br/><sub>Multi-agent orchestration, evidence gating, detection and multi-object tracking.</sub></td>
</tr>
<tr>
<td valign="top"><b>INTERFACE</b></td>
<td valign="top"><code>React</code> <code>RTL / bilingual UI</code> <code>Arabic PDF reporting</code><br/><sub>Right-to-left layout as a first-class constraint, not a translation pass.</sub></td>
</tr>
</table>

## ▍Activity

<p><sub>Contribution rendering — supporting activity, not a measure of the systems above.</sub></p>

<p align="center">
  <img alt="Contribution graph rendered as an animated 3D landscape, night view" src="./profile-3d-contrib/profile-night-view.svg" width="49%" />
  <img alt="Contribution graph rendered as animated 3D commit blocks, night view" src="./profile-3d-contrib/profile-night-green.svg" width="49%" />
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/YAMANOE/YAMANOE/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/YAMANOE/YAMANOE/output/github-snake.svg" />
    <img alt="snake eating my contributions" src="https://raw.githubusercontent.com/YAMANOE/YAMANOE/output/github-snake.svg" width="100%" />
  </picture>
</p>

## ▍Contact

<p align="center">
  <a href="mailto:yamanobiedat5@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/yaman-obiedat"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://github.com/YAMANOE"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
</p>

<p align="center">
  <img alt="" src="./assets/footer.svg" width="100%" />
</p>
