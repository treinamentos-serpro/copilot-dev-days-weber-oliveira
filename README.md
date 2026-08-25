🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

<div align="center">

# 🎯 Soc Ops

**Social Bingo for in-person mixers** — find people who match the prompts and get 5 in a row!

[![Java 21](https://img.shields.io/badge/Java-21-orange?logo=openjdk)](https://adoptium.net/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.4.2-brightgreen?logo=springboot)](https://spring.io/projects/spring-boot)
[![Maven](https://img.shields.io/badge/Maven-3.9%2B-blue?logo=apachemaven)](https://maven.apache.org/)
[![GitHub Copilot](https://img.shields.io/badge/GitHub%20Copilot-Agent%20Lab-black?logo=github)](workshop/GUIDE.md)

[🚀 Quick Start](#-quick-start) · [📚 Lab Guide](#-lab-guide) · [🏗️ Build & Test](#️-build--test)

</div>

---

## ✨ What is Soc Ops?

Soc Ops is a **hands-on workshop project** built around a Social Bingo web app. Participants receive a unique 5×5 bingo card filled with prompts like *"Has lived in another country"* or *"Knows how to play chess"* — then mingle and find real people who match!

But the real magic? **You'll supercharge it with GitHub Copilot Agent Mode** — redesigning the UI, creating custom quiz themes, and building new features using multi-agent TDD workflows.

> ⏱️ **~1 hour** · 🎓 **Intermediate** · ☕ **Java 21 / Spring Boot / Maven**

---

## 🎯 What You'll Build & Learn

| # | Skill | What You'll Do |
|---|-------|----------------|
| 🧠 | **Context Engineering** | Teach Copilot about your codebase with custom instructions |
| 🤖 | **Agentic Primitives** | Use background agents, cloud agents, and custom workflows |
| 🎨 | **Design-First Development** | Let AI iterate on UI while you guide the creative vision |
| 🧪 | **Test-Driven Development** | Ship reliable features with TDD agents |

---

## 🚀 Quick Start

**Prerequisites:** [Java 21 JDK](https://adoptium.net/) · [Maven 3.9+](https://maven.apache.org/) · [VS Code](https://code.visualstudio.com/) · [GitHub Copilot](https://github.com/features/copilot)

> 💡 **Tip:** Use the included DevContainer for a zero-setup environment!

```bash
# Clone & run
cd socops
./mvnw spring-boot:run
```

Open [http://localhost:8080](http://localhost:8080) and you're playing! 🎉

---

## 📚 Lab Guide

Work through the lab parts in order — each builds on the previous:

| Part | Title | Duration | Description |
|------|-------|----------|-------------|
| [**00**](workshop/00-overview.md) | Overview & Checklist | — | Verify your setup before you start |
| [**01**](workshop/01-setup.md) | Setup & Context Engineering | 15 min | Configure Copilot to understand your project |
| [**02**](workshop/02-design.md) | Design-First Frontend | 15 min | Redesign the UI with AI-driven creative themes |
| [**03**](workshop/03-quiz-master.md) | Custom Quiz Master | 10 min | Create your own bingo prompt sets |
| [**04**](workshop/04-multi-agent.md) | Multi-Agent Development | 20 min | Build new features with TDD and design agents |

📖 **[Open the Full Lab Guide →](workshop/GUIDE.md)**

> 📝 All guides live in [`workshop/`](workshop/) for offline reading.

---

## 🏗️ Build & Test

```bash
cd socops

# Run in development mode
./mvnw spring-boot:run

# Build a production JAR
./mvnw clean package

# Run tests
./mvnw test
```

Pushes to `main` deploy automatically to GitHub Pages.
