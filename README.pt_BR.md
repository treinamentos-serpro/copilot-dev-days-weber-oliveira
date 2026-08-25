<!-- l10n-sync: source-file="README.md" -->
🌐 [English](README.md) | [Español](README.es.md)

<div align="center">

# 🎯 Soc Ops

**Social Bingo para encontros presenciais** — encontre pessoas que correspondam às perguntas e faça 5 em linha!

[![Java 21](https://img.shields.io/badge/Java-21-orange?logo=openjdk)](https://adoptium.net/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.4.2-brightgreen?logo=springboot)](https://spring.io/projects/spring-boot)
[![Maven](https://img.shields.io/badge/Maven-3.9%2B-blue?logo=apachemaven)](https://maven.apache.org/)
[![GitHub Copilot](https://img.shields.io/badge/GitHub%20Copilot-Agent%20Lab-black?logo=github)](workshop/pt_BR/GUIDE.md)

[🚀 Início Rápido](#-início-rápido) · [📚 Guia do Lab](#-guia-do-lab) · [🏗️ Build & Testes](#️-build--testes)

</div>

---

## ✨ O que é o Soc Ops?

O Soc Ops é um **projeto de workshop prático** construído em torno de um app de Social Bingo. Os participantes recebem um cartão de bingo 5×5 com perguntas como *"Já morou em outro país"* ou *"Sabe jogar xadrez"* — e saem circulando para encontrar pessoas reais que se encaixem!

Mas a verdadeira magia? **Você vai turbinar o projeto com o GitHub Copilot Agent Mode** — redesenhando a interface, criando temas personalizados e construindo novas funcionalidades com fluxos multi-agente de TDD.

> ⏱️ **~1 hora** · 🎓 **Intermediário** · ☕ **Java 21 / Spring Boot / Maven**

---

## 🎯 O que Você Vai Construir & Aprender

| # | Habilidade | O que Você Vai Fazer |
|---|------------|----------------------|
| 🧠 | **Engenharia de Contexto** | Ensine o Copilot sobre seu projeto com instruções personalizadas |
| 🤖 | **Primitivos Agentes** | Use agentes em background, na nuvem e fluxos customizados |
| 🎨 | **Desenvolvimento Design-First** | Deixe a IA iterar na interface enquanto você guia a visão criativa |
| 🧪 | **Desenvolvimento Orientado a Testes** | Entregue funcionalidades confiáveis com agentes de TDD |

---

## 🚀 Início Rápido

**Pré-requisitos:** [Java 21 JDK](https://adoptium.net/) · [Maven 3.9+](https://maven.apache.org/) · [VS Code](https://code.visualstudio.com/) · [GitHub Copilot](https://github.com/features/copilot)

> 💡 **Dica:** Use o DevContainer incluído para um ambiente sem configuração!

```bash
# Clone & execute
cd socops
./mvnw spring-boot:run
```

Abra [http://localhost:8080](http://localhost:8080) e comece a jogar! 🎉

---

## 📚 Guia do Lab

Siga as partes do lab em ordem — cada uma constrói sobre a anterior:

| Parte | Título | Duração | Descrição |
|-------|--------|---------|-----------|
| [**00**](workshop/pt_BR/00-overview.md) | Visão Geral & Lista Rápida | — | Verifique sua configuração antes de começar |
| [**01**](workshop/pt_BR/01-setup.md) | Configuração & Engenharia de Contexto | 15 min | Configure o Copilot para entender seu projeto |
| [**02**](workshop/pt_BR/02-design.md) | Frontend Design-First | 15 min | Redesenhe a interface com temas criados por IA |
| [**03**](workshop/pt_BR/03-quiz-master.md) | Quiz Master Personalizado | 10 min | Crie seus próprios conjuntos de perguntas |
| [**04**](workshop/pt_BR/04-multi-agent.md) | Desenvolvimento Multi-Agente | 20 min | Construa funcionalidades com TDD e agentes de design |

📖 **[Abrir o Guia Completo do Lab →](workshop/pt_BR/GUIDE.md)**

> 📝 Todos os guias estão na pasta [`workshop/pt_BR/`](workshop/pt_BR/) para leitura offline.

---

## 🏗️ Build & Testes

```bash
cd socops

# Executar em modo de desenvolvimento
./mvnw spring-boot:run

# Gerar JAR de produção
./mvnw clean package

# Rodar testes
./mvnw test
```

Pushes para `main` fazem deploy automático no GitHub Pages.
