<picture>
  <source
    media="(max-width: 640px)"
    srcset="assets/hero-mobile.svg">
  <img
    src="assets/hero.svg"
    alt="Sebastián Camargo, desarrollador Full Stack Junior. Automatización e integraciones de APIs y servicios de IA."
    width="1200">
</picture>

<p align="center">
  <a href="https://www.parzkeys.com/">Portafolio</a>
  &nbsp;·&nbsp;
  <a href="https://github.com/dhait0">GitHub</a>
  &nbsp;·&nbsp;
  <a href="mailto:sebascamargo39@gmail.com">Contacto</a>
</p>

## Sobre mí

Soy Sebastián Camargo, desarrollador Full Stack Junior enfocado en la automatización de procesos empresariales y la integración de APIs y servicios de inteligencia artificial.

En VADEL S.A.S. participo en el desarrollo de funcionalidades frontend y backend, diseño y mantengo flujos de trabajo con n8n e integro servicios para conectar aplicaciones y apoyar procesos empresariales.

Trabajo con React, TypeScript, Node.js, NestJS y Prisma, junto con bases de datos relacionales. También participo en pruebas, dockerización y despliegue con Git, Docker y Jenkins.

Mi experiencia en soporte de TI, Linux, Proxmox y virtualización me ayuda a conectar el desarrollo de software con las necesidades operativas de las personas y los sistemas.

## Lo que desarrollo

Desarrollo aplicaciones web, automatizo procesos con n8n, integro APIs
y servicios de IA, y participo en el despliegue y la operación de aplicaciones.

<picture>
  <source
    media="(max-width: 640px)"
    srcset="assets/especialidades-mobile.svg">
  <img
    src="assets/especialidades.svg"
    alt="Especialidades: desarrollo Full Stack, automatización de procesos, integración de APIs y servicios de IA, y DevOps e infraestructura."
    width="1200">
</picture>

## Proyectos destacados

### WebKitsunova Proyecto
Aplicación full‑stack unificada (único repositorio, único proceso y único despliegue) construida sobre Next.js 16 con App Router y React 19. Autenticación con Supabase Auth + @supabase/ssr (cookies httpOnly, sin token en localStorage), datos en PostgreSQL/Supabase con Prisma, estilos con Tailwind CSS y pruebas con Vitest + Testing Library. Incluye server components, server actions, guards de autorización en Node runtime (USER, PSYCHOLOGIST, ADMIN), MFA, registro público, migraciones con Supabase CLI y despliegue en Vercel; entorno local con Docker Compose + Postgres 16 y hot reload.
- **Stack real**: Next.js 16, React 19, TypeScript, Prisma 5, Supabase (Auth + SSR), Tailwind CSS 3, Vitest 2, Docker, PostgreSQL 16
- **Enlace**: https://github.com/dhait0/webkitsunova-proyecto

### Nexus n8n Workflow Kit

Colección de cuatro workflows importables de n8n (JSON) para demostrar patrones de automatización empresarial: enrutamiento de incidentes por webhook, ingestión de riesgo de proveedores con clasificación por tier, revisión de contenido con puerta de aprobación humana, y sincronización de ciclo de vida de usuarios tipo Microsoft Graph disparada por programador. Incluye payloads de demostración, script local de validación que comprueba estructura, conexiones, IDs de nodos y ausencia de credenciales embebidas, y entorno Docker con n8n 2.29.7 para importar y previsualizar los flujos sin exponerlos. Documentación bilingüe (inglés/español); todos los flujos llevan traducción bilingüe en sus respuestas.

**Aspectos técnicos**
- Cuatro workflows JSON importables: Incident Triage Router, Vendor Risk Intake, AI Review Human Gate, Graph User Lifecycle Sync
- Nodos verificados: Webhook, Code, IF, HTTP Request, Respond to Webhook, Schedule Trigger
- Sin credenciales embebidas en nodos ni workflow (validado por script); placeholders `$env.MOCK_*` y dominios `example.invalid`
- Script local `scripts/validate-workflows.mjs` para validar estructura, conexiones, IDs de nodos y seguridad de credenciales
- Docker Compose con n8nio/n8n:2.29.7 (workflows y samples montados de solo lectura) para importar y previsualizar
- Documentación bilingüe y payloads de demostración en `samples/`

**Stack:** n8n (workflow JSON, formato de importación 2.x), Node.js (scripts de validación), Docker (entorno de previsualización), Prettier, Husky, lint-staged

[Ver código](https://github.com/dhait0/nexus-n8n-workflow-kit)

### Forge CI Deploy Pipeline

Demo bilingüe de Jenkins, Docker y Linux que muestra un pipeline CI/CD para un servicio TypeScript mock: checkout, install, quality gate (lint + build en paralelo), tests, imagen Docker multi-stage, smoke test con Docker Compose y script de rollback simulado. El servicio HTTP de TypeScript expone endpoints de salud (`/health`) y metadatos de release (`/release`); el smoke test los valida con curl y el healthcheck del compose usa `wget`. Incluye script Linux de preflight y archivado de artefactos al finalizar el pipeline.

**Aspectos técnicos**
- Pipeline declarativo de Jenkins con stages: Checkout, Install, Quality Gate (Lint + Build), Test, Docker Image, Smoke Test
- Docker multi-stage (node:22-alpine: dependencies → build → runtime, EXPOSE 4020)
- Docker Compose con healthcheck (`wget -qO- /health`, interval 10s, retries 5)
- Servicio TypeScript HTTP con endpoints `/health` y `/release`
- Scripts: `smoke-test.sh` (curl a health y release), `rollback.sh` (simulado), `linux-preflight.sh`
- Tests con `node --test`, ESLint, Prettier, Husky, lint-staged

**Stack:** Node.js, TypeScript, Jenkins, Docker, Docker Compose, Linux Bash, ESLint, Prettier, Husky

[Ver código](https://github.com/dhait0/forge-ci-deploy-pipeline)

## Tecnologías y herramientas

### Frontend

![React](https://img.shields.io/badge/React-161B22?style=flat-square&logo=react&logoColor=22D3EE)
![TypeScript](https://img.shields.io/badge/TypeScript-161B22?style=flat-square&logo=typescript&logoColor=60A5FA)

### Backend

![Node.js](https://img.shields.io/badge/Node.js-161B22?style=flat-square&logo=nodedotjs&logoColor=22D3EE)
![NestJS](https://img.shields.io/badge/NestJS-161B22?style=flat-square&logo=nestjs&logoColor=60A5FA)
![Prisma ORM](https://img.shields.io/badge/Prisma_ORM-161B22?style=flat-square&logo=prisma&logoColor=A78BFA)

### Bases de datos

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-161B22?style=flat-square&logo=postgresql&logoColor=22D3EE)
![MySQL](https://img.shields.io/badge/MySQL-161B22?style=flat-square&logo=mysql&logoColor=60A5FA)
![SQL Server](https://img.shields.io/badge/SQL_Server-161B22?style=flat-square&logo=microsoftsqlserver&logoColor=A78BFA)

### Automatización e integraciones

![n8n](https://img.shields.io/badge/n8n-161B22?style=flat-square&logo=n8n&logoColor=22D3EE)

**Integración de APIs** · **Servicios de IA**

### DevOps

![Git](https://img.shields.io/badge/Git-161B22?style=flat-square&logo=git&logoColor=22D3EE)
![Docker](https://img.shields.io/badge/Docker-161B22?style=flat-square&logo=docker&logoColor=60A5FA)
![Jenkins](https://img.shields.io/badge/Jenkins-161B22?style=flat-square&logo=jenkins&logoColor=A78BFA)
![Linux](https://img.shields.io/badge/Linux-161B22?style=flat-square&logo=linux&logoColor=E6EDF3)

### Infraestructura y entornos empresariales

![Proxmox](https://img.shields.io/badge/Proxmox-161B22?style=flat-square&logo=proxmox&logoColor=22D3EE)
![Windows](https://img.shields.io/badge/Windows-161B22?style=flat-square&logo=windows11&logoColor=60A5FA)

**Virtualización** · **Redes** · **Administración básica de servidores**

**Microsoft 365** · **Active Directory** · **SharePoint**

### Otras herramientas de mi stack
<details>
<summary>Ver herramientas adicionales</summary>
### Desarrollo web
`JavaScript` · `CSS3` · `Next.js` · `Vite` · `Tailwind CSS` · `Chakra UI` · `React Router` · `React Hook Form` · `React Query` · `NPM` · `WordPress`
### Lenguajes y scripting
`Python` · `PHP` · `C++` · `PowerShell` · `Markdown` · `LaTeX`
### Datos y almacenamiento
`MongoDB` · `Redis` · `SQLite` · `Elasticsearch` · `Pandas` · `Django` · `FastAPI`

### Hardware e infraestructura
`Windows Terminal` · `Cisco` · `Raspberry Pi` · `Arduino`

### Diseño y productividad
`Bitwarden` · `Power BI` · `Notion` · `Prezi` · `Figma` · `Canva` · `Adobe Premiere Pro` · `Adobe Lightroom` · `Adobe Photoshop` · `Adobe Illustrator` · `Adobe Creative Cloud`
</details>

## Actividad de GitHub
![Stats](assets/stats.svg)
[Ver mi perfil de GitHub](https://github.com/dhait0)

## Contacto
[![Website](https://img.shields.io/badge/-ParzKeys-00FFFF?logo=google-chrome&logoColor=white&style=for-the-badge)](https://www.parzkeys.com/)
[![GitHub](https://img.shields.io/badge/-GitHub-181717?logo=github&logoColor=white&style=for-the-badge)](https://github.com/dhait0)
[![Email](https://img.shields.io/badge/-Email-D14836?logo=gmail&logoColor=white&style=for-the-badge)](mailto:sebascamargo39@gmail.com)
[![Instagram](https://img.shields.io/badge/-Instagram-E4405F?logo=instagram&logoColor=white&style=for-the-badge)](https://instagram.com/no4uth_keys)
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?logo=linkedin&logoColor=white&style=for-the-badge)](https://www.linkedin.com/in/sebastian-camargo-a823b6322)

---
*Hecho con ❤️ y ☕. Explora mi trabajo y contacta para colaboraciones.*
