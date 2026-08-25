<!-- l10n-sync: source-file="README.md" -->
🌐 [English](README.md) | [Español](README.es.md)

<div align="center">

# 🎯 Soc Ops

### Social Bingo — com GitHub Copilot Agent Mode

*Encontre pessoas que correspondam às perguntas. Faça 5 em linha. Conquiste a sala.*

<br/>

[![Java 21](https://img.shields.io/badge/Java-21-orange?logo=openjdk&logoColor=white)](https://adoptium.net/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.4.2-brightgreen?logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![Maven](https://img.shields.io/badge/Maven-3.9%2B-blue?logo=apachemaven&logoColor=white)](https://maven.apache.org/)
[![GitHub Copilot](https://img.shields.io/badge/GitHub%20Copilot-Agent%20Lab-black?logo=github&logoColor=white)](workshop/pt_BR/GUIDE.md)
[![Demo ao Vivo](https://img.shields.io/badge/Demo%20ao%20Vivo-GitHub%20Pages-purple?logo=githubpages&logoColor=white)](https://copilot-dev-days.github.io/agent-lab-java/)

<br/>

**[🎮 Demo ao Vivo](https://copilot-dev-days.github.io/agent-lab-java/)** &nbsp;·&nbsp;
**[🚀 Início Rápido](#-início-rápido)** &nbsp;·&nbsp;
**[📚 Guia do Lab](#-guia-do-lab)** &nbsp;·&nbsp;
**[🏗️ Build & Testes](#️-build--testes)**

</div>

---

## ✨ O que é o Soc Ops?

O Soc Ops é um **app de Social Bingo** para encontros e workshops presenciais. Cada jogador recebe um cartão 5×5 cheio de perguntas para quebrar o gelo, como:

> *"Já morou em outro país"* &nbsp;·&nbsp; *"Sabe jogar xadrez"* &nbsp;·&nbsp; *"Prefere modo escuro"*

Circule, encontre pessoas reais que se encaixem, colete assinaturas — e grite **BINGO!** 🎉

Mas tem uma virada: **o próprio app é o workshop**. Em ~1 hora você usará o [GitHub Copilot Agent Mode](https://code.visualstudio.com/docs/copilot/overview) no VS Code para transformá-lo — redesenhando a interface, criando temas personalizados e entregando novas funcionalidades com fluxos multi-agente de TDD.

> ⏱️ **~1 hora** &nbsp;·&nbsp; 🎓 **Intermediário** &nbsp;·&nbsp; ☕ **Java 21 / Spring Boot / Maven**

---

## 🎯 O que Você Vai Construir & Aprender

| | Habilidade | O que Você Vai Fazer |
|---|------------|----------------------|
| 🧠 | **Engenharia de Contexto** | Escreva `copilot-instructions.md` para ensinar a IA as convenções do projeto |
| 🤖 | **Fluxos Agentes** | Execute agentes em background, na nuvem e pipelines personalizados |
| 🎨 | **Desenvolvimento Design-First** | Redesenhe a interface do zero — Cyberpunk Neon, Vaporwave, Terminal Retrô… |
| 🧪 | **Desenvolvimento Orientado a Testes** | Construa o modo Caça ao Tesouro com agentes TDD Red → Green → Refactor |

---

## 🚀 Início Rápido

**Pré-requisitos:** [Java 21 JDK](https://adoptium.net/) · [Maven 3.9+](https://maven.apache.org/) · [VS Code v1.107+](https://code.visualstudio.com/) · [GitHub Copilot](https://github.com/features/copilot)

> 💡 **Caminho mais rápido:** abra em um [Codespace](https://github.com/features/codespaces) ou use o **DevContainer** incluído — sem configuração local necessária.

```bash
# 1. Entre no diretório do app
cd socops

# 2. Inicie o servidor de desenvolvimento
./mvnw spring-boot:run
```

Abra **[http://localhost:8080](http://localhost:8080)** — seu cartão de bingo está pronto. ✅

---

## 📚 Guia do Lab

Siga as partes em ordem; cada uma constrói diretamente sobre a anterior.

| Parte | Título | Tempo | O que Acontece |
|-------|--------|-------|----------------|
| [**00**](workshop/pt_BR/00-overview.md) | Visão Geral & Lista Rápida | — | Verifique seu ambiente e ferramentas |
| [**01**](workshop/pt_BR/01-setup.md) | Configuração & Engenharia de Contexto | 15 min | Configure o Copilot, crie seu site no GitHub Pages |
| [**02**](workshop/pt_BR/02-design.md) | Frontend Design-First | 15 min | Redesign completo — escolha um tema e deixe o agente rodar |
| [**03**](workshop/pt_BR/03-quiz-master.md) | Quiz Master Personalizado | 10 min | Gere conjuntos originais de perguntas de bingo com um agente customizado |
| [**04**](workshop/pt_BR/04-multi-agent.md) | Desenvolvimento Multi-Agente | 20 min | Modo Caça ao Tesouro — agentes de TDD constroem toda a funcionalidade |

📖 **[Abrir o Guia Completo do Lab →](workshop/pt_BR/GUIDE.md)**

> 📝 Todos os guias estão disponíveis em [`workshop/pt_BR/`](workshop/pt_BR/) para leitura offline.

---

## 🎨 Ideias de Temas

Sem ideia do que construir na Parte 2? Alguns pontos de partida para estimular sua criatividade:

`Minimalista Mono` · `Terminal Retrô` · `Cyberpunk Neon` · `Pôr do Sol Vaporwave` · `Noir Modo Escuro` · `Arcade Pixel` · `Galáxia Espacial` · `Blocos Brutalistas` · `Pastel Suave` · `Vidro Gradiente`

---

## 🏗️ Build & Testes

```bash
cd socops

# Executar em modo de desenvolvimento (hot reload)
./mvnw spring-boot:run

# Gerar JAR de produção
./mvnw clean package

# Rodar a suíte de testes
./mvnw test
```

Todo push para `main` faz deploy automático no **GitHub Pages** via GitHub Actions.

---

## 🔗 Recursos

- 📖 [Documentação do GitHub Copilot](https://code.visualstudio.com/docs/copilot/overview)
- ⭐ [Awesome Copilot](https://github.com/github/awesome-copilot)
- 📺 [VS Code no YouTube](https://www.youtube.com/code)
