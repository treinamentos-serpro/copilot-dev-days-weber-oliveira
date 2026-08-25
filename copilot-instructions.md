---
name: workspace
description: Instructions for the Soc Ops Spring Boot project - a social bingo game for in-person mixers
---

# Soc Ops Workspace Instructions

## ✅ Mandatory Development Checklist

Before committing or pushing code, run these in order from `socops/`:
```bash
# 1. Lint & compile
./mvnw clean compile

# 2. Run tests
./mvnw test

# 3. Build package
./mvnw clean package
```
**All three must pass before push to main.**

---

## Project Overview

**Soc Ops** is a Spring Boot 3.4.2 social bingo game (Java 21, Maven). Players find people matching prompts and get 5 in a row. Uses Thymeleaf templates with custom CSS utilities (Tailwind-like).

**Key Structure**: `socops/src/main/java/com/socops/` → `model/`, `service/`, `web/`, `data/`

## Quick Commands

| Command | Purpose |
|---------|---------|
| `cd socops && ./mvnw spring-boot:run` | Start dev server on `http://localhost:8080` (hot reload enabled) |
| `cd socops && ./mvnw test` | Run unit tests |
| `cd socops && ./mvnw clean package` | Build JAR package |

## Code Organization

| Package | Purpose | Classes |
|---------|---------|---------|
| `model/` | Data structures | `BingoCell`, `PlayPhase`, `WinningStreak` |
| `service/` | Business logic | `BoardAssembler` (board generation) |
| `web/` | REST endpoints | `BingoRestController` (routes, JSON responses) |
| `data/` | Static content | `IcebreakerPrompts` (quiz questions) |

**Naming**: PascalCase classes, `com.socops.<layer>` packages. Use Spring annotations: `@Controller`, `@GetMapping`, `@ResponseBody`.

## Frontend & Styling

**Thymeleaf** templates in `src/main/resources/templates/game.html`. Use custom CSS utilities from `app.css`:
- Layout: `.flex`, `.flex-col`, `.grid`, `.grid-cols-5`, `.items-center`, `.justify-center`
- Spacing: `.p-*`, `.mb-*`, `.gap-*` (1-6), `.mx-auto`
- Colors: CSS variables only (no hardcoded colors)

**No external frameworks**—all styling is custom. Avoid inline styles; use utility classes.

## Brutalist Blocks Design Guide

The Soc Ops interface uses a high-contrast, constructivist visual language called **Brutalist Blocks**. Keep this direction consistent when changing the game UI:

- **Tone**: Treat the interface like a social field kit or printed event poster: bold, direct, energetic, and easy to scan.
- **Palette**: Use the CSS tokens in `app.css` (`--ink`, `--paper`, `--acid`, `--signal`, `--sky`, and `--mint`). Do not add hardcoded colors to templates or new components.
- **Typography**: Use the existing display and body font tokens (`--font-display` and `--font-body`). Display type is reserved for branding, section headings, labels, and major game states.
- **Geometry**: Prefer square corners, thick dark borders, offset block shadows, strong alignment, and restrained geometric textures. Avoid soft cards, pill-shaped controls, glass effects, and decorative gradients.
- **Game board**: Keep the board at 5x5 with stable cell dimensions. Preserve clear visual differences between idle, marked, free-space, and winning cells. Prompts must wrap without horizontal overflow.
- **Interaction**: Buttons and cells need visible `hover`, `active`, `disabled`, and `:focus-visible` states. Keep touch targets comfortable and preserve `aria-pressed` and `aria-label` behavior.
- **Motion**: Use short, purposeful transitions and entry animation only. Respect `prefers-reduced-motion` for all new animation or transition rules.
- **Responsive layout**: Design for narrow mobile screens first, then expand the composition for desktop. Test the lobby, board, victory banner, and modal without horizontal scrolling.
- **Scope**: Preserve `lobbyView`, `activeView`, `gridContainer`, `bingoBanner`, and `victoryOverlay`, along with their existing global handlers and local-storage snapshot format.

When adding a new visual element, prefer a semantic class in `app.css` over inline styles or a new dependency. Keep the interface in English unless a localization task explicitly changes that requirement.

## API Endpoints

| Endpoint | Method | Response |
|----------|--------|----------|
| `/` | GET | Game HTML page |
| `/api/bingo/fresh-board` | GET | JSON array of `BingoCell` objects |

## Development Workflow

**Adding Features**: Model → Service → Web endpoint → Template → CSS

**Modify Board Logic**: Edit `BoardAssembler.java` or `IcebreakerPrompts.java` (questions)

**New CSS**: Add utility classes to `app.css` following `.property-value` pattern

**Testing**: Add tests in `src/test/java/com/socops/service/` using JUnit 5. Use Spring DevTools for hot reload during dev.

## Files to Reference

- `.github/instructions/css-utilities.instructions.md` — CSS utilities guide
- `.github/instructions/frontend-design.instructions.md` — Frontend design best practices
- `workshop/GUIDE.md` — Lab exercises
- `pom.xml` — Dependencies

## Key Points

- **Spring DevTools**: Hot reload on file changes—no server restart needed
- **Tests must pass**: Run full checklist before any push
- Multi-language docs: Maintain English, Portuguese (BR), Spanish parity
- Auto-deploys to GitHub Pages on push to `main`
