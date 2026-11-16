<!-- ═══════════════════════════════  HEADER  ═══════════════════════════════ -->
<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=220&color=0:0f172a,50:1e3a8a,100:7c3aed&text=Jorge%20Carrascosa&fontColor=ffffff&fontSize=60&fontAlignY=36&desc=Software%20Engineer%20%C2%B7%20AI%20%C2%B7%20Security%20%C2%B7%20Full-Stack&descAlignY=58&descSize=20&animation=fadeIn" alt="Jorge Carrascosa — Software Engineer" />

<a href="https://github.com/oblivionwing26">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=3200&pause=900&color=A78BFA&center=true&vCenter=true&width=620&lines=Software+Engineer+%E2%80%94+UCLM+graduate+%F0%9F%8E%93;I+build+LLM+agents+that+test+real+software;Security+%C3%97+UX%3A+measuring+the+cost+of+every+fix;TypeScript+%C2%B7+Python+%C2%B7+C%2FC%2B%2B+%C2%B7+Java+%C2%B7+Dart" alt="Typing intro" />
</a>

<p>
  <a href="mailto:jorgestegos@gmail.com"><img src="https://img.shields.io/badge/Email-jorgestegos%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
  <!-- TODO: descomenta y pon tu URL de LinkedIn
  <a href="https://www.linkedin.com/in/TU-USUARIO"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  -->
  <!-- TODO: descomenta y pon la URL de tu portfolio web
  <a href="https://TU-PORTFOLIO"><img src="https://img.shields.io/badge/Portfolio-Visit-111827?style=flat-square&logo=googlechrome&logoColor=white" alt="Portfolio" /></a>
  -->
  <img src="https://img.shields.io/badge/Based%20in-Spain%20%F0%9F%87%AA%F0%9F%87%B8-F59E0B?style=flat-square" alt="Spain" />
  <img src="https://img.shields.io/badge/Open%20to-opportunities-22C55E?style=flat-square" alt="Open to opportunities" />
</p>

</div>

<!-- ═══════════════════════════════  ABOUT  ═══════════════════════════════ -->

## 👋 About me

I'm a **Software Engineer** (B.Sc. in Software Engineering, *Universidad de Castilla-La Mancha*) who likes building systems that are **measurable, reproducible and honest about their numbers**.

Lately I've been working where **LLM agents, application security and UX** meet: tools in which the model decides *what to try next*, and deterministic code decides *whether it worked*.

```ts
const jorge = {
  role:        "Software Engineer",
  education:   "B.Sc. Software Engineering — UCLM (Spain)",
  focus:       ["LLM agents", "AppSec / Red & Blue teaming", "Full-stack TypeScript"],
  principles:  ["Deterministic first, LLM second", "Hexagonal architecture", "Tests or it didn't happen"],
  alsoLikes:   ["Game engines from scratch", "Mobile apps", "Data bots"],
  languages:   { spanish: "native", english: "professional" },
};
```

<!-- ═══════════════════════════════  FEATURED  ═══════════════════════════════ -->

## 🚀 Featured project

<table>
<tr>
<td width="62%" valign="top">

### 🛡️ [Janus Arena](https://github.com/oblivionwing26/janus-arena)

**A pre-release gate that catches UX-friction regressions *and* security regressions in the same pull request — and measures the UX cost of every security fix.**

- 🧪 **SynthLab** — synthetic user personas drive two variants of a web app in a real browser (Playwright). An LLM picks the next action; friction, success, latency and statistics are computed by code.
- ⚔️ **WarRoom** — static audit → **Red Team** attacks in an isolated sandbox → **Blue Team** agent patches → fix verified **three independent ways** (PoC dead, tests + regression test green, UX within tolerance).
- 📜 Output: a **signed dual report** (UX A/B + security) attached to a PR. Janus never merges — a human does.
- 📈 Found **6 confirmed vulnerabilities** on OWASP Juice Shop with replayable PoCs; showed an account lockout costs real users while a per-account rate limit doesn't.

<p>
  <a href="https://janus-arena.vercel.app"><img src="https://img.shields.io/badge/Live%20demo-janus--arena.vercel.app-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Live demo" /></a>
  <a href="https://youtu.be/rH7XLE4Ujks"><img src="https://img.shields.io/badge/3--min%20video-Watch-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Video" /></a>
</p>

</td>
<td width="38%" valign="top">

**Architecture highlights**

- Monorepo · **pnpm + Turborepo**
- **NestJS on Fastify**, hexagonal (rules enforced in CI with *dependency-cruiser*)
- **Next.js 16 / React 19** console with attack graph (*React Flow*) and swarm canvas (*PixiJS*)
- **PostgreSQL + Prisma**, append-only event log (DB trigger blocks updates)
- **Redis + BullMQ** job queue
- **Docker** sandboxes behind a socket proxy
- **Claude API** agents with per-stage budgets
- Seeded stats: **Wilson intervals, paired bootstrap**
- Resumable pipeline, signed & verifiable reports
- **Vitest**, ESLint, Prettier, GitHub Actions CI

</td>
</tr>
</table>

## 🧩 More projects

<div align="center">

<a href="https://github.com/oblivionwing26/janus-shoplab"><img width="49%" src="https://github-readme-stats.vercel.app/api/pin/?username=oblivionwing26&repo=janus-shoplab&theme=tokyonight&hide_border=true&border_radius=12&description_lines_count=2" alt="Janus ShopLab" /></a>
<a href="https://github.com/oblivionwing26/MazeRay"><img width="49%" src="https://github-readme-stats.vercel.app/api/pin/?username=oblivionwing26&repo=MazeRay&theme=tokyonight&hide_border=true&border_radius=12&description_lines_count=2" alt="MazeRay" /></a>

</div>

| Project | What it is | Stack |
|---|---|---|
| 🛒 **[Janus ShopLab](https://github.com/oblivionwing26/janus-shoplab)** | E-commerce target app with *documented* UX flaws as ground truth, plus opt-in defenses (rate limits, lockouts) to measure what security costs real users. | Next.js · Prisma · PostgreSQL · Zod · Docker · Vitest |
| 🎮 **[MazeRay](https://github.com/oblivionwing26/MazeRay)** | First-person maze shooter on a **custom raycasting engine**: procedurally generated mazes (modified DFS), z-buffered sprites, enemies with chase AI. | C · raylib · Make |
| ⏰ **Smart Alarm** | Cross-platform smart alarm mobile app. | Dart · Flutter |
| 🕒 **Timbra** | Application in active development. | TypeScript |
| 🏁 **Racing Team Web** | Website for a racing team. | TypeScript |
| 📊 **Memecoin market crawler** | Bot for market research and prediction on Solana memecoins: scraping, data collection and analysis. | Python |
| 🧮 **SSDD Calculator** | Distributed-systems coursework: remote calculator service. | Python |
| 🏗️ **Software Design web app** | Web application built for the *Software Design* course. | Java |

<!-- ═══════════════════════════════  STACK  ═══════════════════════════════ -->

## 🛠️ Tech stack

<table>
<tr><td><b>Languages</b></td><td>
<img src="https://skillicons.dev/icons?i=ts,js,python,c,cpp,java,dart,html,css,ruby&perline=12" alt="Languages" />
</td></tr>
<tr><td><b>Frontend & mobile</b></td><td>
<img src="https://skillicons.dev/icons?i=react,nextjs,tailwind,flutter,vite&perline=12" alt="Frontend" />
</td></tr>
<tr><td><b>Backend</b></td><td>
<img src="https://skillicons.dev/icons?i=nodejs,nestjs,django,flask,rails,prisma&perline=12" alt="Backend" />
</td></tr>
<tr><td><b>Data & infra</b></td><td>
<img src="https://skillicons.dev/icons?i=postgres,redis,docker,vercel,githubactions,linux,ubuntu&perline=12" alt="Infra" />
</td></tr>
<tr><td><b>Testing & tooling</b></td><td>
<img src="https://skillicons.dev/icons?i=vitest,pnpm,git,github,vscode,visualstudio,eclipse,raylib&perline=12" alt="Tooling" />
</td></tr>
</table>

<sub>Also: <b>Playwright</b> · <b>Claude API / LLM agents</b> · <b>BullMQ</b> · <b>Zod</b> · <b>Turborepo</b> · <b>React Flow</b> · <b>PixiJS</b> · <b>dependency-cruiser</b> · <b>OWASP</b> testing</sub>

<!-- ═══════════════════════════════  HOW I WORK  ═══════════════════════════════ -->

## 🧠 How I work

- **Deterministic first, LLM second** — models propose; code, oracles and statistics decide.
- **Architecture you can enforce** — hexagonal layers, checked in CI, not just drawn in a diagram.
- **Reproducible by default** — event logs, seeded stats, replayable runs, Docker everywhere.
- **Report the unflattering numbers too** — confidence intervals, not cherry-picked screenshots.

<!-- ═══════════════════════════════  STATS  ═══════════════════════════════ -->

## 📈 GitHub activity

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=oblivionwing26&show_icons=true&count_private=true&include_all_commits=true&rank_icon=github&theme=tokyonight&hide_border=true&border_radius=12" alt="GitHub stats" />
<img height="165" src="https://streak-stats.demolab.com?user=oblivionwing26&theme=tokyonight&hide_border=true&border_radius=12" alt="GitHub streak" />

<img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=oblivionwing26&theme=tokyo-night&hide_border=true&area=true&radius=12" alt="Contribution graph" />

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/oblivionwing26/oblivionwing26/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/oblivionwing26/oblivionwing26/output/github-snake.svg" />
  <img alt="Contribution snake" src="https://raw.githubusercontent.com/oblivionwing26/oblivionwing26/output/github-snake.svg" />
</picture>

</div>

<!-- ═══════════════════════════════  FOOTER  ═══════════════════════════════ -->

## 📫 Let's talk

I'm open to **Software Engineer** roles and interesting collaborations — especially around AI agents, application security or full-stack product work.
The fastest way to reach me is **[jorgestegos@gmail.com](mailto:jorgestegos@gmail.com)**.

<div align="center">

<img src="https://komarev.com/ghpvc/?username=oblivionwing26&style=flat-square&color=7c3aed&label=profile+views" alt="Profile views" />

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=110&color=0:7c3aed,50:1e3a8a,100:0f172a&section=footer" alt="" />

</div>
