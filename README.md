# Research Methodology Hub

> Standardized, step-by-step **research-methodology guides across disciplines** — built for reproducibility, rigor, and structure.

![Status](https://img.shields.io/badge/status-early%20stage-orange)
![License](https://img.shields.io/badge/license-Apache%202.0-blue)
![Org](https://img.shields.io/badge/org-Research--Methodology--Hub-black)

This project was built to make rigorous, reproducible research accessible to everyone — across disciplines. 🔬 by Mohamed El Hajji and the community.

> ⚠️ **Early stage.** Guide content is being written and the platform is taking shape. The roadmap below describes where this project is headed.

---

## Overview

Across disciplines, **reproducibility and methodological rigor are major challenges**. Research Methodology Hub is an open-source toolbox of guidelines, frameworks, and templates that help researchers follow a clear, dependable process — from formulating a problem to disseminating results.

Rather than one guide, the Hub hosts **multiple methodology guides**, each tailored to its field but sharing the same structure: an overview of scientific research, followed by an ordered, step-by-step research process.

---

## Methodology guides

| Guide | Domain | Status |
|-------|--------|--------|
| **Computer Science & AI** | Computer Science · AI · Data Science | ✅ Available (7 steps) |
| **Educational Research** | Education · Social Sciences | ✅ Available (7 steps) |
| **Health Research** | Clinical · Public Health · Biomedical | 🟡 Coming soon |
| _More disciplines_ | Engineering, Medicine, … | 📋 Planned |

Each guide is **self-contained and kept methodologically distinct** (e.g. the computational workflow — datasets, architectures, benchmarks — is never mixed with the social-science workflow — variables, instruments, sampling). Adding a new methodology is intentionally easy: drop one file into `web/src/guide/methodologies/` and register it.

---

## Who It's For

- 🎓 **Master's students** — learning to structure a research project
- 🔬 **PhD students** — conducting and publishing original research
- 🧑‍🏫 **Supervisors / teachers** — guiding and reviewing student work (encadrement)
- 📚 **Scientific researchers** — standardizing methodology across projects
- 🤖 **AI assistants / agents** — supporting researchers throughout the workflow

---

## Repository Structure

```
.
├── README.md            # You are here
├── CONTRIBUTING.md      # How to contribute
├── LICENSE              # Apache 2.0
├── doc/                 # Documentation & community notes
└── web/                 # Frontend app — React + Vite + TypeScript
    └── src/
        ├── brand/                  # Méridien logo & palette
        ├── guide/methodologies/    # one file per methodology guide
        └── pages/                  # Landing · Catalogue · GuideEntry · About
```

> A future `api/` (backend & AI services) will be added as the platform grows.

### Running the web app

```bash
cd web
npm install
npm run dev      # start the dev server
npm run build    # production build (also type-checks)
```

---

## How to Use This Repository

1. **Explore** — browse the methodology guides and find the one matching your discipline.
2. **Clone** — get a local copy:
   ```bash
   git clone https://github.com/Research-Methodology-Hub/Research-Methodologies.git
   ```
3. **Adapt** — modify the templates and steps to fit your specific research project and constraints.

---

## Roadmap / Coming Soon

Beyond the written guides, the project aims to deliver methodology through an interactive platform:

- 🧭 **Methodology Master** — an AI agent that mentors researchers step-by-step
- 💬 **AI assistant / chatbot** — grounded Q&A over the guides (MCP + skills)
- 🧪 **Decision aid** — "which methodology should I use?" wizard
- 🎯 **Quizzes & self-assessment** per step
- 🎬 **Learning formats** — infographics, case studies, slides, and videos
- 📱 **Mobile app** · 🔗 **Integrations** (Google Colab, Notion)

See [doc/community-issues.md](doc/community-issues.md) for the flagship epics.

### Planned Tech Stack

| Layer          | Technology                              | Status              |
|----------------|-----------------------------------------|---------------------|
| **Frontend**   | React + Vite + TypeScript, React Router | ✅ Confirmed        |
| **Backend**    | Node.js (`api/`)                        | 🟡 Under evaluation |
| **AI / Agent** | MCP + Skills.                           | ✅ Confirmed        |
| **CI/CD**      | GitHub Actions                          | ✅ Confirmed        |

> The stack is planned and may evolve as the platform takes shape.

---

## Contributing

Contributions are what make the research community vibrant — fixes, new methodology guides, and improvements are all welcome. Please read **[CONTRIBUTING.md](CONTRIBUTING.md)** for the workflow, local checks, and our Conventional-Commit + AI-assistance conventions.

In short: fork → branch off `main` → run `npm run lint` and `npm run build` in `web/` → open a PR with a Conventional-Commit title.

---

## License

Distributed under the **Apache License 2.0**. See the [LICENSE](LICENSE) file for details.
