🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

<div align="center">

# 🎯 Soc Ops

### Social Bingo — powered by GitHub Copilot Agent Mode

*Find people who match the prompts. Get 5 in a row. Win the room.*

<br/>

[![Java 21](https://img.shields.io/badge/Java-21-orange?logo=openjdk&logoColor=white)](https://adoptium.net/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.4.2-brightgreen?logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![Maven](https://img.shields.io/badge/Maven-3.9%2B-blue?logo=apachemaven&logoColor=white)](https://maven.apache.org/)
[![GitHub Copilot](https://img.shields.io/badge/GitHub%20Copilot-Agent%20Lab-black?logo=github&logoColor=white)](workshop/GUIDE.md)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-purple?logo=githubpages&logoColor=white)](https://copilot-dev-days.github.io/agent-lab-java/)

<br/>

**[🎮 Live Demo](https://copilot-dev-days.github.io/agent-lab-java/)** &nbsp;·&nbsp;
**[🚀 Quick Start](#-quick-start)** &nbsp;·&nbsp;
**[📚 Lab Guide](#-lab-guide)** &nbsp;·&nbsp;
**[🏗️ Build & Test](#️-build--test)**

</div>

---

## ✨ What is Soc Ops?

Soc Ops is a **Social Bingo web app** for in-person mixers and workshops. Each player gets a 5×5 card packed with icebreaker prompts like:

> *"Has lived in another country"* &nbsp;·&nbsp; *"Knows how to play chess"* &nbsp;·&nbsp; *"Prefers dark mode"*

Mingle, find real people who match, collect signatures — and shout **BINGO!** 🎉

But here's the twist: **the app itself is the workshop**. Over ~1 hour you'll use [GitHub Copilot Agent Mode](https://code.visualstudio.com/docs/copilot/overview) inside VS Code to transform it — redesigning the UI, authoring custom quiz themes, and shipping new features end-to-end with multi-agent TDD workflows.

> ⏱️ **~1 hour** &nbsp;·&nbsp; 🎓 **Intermediate** &nbsp;·&nbsp; ☕ **Java 21 / Spring Boot / Maven**

---

## 🎯 What You'll Build & Learn

| | Skill | What You'll Do |
|---|-------|----------------|
| 🧠 | **Context Engineering** | Write `copilot-instructions.md` to teach the AI your codebase conventions |
| 🤖 | **Agentic Workflows** | Run background agents, cloud agents, and custom agent pipelines |
| 🎨 | **Design-First Frontend** | Redesign the UI from scratch — Cyberpunk Neon, Vaporwave, Retro Terminal… |
| 🧪 | **Test-Driven Development** | Build a Scavenger Hunt mode with TDD Red → Green → Refactor agents |

---

## 🚀 Quick Start

**Prerequisites:** [Java 21 JDK](https://adoptium.net/) · [Maven 3.9+](https://maven.apache.org/) · [VS Code v1.107+](https://code.visualstudio.com/) · [GitHub Copilot](https://github.com/features/copilot)

> 💡 **Fastest path:** open in a [Codespace](https://github.com/features/codespaces) or use the included **DevContainer** — zero local setup required.

```bash
# 1. Move into the app directory
cd socops

# 2. Start the dev server
./mvnw spring-boot:run
```

Open **[http://localhost:8080](http://localhost:8080)** — your bingo card is ready. ✅

---

## 📚 Lab Guide

Work through the parts in order; each one builds directly on the last.

| Part | Title | Time | What Happens |
|------|-------|------|--------------|
| [**00**](workshop/00-overview.md) | Overview & Checklist | — | Verify your environment and tools |
| [**01**](workshop/01-setup.md) | Setup & Context Engineering | 15 min | Configure Copilot, create your GitHub Pages site |
| [**02**](workshop/02-design.md) | Design-First Frontend | 15 min | Full UI redesign — pick a theme and let the agent run |
| [**03**](workshop/03-quiz-master.md) | Custom Quiz Master | 10 min | Generate original bingo question sets with a custom agent |
| [**04**](workshop/04-multi-agent.md) | Multi-Agent Development | 20 min | Scavenger Hunt mode — TDD agents build the whole feature |

📖 **[Open the Full Lab Guide →](workshop/GUIDE.md)**

> 📝 All guides are available in [`workshop/`](workshop/) for offline reading.

---

## 🎨 Theme Ideas

Not sure what to build in Part 2? Here are some starting points to spark your creativity:

`Minimalist Mono` · `Retro Terminal` · `Cyberpunk Neon` · `Vaporwave Sunset` · `Dark Mode Noir` · `Pixel Arcade` · `Space Galaxy` · `Brutalist Blocks` · `Soft Pastel` · `Gradient Glass`

---

## 🏗️ Build & Test

```bash
cd socops

# Run in development mode (hot reload)
./mvnw spring-boot:run

# Build a production JAR
./mvnw clean package

# Run the test suite
./mvnw test
```

Every push to `main` automatically deploys to **GitHub Pages** via GitHub Actions.

---

## 🔗 Resources

- 📖 [GitHub Copilot Docs](https://code.visualstudio.com/docs/copilot/overview)
- ⭐ [Awesome Copilot](https://github.com/github/awesome-copilot)
- 📺 [VS Code YouTube](https://www.youtube.com/code)
