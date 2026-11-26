<div align="center">
  <img src="assets/hero.svg" alt="Juarman — sysadmin, homelab y ciberseguridad" width="100%" />
</div>

<p align="center">
  <em>Infraestructura propia, decisiones medidas y poca fe en el software que no puedo auditar.</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Proxmox-161B22?style=flat-square&logo=proxmox&logoColor=8B949E&labelColor=0D1117" />
  <img src="https://img.shields.io/badge/Docker-161B22?style=flat-square&logo=docker&logoColor=8B949E&labelColor=0D1117" />
  <img src="https://img.shields.io/badge/Linux-161B22?style=flat-square&logo=linux&logoColor=8B949E&labelColor=0D1117" />
  <img src="https://img.shields.io/badge/Nginx-161B22?style=flat-square&logo=nginx&logoColor=8B949E&labelColor=0D1117" />
  <img src="https://img.shields.io/badge/Cloudflare-161B22?style=flat-square&logo=cloudflare&logoColor=8B949E&labelColor=0D1117" />
  <br />
  <img src="https://img.shields.io/badge/Python-161B22?style=flat-square&logo=python&logoColor=8B949E&labelColor=0D1117" />
  <img src="https://img.shields.io/badge/TypeScript-161B22?style=flat-square&logo=typescript&logoColor=8B949E&labelColor=0D1117" />
  <img src="https://img.shields.io/badge/Rust-161B22?style=flat-square&logo=rust&logoColor=8B949E&labelColor=0D1117" />
  <img src="https://img.shields.io/badge/C%23_%2F_.NET-161B22?style=flat-square&logo=dotnet&logoColor=8B949E&labelColor=0D1117" />
  <img src="https://img.shields.io/badge/C%2B%2B-161B22?style=flat-square&logo=cplusplus&logoColor=8B949E&labelColor=0D1117" />
</p>

---

## whoami

Soy Juarman. Administro sistemas, rompo los míos para entenderlos y los vuelvo a levantar cuando ya sé exactamente por qué fallaban.

Mi día a día es infraestructura: un hipervisor Proxmox, contenedores LXC y Docker, proxies inversos, backups que de verdad restauran y una VPN que cierra la puerta desde fuera. No es un laboratorio de juguete: es lo que sostiene mis servicios, mi gestor de contraseñas y los agentes de IA que me echan una mano.

No vengo de un CV lleno de certificados. Vengo de haber roto algo a las dos de la mañana, arreglarlo y escribir después qué había pasado para no repetirlo.

---

## cómo trabajo

Cuatro reglas que me ahorran disgustos:

| Principio | Lo que significa |
|---|---|
| **Primero mido, después toco** | Ningún cambio se justifica con «debería ir mejor». Se justifica con números de antes y de después. |
| **Si no es reversible, no es un cambio** | Punto de restauración, copia del archivo, la versión anterior al lado. Volver atrás tiene que seguir siendo posible. |
| **Prefiero lo pequeño a lo completo** | Una herramienta que entiendo entera vale más que una suite de la que uso el 5 %. |
| **Lo que no está escrito, no existe** | Cada decisión y cada error acaban documentados. Sobre todo los errores. |

> *Vibe coding sí, pero con recibo: la IA acelera la primera versión; la segunda la escribe la medición.*

---

## el laboratorio

Un hipervisor, un puñado de contenedores y una norma: cada servicio con un trabajo claro y una forma de volver atrás.

| Contenedor | Qué corre dentro |
|---|---|
| `docker` | Hermes Agent, Portainer y la pila de observabilidad (Promtail + Loki) |
| `tunnel` | Cloudflare Tunnel: servicios publicados sin abrir un solo puerto |
| `utils` | PriceBuddy, ChangeDetection y las herramientas OSINT |
| `vpn` | pasarela VPN para salida y entrada cifrada |
| `vault` | Vaultwarden con backups comprimidos y retención de siete días |

```text
proxmox
├── docker ────── hermes · portainer · loki
├── tunnel ────── cloudflare tunnel
├── utils ─────── pricebuddy · changedetection · osint
├── vpn ───────── pasarela cifrada
└── vault ─────── vaultwarden (backup diario, 7 días)
```

Cada contenedor tiene un propósito y un límite. Lo que no aporta, se apaga; lo que se apaga, se documenta.

---

## el equipo

No trabajo solo: tengo un tablero Kanban y cinco agentes con roles fijos. Cada tarjeta entra por investigación y no sale hasta que alguien la ha revisado.

| Rol | Qué hace |
|---|---|
| **Merovingio** | investiga: viabilidad, alternativas y coste real de cada opción |
| **Arquitecto** | decide estructura, stack y, sobre todo, qué se descarta |
| **Constructor** | implementa, prueba y deja el build en verde |
| **Revisor** | audita código, seguridad y rendimiento |
| **Desbloqueador** | rescata lo que lleva demasiado tiempo atascado |

```text
research  →  design  →  build  →  review  →  deploy
```

El orquestador es Hermes Agent, mi propio asistente, y el tablero vive en la misma infraestructura que todo lo demás.

---

## ia local

16 GB de VRAM y una regla: los datos que no necesito fuera de casa, no salen.

- **llama.cpp** compilado contra Vulkan, con modelos GGUF en cuantizaciones agresivas.
- **Modelos MoE con offload parcial**: la parte caliente en VRAM, el resto en RAM.
- Un **router propio con watchdog** que decide qué motor atiende cada petición.
- Experimentos con motores alternativos cuando prometen más tokens por vatio. Y medición para comprobarlo.

La IA local no es una demo: es la razón por la que puedo trabajar con datos que no subiría a una API.

---

## proyectos

| Proyecto | Qué es | Stack |
|---|---|---|
| **Hermes Agent** | orquestador con agentes, tablero Kanban y plugins propios, incluido REA para ingeniería inversa (Ghidra, Frida, rizin) | Python · MCP |
| **Lumen** | estudio de fondos de pantalla procedurales: genera, previsualiza y exporta | C# / .NET |
| **StartRed** | recolorea el orbe de Inicio y la barrita del taskbar de Windows 11 desde dentro del shell | C++ · DLL · hooks |
| **NZXT Lite** | control del RGB de NZXT por HID, con los efectos en el firmware del controlador: 2 MB y 0 % de CPU en reposo | C# / .NET |
| **Sapientia** | plataforma OSINT autoalojada: recolección, correlación y paneles | Docker · Python |
| **ShiftPlanner** | cuadrantes de turnos rotativos con festivos, bajas y reglas de planificación; 100 % en el navegador, sin backend | React 19 · sql.js · IndexedDB |

---

## stack

```text
sistemas      proxmox · lxc · docker · systemd · zfs · nginx
red           cloudflare tunnel · wireguard · dns · firewalls
lenguajes     python · typescript · rust · c# · c++ · sql
ia            llama.cpp · gguf · moe · rag · mcp
herramientas  ghidra · frida · rizin · git · obsidian
```

---

## criterio de diseño

| Pieza | Valor |
|---|---|
| Fondo | `#07080B` |
| Texto | `#F2F5F9` |
| Acento | `#00E5FF`, uno solo y con moderación |
| Tipografía | sistema para interfaz, monoespaciada para datos |
| Regla | menos color, más aire. Si dudo, lo quito |

Vengo del neón y del glassmorphism. Sigo usando el mismo negro, pero cada vez me interesa más lo que no se ve: jerarquía, contraste y espacio.

---

## ahora

Cosas que estoy tocando estos meses:

- Afinar la IA local: cuantizaciones, offload y un router que elija motor sin que yo tenga que pensarlo.
- Quitar de mi PC el último software de fabricante que sigue pidiendo más de lo que da.
- Llevar todo a la medición: temperaturas, latencias, tokens por segundo y vatios. Lo que no se mide, no se mejora.

---

## fuera de la terminal

Guitarra eléctrica y amplificadores simulados: tengo una carpeta de presets que va de Mägo de Oz a System of a Down. Algún RPG de mundo abierto cuando el día ha sido largo. Y un vault de Obsidian donde acaba todo lo que aprendo, incluso lo que preferiría olvidar.

---

<p align="center">
  <samp>«How to learn about everything.»</samp>
</p>
