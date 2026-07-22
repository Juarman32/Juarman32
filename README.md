<div align="center">

```
   ██╗██╗   ██╗ █████╗ ██████╗ ███╗   ███╗ █████╗ ███╗   ██╗
   ██║██║   ██║██╔══██╗██╔══██╗████╗ ████║██╔══██╗████╗  ██║
   ██║██║   ██║███████║██████╔╝██╔████╔██║███████║██╔██╗ ██║
  ██╔╝██║   ██║██╔══██║██╔══██╗██║╚██╔╝██║██╔══██║██║╚██╗██║
  ██╔╝ ╚██████╔╝██║  ██║██║  ██║██║ ╚═╝ ██║██║  ██║██║ ╚████║
  ╚═╝   ╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝     ╚═╝╚═╝  ╚═╝╚═╝  ╚═══╝
</div>

<br>

### Sys Admin · Ciberseguridad · Automatización · Infraestructura Self-Hosted

Barcelona 🇪🇸 · Canary Islands 🌴

[![Proxmox](https://img.shields.io/badge/Proxmox-E57000?style=for-the-badge&logo=proxmox&logoColor=white)](https://www.proxmox.com/)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://docker.com)
[![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)](https://nginx.org)
[![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://kernel.org)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://typescriptlang.org)
[![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev)
[![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)](https://rust-lang.org)

---

## 🧠 Filosofía

> *"No describas lo que harías. Hazlo. Si falla, reconstrúyelo desde cero. Si funciona, que sea limpio, rápido y bonito."*

Soy un **Sys Admin en formación** obsesionado con la automatización, la infraestructura self-hosted y la ciberseguridad. Creo en el **modo YOLO**: máxima autonomía, mínima fricción. Mis proyectos no se planean eternamente — se construyen, se rompen, se arreglan y se despliegan. 

### 🎸 Vibe Coding Enjoyer

Soy un firme defensor del **vibe coding**. ¿Documentación? La justa. ¿Planificación? Un README y pa'lante. Mi flujo de trabajo consiste en abrir el editor, poner música, y dejar que el código fluya como si fuese jazz — a veces suena glorioso, a veces es ruido, pero siempre es auténtico.

> *"El 90% de mis commits son `fix: lol`, `feat: vibes`, y `chore: esto no debería funcionar pero funciona`. El otro 10% son reverts de los primeros."*

Si el código compila a la primera, desconfío. Si tuve que hacer `git reset --hard` 3 veces antes del PR final, entonces sé que el proyecto va por buen camino. Mis variables se llaman `cosa`, `cosita`, y `laBuena` — y si alguien pregunta, son "nombres semánticos contextuales".

**Principios del Vibe Coding según juarman:**
- 🚀 `git push --force` no es un bug, es un estilo de vida
- 🎯 Si funciona, no lo toques... demasiado
- 🧪 Testear en producción es la única forma de saber si realmente funciona
- 📝 Los comentarios son para los débiles (el código se explica solo... o no)
- 🤖 Si una IA puede escribirlo en 30s, ¿para qué pasar 3h haciéndolo a mano?

Mi laboratorio es un **Proxmox VE** donde virtualizo mi propio ecosistema: contenedores Docker, VMs con GPU passthrough, reverse proxies con Nginx, stacks LAMP/MEAN, y un equipo de **agentes de IA autónomos** que trabajan para mí en un tablero Kanban.

---

## 🏗️ Infraestructura

<table>
<tr>
<td width="50%">

### 🖥️ Proxmox VE — `zanarkand`
> Hipervisor principal · 192.168.88.10

| ID | Hostname | Rol | Specs |
|---|---|---|---|
| **CT 100** | hermes-agent | IA + Automatización | Docker |
| **CT 103** | sapientia-osint | OSINT Platform | OSIRIS, SpiderFoot |
| **CT 110** | bitwarden-vault | Password Manager | Vaultwarden + SSL |
| **VM 200** | cachyos-gaming | Gaming + GPU | 8GB, GPU Passthrough |

</td>
<td width="50%">

### 🔧 Stack Principal

```
┌─────────────────────────────────┐
│         Nginx Reverse Proxy      │
│      SSL · Fail2ban · Rate Limit │
├─────────────────────────────────┤
│  ┌──────────┐  ┌──────────────┐  │
│  │ Docker   │  │  Proxmox LXC │  │
│  │ Compose  │  │  Containers  │  │
│  └──────────┘  └──────────────┘  │
├─────────────────────────────────┤
│  ┌──────────┐  ┌──────────────┐  │
│  │ Hermes   │  │  Kanban      │  │
│  │ Agent    │  │  Multi-Agent │  │
│  └──────────┘  └──────────────┘  │
├─────────────────────────────────┤
│  Python · TS · React · Rust     │
└─────────────────────────────────┘
```

</td>
</tr>
</table>

---

## 🚀 Proyectos Destacados

### 🕵️ Sapientia OSINT
[![Status](https://img.shields.io/badge/Status-Active-00E5FF?style=flat-square)](https://github.com/Juarman32)
[![Stack](https://img.shields.io/badge/Stack-Docker%20%7C%20Python%20%7C%20Nginx-D4AF37?style=flat-square)](https://github.com/Juarman32)

Plataforma de inteligencia de fuentes abiertas auto-hospedada. Integra **SpiderFoot**, **OSIRIS**, y APIs de inteligencia para recolección y análisis de datos OSINT. Desplegada en CT 103 con acceso controlado.

```
osiris/      — Framework OSINT principal
spiderfoot/  — Automatización de reconocimiento
tools/       — API OSINT interna
```

---

### 📊 ShiftPlanner
[![Status](https://img.shields.io/badge/Status-Completed-00E5FF?style=flat-square)](https://github.com/Juarman32)
[![Stack](https://img.shields.io/badge/Stack-Vite%20%7C%20React%2019%20%7C%20sql.js%20%7C%20Zustand-D4AF37?style=flat-square)](https://github.com/Juarman32)

Aplicación web de gestión de cuadrantes laborales con turnos rotativos, vacaciones, bajas, festivos y reglas complejas de planificación. Funciona completamente en el navegador sin backend — **sql.js + IndexedDB** para persistencia local.

- ✅ 24/24 tests pasando
- ✅ Build de producción ~472KB
- ✅ Modo auto-contenido (offline-first)

---

### 🌐 Nexus Feed
[![Status](https://img.shields.io/badge/Status-In_Progress-00E5FF?style=flat-square)](https://github.com/Juarman32)
[![Stack](https://img.shields.io/badge/Stack-Next.js%20%7C%20Framer%20Motion%20%7C%20TypeScript-D4AF37?style=flat-square)](https://github.com/Juarman32)

Proyecto web con diseño **cyberpunk glassmorphism** — estética oscura, neones, scanlines, mesh backgrounds. Server Components por defecto, animaciones con Framer Motion.

---

### 🔐 Bitwarden Vault
[![Status](https://img.shields.io/badge/Status-Deployed-00E5FF?style=flat-square)](https://github.com/Juarman32)

Gestor de contraseñas self-hosted con **Vaultwarden** sobre Docker en LXC. Nginx con SSL auto-firmado, Fail2ban, rate limiting. Backups diarios automáticos con retención de 7 días. Integración nativa con Hermes Agent vía CLI + plugin.

---

### 📡 VPN Streaming Guide
[![Status](https://img.shields.io/badge/Status-Documented-00E5FF?style=flat-square)](https://github.com/Juarman32)

Guía de infraestructura VPN para streaming — documentación completa con stack networking, configuración de túneles, y optimización para acceso geográfico.

---

## 🤖 Automatización con IA

Mi equipo de **5 agentes autónomos** trabajando en un tablero Kanban:

| Agente | Rol | Especialidad |
|---|---|---|
| 🧙 **Merovingio** | Investigador | Análisis tecnológico, viabilidad, mejores prácticas |
| 🏛️ **Arquitecto** | Diseñador | Estructura del proyecto, stack técnico, arquitectura |
| 🔨 **Constructor** | Developer | Implementación, código, tests, documentación |
| 🔍 **Revisor** | QA Engineer | Code review, seguridad, rendimiento, calidad |
| ✅ **Verificador** | Aprobador | Veredicto final, requisitos cumplidos, ZIP de entrega |

**Flujo:** `research → design → build → review → verify → deploy`

Todo orquestado desde **Hermes Agent** con notificaciones vía Telegram.

---

## 🎨 Diseño

Mi seña de identidad visual:

<table>
<tr>
<td>

```
┌──────────────────────────────────┐
│  🌑 bg:        #06060c           │
│  💎 cyan:      #00E5FF           │
│  🥇 gold:      #D4AF37           │
│  🧊 glass:     backdrop-blur     │
│  📝 fonts:     Inter + JetBrains │
│  🌐 mesh:      subtle gradient   │
│  📟 scanline:  overlay 5%        │
└──────────────────────────────────┘
```

</td>
<td>

- **Dark mode** siempre — `#06060c` de fondo
- **Glassmorphism** con `backdrop-filter: blur()`
- **Neones** cyan + gold sobre fondos oscuros
- **Fuentes**: Inter para UI, JetBrains Mono para código
- **Nunca Bootstrap** — diseño custom moderno
- **Animaciones** sutiles, sin excesos

</td>
</tr>
</table>

---

## 📊 Estadísticas

<div align="center">

[![GitHub Stats](https://github-readme-stats.vercel.app/api?username=Juarman32&show_icons=true&theme=tokyonight&hide_border=true&bg_color=06060c&title_color=00E5FF&icon_color=D4AF37&text_color=888888)](https://github.com/Juarman32)

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Juarman32&layout=compact&theme=tokyonight&hide_border=true&bg_color=06060c&title_color=00E5FF&text_color=888888)](https://github.com/Juarman32)

</div>

---

## 🔗 Enlaces

[![GitHub](https://img.shields.io/badge/GitHub-Juarman32-00E5FF?style=for-the-badge&logo=github)](https://github.com/Juarman32)
[![Proxmox](https://img.shields.io/badge/Proxmox-zanarkand-E57000?style=for-the-badge&logo=proxmox)](https://www.proxmox.com/)

---

<div align="center">

### 💬 *"How to learn about everything."*

🐧 **Sys Admin · Ciberseguridad · Open Source · Automatización · Self-Hosting** 🔐

</div>
