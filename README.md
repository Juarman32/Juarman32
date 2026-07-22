<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=28&duration=3000&pause=1000&color=00E5FF&center=true&vCenter=true&width=600&lines=JUARMAN;Sys+Admin+%7C+Ciberseguridad;Automatizaci%C3%B3n+%7C+Self-Hosting;Vibe+Coding+Enjoyer+%F0%9F%8E%B8" alt="Typing SVG" />
</p>

<p align="center">
  <samp>Barcelona 🇪🇸 · Canary Islands 🌴</samp>
</p>

<p align="center">
  <a href="https://www.proxmox.com/"><img src="https://img.shields.io/badge/Proxmox-E57000?style=for-the-badge&logo=proxmox&logoColor=white" /></a>
  <a href="https://docker.com"><img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" /></a>
  <a href="https://nginx.org"><img src="https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white" /></a>
  <a href="https://kernel.org"><img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" /></a>
  <a href="https://python.org"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" /></a>
  <a href="https://typescriptlang.org"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" /></a>
  <a href="https://react.dev"><img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" /></a>
  <a href="https://rust-lang.org"><img src="https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white" /></a>
</p>

---

## 🧠 Filosofía

> *"No describas lo que harías. Hazlo. Si falla, reconstrúyelo desde cero. Si funciona, que sea limpio, rápido y bonito."*

Soy un **Sys Admin en formación** obsesionado con la automatización, la infraestructura self-hosted y la ciberseguridad. Creo en el **modo YOLO**: máxima autonomía, mínima fricción. Mis proyectos no se planean eternamente — se construyen, se rompen, se arreglan y se despliegan.

### 🎸 Vibe Coding Enjoyer

Soy un firme defensor del **vibe coding**. ¿Documentación? La justa. ¿Planificación? Un README y pa'lante. Mi flujo de trabajo consiste en abrir el editor, poner música, y dejar que el código fluya como si fuese jazz — a veces suena glorioso, a veces es ruido, pero siempre es auténtico.

> *"El 90% de mis commits son `fix: lol`, `feat: vibes`, y `chore: esto no debería funcionar pero funciona`. El otro 10% son reverts de los primeros."*

Si el código compila a la primera, desconfío. Si tuve que hacer `git reset --hard` 3 veces antes del PR final, entonces sé que el proyecto va por buen camino.

**Principios del Vibe Coding según juarman:**

- 🚀 `git push --force` no es un bug, es un estilo de vida
- 🎯 Si funciona, no lo toques... demasiado
- 🧪 Testear en producción es la única forma de saber si realmente funciona
- 📝 Los comentarios son para los débiles (el código se explica solo... o no)
- 🤖 Si una IA puede escribirlo en 30s, ¿para qué pasar 3h haciéndolo a mano?

Mi laboratorio es un **Proxmox VE** donde virtualizo mi propio ecosistema: contenedores Docker, VMs con GPU passthrough, reverse proxies con Nginx, stacks LAMP/MEAN, y un equipo de **agentes de IA autónomos** que trabajan para mí en un tablero Kanban.

---

## 🏗️ Infraestructura

### 🖥️ Proxmox VE — `zanarkand`

> Hipervisor principal · `192.168.88.10`

| ID | Hostname | Rol | Stack |
|---|---|---|---|
| **CT 100** | `hermes-agent` | IA + Automatización | Docker |
| **CT 103** | `sapientia-osint` | OSINT Platform | OSIRIS, SpiderFoot |
| **CT 110** | `bitwarden-vault` | Password Manager | Vaultwarden, Nginx, SSL |
| **VM 200** | `cachyos-gaming` | Gaming + GPU | 8GB, GPU Passthrough |

### 🔧 Stack

```
Nginx Reverse Proxy (SSL · Fail2ban · Rate Limit)
├── Docker Compose
├── Proxmox LXC Containers
├── Hermes Agent (IA + Multi-Agente Kanban)
└── Python · TypeScript · React · Rust
```

---

## 🚀 Proyectos

### 🕵️ Sapientia OSINT

![Status](https://img.shields.io/badge/Status-Active-00E5FF?style=flat-square)
![Stack](https://img.shields.io/badge/Stack-Docker_|_Python_|_Nginx-D4AF37?style=flat-square)

Plataforma de inteligencia de fuentes abiertas auto-hospedada. Integra **SpiderFoot**, **OSIRIS**, y APIs OSINT para recolección y análisis de datos.

```
osiris/      → Framework OSINT principal
spiderfoot/  → Automatización de reconocimiento
tools/       → API OSINT interna
```

---

### 📊 ShiftPlanner

![Status](https://img.shields.io/badge/Status-Completed-00E5FF?style=flat-square)
![Stack](https://img.shields.io/badge/Stack-Vite_|_React_19_|_sql.js_|_Zustand-D4AF37?style=flat-square)

Aplicación web de gestión de cuadrantes laborales con turnos rotativos, vacaciones, bajas, festivos y reglas complejas de planificación. 100% client-side — **sql.js + IndexedDB** sin backend.

- ✅ 24/24 tests pasando
- ✅ Build de producción ~472KB
- ✅ Modo offline-first auto-contenido

---

### 🌐 Nexus Feed

![Status](https://img.shields.io/badge/Status-In_Progress-00E5FF?style=flat-square)
![Stack](https://img.shields.io/badge/Stack-Next.js_|_Framer_Motion_|_TypeScript-D4AF37?style=flat-square)

Proyecto web con diseño **cyberpunk glassmorphism** — estética oscura, neones cyan + gold, scanlines, mesh backgrounds, Server Components por defecto, animaciones con Framer Motion.

---

### 🔐 Bitwarden Vault

![Status](https://img.shields.io/badge/Status-Deployed-00E5FF?style=flat-square)

Gestor de contraseñas self-hosted con **Vaultwarden** sobre Docker en LXC. Nginx con SSL, Fail2ban, rate limiting. Backups diarios automáticos (zstd, 7 días de retención). Integración nativa con Hermes Agent vía CLI + plugin.

---

### 📡 VPN Streaming Guide

![Status](https://img.shields.io/badge/Status-Documented-00E5FF?style=flat-square)

Guía de infraestructura VPN para streaming — documentación completa con stack networking, configuración de túneles, y optimización para acceso geográfico.

---

## 🤖 Multi-Agente Kanban

Mi equipo de **5 agentes de IA autónomos** trabajando en tablero Kanban:

| Agente | Rol | Especialidad |
|---|---|---|
| 🧙 **Merovingio** | Investigador | Análisis tecnológico, viabilidad, mejores prácticas |
| 🏛️ **Arquitecto** | Diseñador | Estructura, stack técnico, arquitectura |
| 🔨 **Constructor** | Developer | Implementación, código, tests, docs |
| 🔍 **Revisor** | QA Engineer | Code review, seguridad, rendimiento |
| ✅ **Verificador** | Aprobador | Veredicto final, ZIP de entrega |

**Pipeline:** `research → design → build → review → verify → deploy`

Orquestado desde **Hermes Agent** con notificaciones vía Telegram.

---

## 🎨 Design System

| Token | Value |
|---|---|
| 🌑 Background | `#06060c` |
| 💎 Cyan | `#00E5FF` |
| 🥇 Gold | `#D4AF37` |
| 🧊 Glass | `backdrop-filter: blur()` |
| 📝 Fonts | Inter (UI) + JetBrains Mono (code) |
| 🌐 Mesh | Subtle gradient background |
| 📟 Scanline | 5% overlay |

**Reglas:** Dark mode siempre · Glassmorphism · Nunca Bootstrap · Animaciones sutiles · Diseño moderno y pulido

---

## 📊 Stats

<p align="center">
  <a href="https://github.com/Juarman32">
    <img height="180em" src="https://github-readme-stats.vercel.app/api?username=Juarman32&show_icons=true&theme=tokyonight&hide_border=true&bg_color=06060c&title_color=00E5FF&icon_color=D4AF37&text_color=888888" />
    <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Juarman32&layout=compact&theme=tokyonight&hide_border=true&bg_color=06060c&title_color=00E5FF&text_color=888888" />
  </a>
</p>

---

<p align="center">
  <samp>
    <a href="https://github.com/Juarman32">github</a> ·
    <a href="https://www.proxmox.com/">proxmox</a>
  </samp>
</p>

<p align="center">
  <samp><i>"How to learn about everything."</i></samp>
</p>

<p align="center">
  <samp>🐧 Sys Admin · Ciberseguridad · Open Source · Automatización · Self-Hosting 🔐</samp>
</p>
