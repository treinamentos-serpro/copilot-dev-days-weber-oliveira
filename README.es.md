<!-- l10n-sync: source-file="README.md" -->
🌐 [English](README.md) | [Português (BR)](README.pt_BR.md)

<div align="center">

# 🎯 Soc Ops

### Social Bingo — con GitHub Copilot Agent Mode

*Encuentra personas que coincidan con las preguntas. Consigue 5 en línea. ¡Conquista la sala!*

<br/>

[![Java 21](https://img.shields.io/badge/Java-21-orange?logo=openjdk&logoColor=white)](https://adoptium.net/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.4.2-brightgreen?logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![Maven](https://img.shields.io/badge/Maven-3.9%2B-blue?logo=apachemaven&logoColor=white)](https://maven.apache.org/)
[![GitHub Copilot](https://img.shields.io/badge/GitHub%20Copilot-Agent%20Lab-black?logo=github&logoColor=white)](workshop/es/GUIDE.md)
[![Demo en Vivo](https://img.shields.io/badge/Demo%20en%20Vivo-GitHub%20Pages-purple?logo=githubpages&logoColor=white)](https://copilot-dev-days.github.io/agent-lab-java/)

<br/>

**[🎮 Demo en Vivo](https://copilot-dev-days.github.io/agent-lab-java/)** &nbsp;·&nbsp;
**[🚀 Inicio Rápido](#-inicio-rápido)** &nbsp;·&nbsp;
**[📚 Guía del Lab](#-guía-del-lab)** &nbsp;·&nbsp;
**[🏗️ Build & Pruebas](#️-build--pruebas)**

</div>

---

## ✨ ¿Qué es Soc Ops?

Soc Ops es una **app de Social Bingo** para encuentros y talleres presenciales. Cada jugador recibe una tarjeta 5×5 llena de preguntas para romper el hielo, como:

> *"Ha vivido en otro país"* &nbsp;·&nbsp; *"Sabe jugar ajedrez"* &nbsp;·&nbsp; *"Prefiere el modo oscuro"*

Circúla, encuentra personas reales que coincidan, recoge firmas — ¡y grita **BINGO!** 🎉

Pero hay un giro: **la propia app es el taller**. En ~1 hora usarás [GitHub Copilot Agent Mode](https://code.visualstudio.com/docs/copilot/overview) en VS Code para transformarla — rediseñando la interfaz, creando temas personalizados y entregando nuevas funcionalidades con flujos multi-agente de TDD.

> ⏱️ **~1 hora** &nbsp;·&nbsp; 🎓 **Intermedio** &nbsp;·&nbsp; ☕ **Java 21 / Spring Boot / Maven**

---

## 🎯 Qué Construirás y Aprenderás

| | Habilidad | Qué Harás |
|---|-----------|-----------|
| 🧠 | **Ingeniería de Contexto** | Escribe `copilot-instructions.md` para enseñarle a la IA las convenciones del proyecto |
| 🤖 | **Flujos Agentes** | Ejecuta agentes en background, en la nube y pipelines personalizados |
| 🎨 | **Desarrollo Design-First** | Rediseña la interfaz desde cero — Cyberpunk Neon, Vaporwave, Terminal Retro… |
| 🧪 | **Desarrollo Orientado a Pruebas** | Construye el modo Búsqueda del Tesoro con agentes TDD Red → Green → Refactor |

---

## 🚀 Inicio Rápido

**Requisitos previos:** [Java 21 JDK](https://adoptium.net/) · [Maven 3.9+](https://maven.apache.org/) · [VS Code v1.107+](https://code.visualstudio.com/) · [GitHub Copilot](https://github.com/features/copilot)

> 💡 **Camino más rápido:** ábrelo en un [Codespace](https://github.com/features/codespaces) o usa el **DevContainer** incluido — sin configuración local necesaria.

```bash
# 1. Entra al directorio de la app
cd socops

# 2. Inicia el servidor de desarrollo
./mvnw spring-boot:run
```

Abre **[http://localhost:8080](http://localhost:8080)** — tu tarjeta de bingo está lista. ✅

---

## 📚 Guía del Lab

Trabaja las partes en orden; cada una construye directamente sobre la anterior.

| Parte | Título | Tiempo | Qué Sucede |
|-------|--------|--------|------------|
| [**00**](workshop/es/00-overview.md) | Descripción General y Lista de Verificación | — | Verifica tu entorno y herramientas |
| [**01**](workshop/es/01-setup.md) | Configuración e Ingeniería de Contexto | 15 min | Configura Copilot, crea tu sitio en GitHub Pages |
| [**02**](workshop/es/02-design.md) | Desarrollo Frontend Orientado al Diseño | 15 min | Rediseño completo — elige un tema y deja correr el agente |
| [**03**](workshop/es/03-quiz-master.md) | Quiz Master Personalizado | 10 min | Genera conjuntos originales de preguntas de bingo con un agente personalizado |
| [**04**](workshop/es/04-multi-agent.md) | Desarrollo Multi-Agente | 20 min | Modo Búsqueda del Tesoro — agentes TDD construyen toda la funcionalidad |

📖 **[Abrir la Guía Completa del Lab →](workshop/es/GUIDE.md)**

> 📝 Todas las guías están disponibles en [`workshop/es/`](workshop/es/) para lectura sin conexión.

---

## 🎨 Ideas de Temas

¿Sin idea de qué construir en la Parte 2? Algunos puntos de partida para despertar tu creatividad:

`Minimalista Mono` · `Terminal Retro` · `Cyberpunk Neon` · `Atardecer Vaporwave` · `Noir Modo Oscuro` · `Arcade Pixel` · `Galaxia Espacial` · `Bloques Brutalistas` · `Pastel Suave` · `Cristal Degradado`

---

## 🏗️ Build & Pruebas

```bash
cd socops

# Ejecutar en modo de desarrollo (hot reload)
./mvnw spring-boot:run

# Generar JAR de producción
./mvnw clean package

# Correr la suite de pruebas
./mvnw test
```

Cada push a `main` despliega automáticamente a **GitHub Pages** mediante GitHub Actions.

---

## 🔗 Recursos

- 📖 [Documentación de GitHub Copilot](https://code.visualstudio.com/docs/copilot/overview)
- ⭐ [Awesome Copilot](https://github.com/github/awesome-copilot)
- 📺 [VS Code en YouTube](https://www.youtube.com/code)
