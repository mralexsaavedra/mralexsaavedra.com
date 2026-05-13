# Alexander Saavedra González

**Senior Software Engineer — Frontend**
Barakaldo, Bizkaia · mralexsaavedra@gmail.com · [mralexsaavedra.com](https://mralexsaavedra.com) · [github.com/mralexsaavedra](https://github.com/mralexsaavedra) · [linkedin.com/in/mralexsaavedra](https://linkedin.com/in/mralexsaavedra)

---

## Resumen

9 años con JavaScript/TypeScript en producción. Trabajo bien tanto en producto como en
arquitectura: Clean Architecture y DDD en el frontend, monorepos, mobile con React Native
y full-stack cuando hace falta. Contribuyo a proyectos Open Source y tengo un flujo de
trabajo con IA estructurado: Claude Code y Opencode como herramientas de desarrollo,
Engram para memoria persistente entre sesiones y SDD (Spec-Driven Development) para
cambios con impacto arquitectónico.

---

## Stack Técnico

**Frontend:** React 19/18, TypeScript, React Router v7, TanStack Query, Zustand, Tailwind CSS v4, SASS, Vite, Astro

**Mobile:** React Native, Expo, React Native Web

**Testing:** Vitest, Jest, Playwright, Cypress, Detox, Testing Library (React, DOM, user-event)

**Arquitectura:** Clean Architecture, Domain-Driven Design, Hexagonal Architecture, Monorepo (pnpm + Turbo)

**Backend / APIs:** Node.js, Express, Prisma, SQLite, Redis, BullMQ, Zod

**Tooling / DX:** ESLint, Oxlint, Prettier, Husky, lint-staged, Claude Code, Opencode, Engram, SDD

**Infraestructura:** Docker, Docker Compose, Traefik, Proxmox, LXC, GitHub Actions

**Otros:** Python, i18next, React Intl, Sentry

---

## Experiencia Profesional

### Lookiero — Front-end Engineer

`Mar 2022 – Presente · Bilbao (remoto)`

- Monorepo de frontend a escala: 8 aplicaciones y 22 paquetes compartidos en el mismo repo
  (npm workspaces + Turbo). Codebase multi-plataforma con React para web y React Native +
  Expo para mobile, compartiendo lógica via react-native-web.
- Clean Architecture y DDD en el frontend: capas `domain / application / infrastructure`
  por módulo, lo que permite test unitario sin montar el framework y reduce el tiempo de
  onboarding de nuevos desarrolladores al aislar la lógica de negocio del framework.
- Configuración centralizada como workspace packages propios: ESLint, Prettier, TypeScript
  y Jest compartidos entre todas las aplicaciones del repo.
- CI/CD con jobs paralelos (lint, build, test, Cypress) y caché Turbo en GitHub Actions,
  reduciendo tiempos de pipeline en el monorepo.
- Decisiones de arquitectura transversal: contratos de API, estado global, boundaries de
  módulos e i18n.

### Kira Health — Front-end Developer

`Nov 2020 – Feb 2022 · Bilbao`

- Producto de salud digital en React y TypeScript. Flujos críticos de datos de paciente
  donde el estado bien modelado y la cobertura de tests no eran opcionales.

### S&M Services — Full Stack Developer

`Oct 2018 – Nov 2019 · Bilbao`

- Aplicaciones de gestión para cliente corporativo: diseño de API, base de datos, interfaz
  y puesta en producción.

### Inycom — Full Stack Developer

`Sep 2017 – Sep 2018 · Bilbao`

- Desarrollo e integración de servicios TIC para clientes del sector corporativo y público.

### Shackleton — Full Stack Developer

`Feb 2017 – Ago 2017 · Bilbao`

- Renovación de herramientas internas en JavaScript y MySQL.

---

## Proyectos Open Source

### [spotiarr](https://github.com/mralexsaavedra/spotiarr) — 27 ★ · 5 forks

Descargador de Spotify self-hosted con integración Jellyfin/Plex. Proyecto completo con
650+ commits: React 19, TypeScript, Express, Prisma, SQLite, Redis, BullMQ, Docker Compose
y Traefik. Cola asíncrona de trabajos, detección de duplicados, embedding de metadatos y
sincronización en tiempo real vía Server-Sent Events. CI/CD con GitHub Actions y builds
multi-arquitectura (amd64/arm64) publicados en Docker Hub. Referencia pública de cómo
aplicar DDD y Clean Architecture en un producto full-stack real.

### [koma](https://github.com/mralexsaavedra/koma)

Gestor de cómics self-hosted en TypeScript. Monorepo con capas explícitas: `core` (lógica
de dominio sin ninguna dependencia de framework), `database` (adaptador Prisma),
`metadata` (Google Books, AniList) y `cli`. El core es completamente testable en aislamiento.

### [jellytube](https://github.com/mralexsaavedra/jellytube)

Microservicio en TypeScript que genera `.strm` y `.nfo` para Jellyfin/Plex a partir de
contenido de YouTube, sin almacenamiento local. Monorepo con dos paquetes: ingesta de
metadatos y resolución de URLs de stream en tiempo real.

### [spotdl-bot](https://github.com/mralexsaavedra/spotdl-bot) — 11 ★

Bot de Telegram en Python para descarga automatizada de música desde Spotify. Mencionado
en el [podcast Desde el Reloj](https://www.desdeelreloj.com/e1145/).

### Contribuciones al ecosistema Orca

Tres features en el IDE Orca (TypeScript, Electron, xterm.js, Monaco Editor): panel de
source control con commit/push/pull/sync, tracking de rate-limits para Gemini y OpenCode,
e importación de configuración Ghostty con preview en tiempo real. Contribuciones de nivel
de feature en una base de código compleja de terceros con más de 1.500 commits.

---

## Infraestructura Personal

Servidor doméstico con **Proxmox** como hipervisor, contenedores **LXC** y stacks **Docker**
para servicios self-hosted: Jellyfin, spotiarr, Traefik.

---

## Comunidad

**Google Developers Group Bilbao — Co-organizador** `Ene 2019 – Nov 2019`
Organización de eventos técnicos y construcción de comunidad de ingeniería en Bizkaia.

---

## Educación

**Grado en Ingeniería Informática de Gestión y Sistemas de Información**
Universidad del País Vasco (UPV/EHU) · 2013 – 2018

**Máster Avanzado en Animación**
Lightbox Academy · 2019 – 2020

---

## Idiomas

- Español: Nativo
- Euskera: C1 (certificado Eusko Jaurlaritza)
- Inglés: Profesional (lectura técnica diaria)
