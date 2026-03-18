# 🔍 osint-phishing-walkthrough

<div align="center">

![OSINT](https://img.shields.io/badge/OSINT-Phishing%20Investigation-00d4ff?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0xMiAyQzYuNDggMiAyIDYuNDggMiAxMnM0LjQ4IDEwIDEwIDEwIDEwLTQuNDggMTAtMTBTMTcuNTIgMiAxMiAyem0xIDE3aC0ydi02aDJ2NnptMC04aC0yVjdoMnYyeiIvPjwvc3ZnPg==)
![Tier](https://img.shields.io/badge/Tier%201%20%7C%202%20%7C%203-Escalation%20Model-2ed573?style=for-the-badge)
![Free Tools](https://img.shields.io/badge/Tools-100%25%20Free-ffa502?style=for-the-badge)
![Language](https://img.shields.io/badge/Language-EN%20%7C%20ES--PR-ff4757?style=for-the-badge)

**A tiered, practical walkthrough for investigating email phishing campaigns using free OSINT tools.**  
**Una guía práctica y escalonada para investigar campañas de phishing usando herramientas OSINT gratuitas.**

</div>

---

## 🇺🇸 English

### 📖 About / Description

This repository contains a fully interactive HTML walkthrough designed to guide security professionals, SOC analysts, IT administrators, and cybersecurity students through the process of investigating suspicious email phishing campaigns using **free, open-source intelligence (OSINT) tools** — no paid subscriptions required.

The guide follows a **three-tier escalation model**:

| Tier | Focus | Audience |
|------|-------|----------|
| 🟢 Tier 1 | Triage & Surface Analysis | L1 SOC Analyst / Help Desk |
| 🟡 Tier 2 | Deep Link & Payload Analysis | L2 SOC Analyst |
| 🔴 Tier 3 | Threat Actor & Campaign Mapping | L3 Analyst / Threat Intel Team |

Each tier includes step-by-step instructions, mock UI screenshots, analyst tips, and clear escalation triggers so you always know when to move to the next level.

---

### 🛠 Tools Used

All tools featured in this walkthrough are **free to use** with no account required (unless noted).

| Tool | URL | Tier | Purpose |
|------|-----|------|---------|
| 📧 Google Admin Toolbox | [toolbox.googleapps.com](https://toolbox.googleapps.com/apps/messageheader/) | Tier 1 | Email header parsing & SPF/DKIM/DMARC analysis |
| 🔍 MXToolbox | [mxtoolbox.com](https://mxtoolbox.com) | Tier 1 | DNS lookup, blacklist checks, WHOIS |
| 🛡 VirusTotal | [virustotal.com](https://www.virustotal.com) | Tier 2 | URL, file & hash scanning (70+ AV engines) |
| 🌐 URLScan.io | [urlscan.io](https://urlscan.io) | Tier 2 | Safe live URL inspection & redirect chain analysis |
| 🕸 Maltego CE | [maltego.com/maltego-community](https://www.maltego.com/maltego-community/) | Tier 3 | Infrastructure graph mapping & pivot analysis |
| 🎣 PhishTank | [phishtank.org](https://phishtank.org) | Tier 3 | Community phishing URL database |
| 🎣 OpenPhish | [openphish.com](https://openphish.com) | Tier 3 | Automated phishing feed & blocklist |

---

### 🚀 How to Use / Getting Started

**No installation required.** This is a standalone HTML file that runs entirely in your browser.

**Step 1 — Clone the repository:**
```bash
git clone https://github.com/boricua/osint-phishing-walkthrough.git
cd osint-phishing-walkthrough
```

**Step 2 — Open the walkthrough:**
```bash
# Simply open the file in any modern web browser
open osint_phishing_walkthrough.html

# Or on Windows:
start osint_phishing_walkthrough.html

# Or on Linux:
xdg-open osint_phishing_walkthrough.html
```

**Step 3 — Follow the tiers in order:**
- Start at **Tier 1** with a suspicious email's raw headers
- Escalate to **Tier 2** if authentication failures or blacklist hits are found
- Escalate to **Tier 3** for campaign mapping and threat actor attribution

> 💡 **Tip:** Always have a suspicious email's raw headers ready before starting. In Gmail, use `More → Show Original`. In Outlook, use `File → Properties → Internet Headers`.

---

### 👤 Author / Contact Info

| | |
|---|---|
| **Name** | Andres Rafael Maldonado |
| **LinkedIn** | [linkedin.com/in/boricua](https://linkedin.com/in/boricua) |
| **Published** | March 18, 2026 |
| **Background** | Systems Engineer @ Oracle · B.S. Computer Information Systems (Digital Forensics) · DeVry University |

---

### ⚖️ Disclaimer / Legal Notice

> This walkthrough is intended **strictly for educational and defensive security purposes**. All tools referenced are publicly available and free to use. The phishing indicators, IP addresses, and domains shown in the mock screenshots are **fictional examples created for illustration only** and do not represent real active threats.
>
> The author assumes **no liability** for misuse of the techniques or tools described in this guide. Always obtain proper authorization before investigating systems or networks you do not own. Unauthorized access to computer systems is illegal under the Computer Fraud and Abuse Act (CFAA) and equivalent laws in other jurisdictions.
>
> Use this knowledge responsibly. 🛡

---
---

## 🇵🇷 Español (Puerto Rico)

### 📖 Descripción

Este repositorio contiene una guía interactiva en formato HTML diseñada para orientar a profesionales de seguridad, analistas de SOC, administradores de TI y estudiantes de ciberseguridad en el proceso de investigar campañas sospechosas de phishing por correo electrónico usando **herramientas gratuitas de inteligencia de fuente abierta (OSINT)** — sin necesidad de suscripciones de pago.

La guía sigue un **modelo de escalación de tres niveles**:

| Nivel | Enfoque | Audiencia |
|-------|---------|-----------|
| 🟢 Nivel 1 | Triaje y Análisis Superficial | Analista L1 / Mesa de Ayuda |
| 🟡 Nivel 2 | Análisis Profundo de Enlaces y Cargas | Analista L2 SOC |
| 🔴 Nivel 3 | Mapeo de Actores y Campañas | Analista L3 / Equipo de Inteligencia |

Cada nivel incluye instrucciones paso a paso, capturas de pantalla simuladas, notas del analista, y detonantes claros de escalación para que siempre sepas cuándo avanzar al siguiente nivel.

---

### 🛠 Herramientas Utilizadas

Todas las herramientas en esta guía son **gratuitas** y no requieren cuenta (salvo indicación contraria).

| Herramienta | URL | Nivel | Propósito |
|-------------|-----|-------|-----------|
| 📧 Google Admin Toolbox | [toolbox.googleapps.com](https://toolbox.googleapps.com/apps/messageheader/) | Nivel 1 | Análisis de encabezados y verificación SPF/DKIM/DMARC |
| 🔍 MXToolbox | [mxtoolbox.com](https://mxtoolbox.com) | Nivel 1 | Búsqueda DNS, listas negras, WHOIS |
| 🛡 VirusTotal | [virustotal.com](https://www.virustotal.com) | Nivel 2 | Escaneo de URLs, archivos y hashes (70+ motores AV) |
| 🌐 URLScan.io | [urlscan.io](https://urlscan.io) | Nivel 2 | Inspección segura de URLs y análisis de cadenas de redirección |
| 🕸 Maltego CE | [maltego.com/maltego-community](https://www.maltego.com/maltego-community/) | Nivel 3 | Mapeo gráfico de infraestructura y análisis de pivote |
| 🎣 PhishTank | [phishtank.org](https://phishtank.org) | Nivel 3 | Base de datos comunitaria de URLs de phishing |
| 🎣 OpenPhish | [openphish.com](https://openphish.com) | Nivel 3 | Feed automatizado de phishing y listas de bloqueo |

---

### 🚀 Cómo Usar / Instrucciones de Inicio

**No se requiere instalación.** Este es un archivo HTML independiente que corre completamente en tu navegador.

**Paso 1 — Clona el repositorio:**
```bash
git clone https://github.com/boricua/osint-phishing-walkthrough.git
cd osint-phishing-walkthrough
```

**Paso 2 — Abre la guía:**
```bash
# Abre el archivo en cualquier navegador moderno
open osint_phishing_walkthrough.html

# En Windows:
start osint_phishing_walkthrough.html

# En Linux:
xdg-open osint_phishing_walkthrough.html
```

**Paso 3 — Sigue los niveles en orden:**
- Comienza en el **Nivel 1** con los encabezados sin procesar de un correo sospechoso
- Escala al **Nivel 2** si se encuentran fallas de autenticación o resultados en listas negras
- Escala al **Nivel 3** para mapeo de campañas y atribución de actores de amenaza

> 💡 **Consejo:** Ten siempre listos los encabezados sin procesar del correo sospechoso antes de comenzar. En Gmail, usa `Más → Mostrar Original`. En Outlook, usa `Archivo → Propiedades → Encabezados de Internet`.

---

### 👤 Autor / Información de Contacto

| | |
|---|---|
| **Nombre** | Andres Rafael Maldonado |
| **LinkedIn** | [linkedin.com/in/boricua](https://linkedin.com/in/boricua) |
| **Publicado** | 18 de marzo de 2026 |
| **Trasfondo** | Ingeniero de Sistemas @ Oracle · B.S. en Sistemas de Información (Forense Digital) · DeVry University |

---

### ⚖️ Aviso Legal / Descargo de Responsabilidad

> Esta guía está destinada **estrictamente para propósitos educativos y de seguridad defensiva**. Todas las herramientas mencionadas son de acceso público y gratuitas. Los indicadores de phishing, direcciones IP y dominios mostrados en las capturas de pantalla simuladas son **ejemplos ficticios creados solo con fines ilustrativos** y no representan amenazas activas reales.
>
> El autor **no asume responsabilidad alguna** por el mal uso de las técnicas o herramientas descritas en esta guía. Siempre obtén la autorización adecuada antes de investigar sistemas o redes que no sean de tu propiedad. El acceso no autorizado a sistemas informáticos es ilegal bajo el Computer Fraud and Abuse Act (CFAA) y leyes equivalentes en otras jurisdicciones.
>
> Usa este conocimiento de forma responsable. 🛡

---

<div align="center">

*Built with purpose · Construido con propósito* 🇵🇷

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Andres%20Rafael%20Maldonado-0077B5?style=flat&logo=linkedin)](https://linkedin.com/in/boricua)

</div>
