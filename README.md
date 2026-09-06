<div align="center">

<!-- Banner animado -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0F172A,50:1E3A8A,100:2563EB&height=220&section=header&text=Daniel%20Moreno%20López&fontSize=42&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Backend%20y%20sistemas%20distribuidos%20·%20Full-Stack&descAlignY=58&descSize=18" />

<!-- Typing SVG -->
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=800&color=60A5FA&center=true&vCenter=true&width=650&lines=Software+Engineer;Java+%2B+Spring+Boot+%2B+AWS;Next.js+%2B+TypeScript;Arquitecturas+event-driven+y+distribuidas" alt="Typing SVG" />

<br/>

<a href="https://my-portafolio-fawn.vercel.app"><img src="https://img.shields.io/badge/🌐_Portfolio-2563EB?style=for-the-badge&logoColor=white"></a>
<a href="https://linkedin.com/in/daniel-de-jes%C3%BAs-moreno-l%C3%B3pez-889a15303"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"></a>
<a href="mailto:danielmoreno123g@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"></a>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=DaniDJ-Hub&label=Visitas+al+perfil&color=2563EB&style=flat-square" alt="visitor badge"/>

</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:2563EB,100:0F172A&height=3&width=100%25" />

## 🧭 Sobre mí

<table>
<tr>
<td width="60%" valign="top">

Construyo sistemas backend orientados a eventos en **Java** y **Spring Boot**, y los productos web que los consumen en **Next.js** y **TypeScript**. Mi trabajo más reciente son plataformas distribuidas con Kafka, arquitectura hexagonal e infraestructura como código.

- 🎓 Ingeniería en Sistemas Computacionales — TecNM, Campus Comitán (2022–2027)
- ⚙️ Foco en sistemas distribuidos, mensajería asíncrona y calidad de entrega
- 📍 Comitán de Domínguez, Chiapas, México
- 🗣️ Español (nativo) · Inglés (B2)

</td>
<td width="40%" valign="top" align="center">

```yaml
daniel.dev:
  role: "Software Engineer"
  focus: [Backend, Distributed Systems, Full-Stack]
  stack: [Java, Spring Boot, Next.js, TypeScript]
  status: "Aprendiendo Spring Framework 6 a fondo"
```

</td>
</tr>
</table>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:2563EB,100:0F172A&height=3&width=100%25" />

## 🛰️ Sistemas distribuidos y backend

Cuatro plataformas construidas para practicar patrones reales de sistemas distribuidos.

<table width="100%">
<tr>
<td width="50%" valign="top">

### 🏦 NEXUS Financial Platform
*Plataforma fintech de banca digital*

Cubre el ciclo completo: identidad del cliente, KYC, apertura de cuentas, transferencias, contabilidad de partida doble, detección de fraude, scoring de riesgo y auditoría inmutable.

**17 servicios** — 16 Spring Boot + 1 Quarkus nativo — coordinados por Kafka, con persistencia poliglota e IA integrada vía OpenAI, Ollama y pgvector.

<p>
<img src="https://img.shields.io/badge/Java_25-007396?style=flat-square&logo=openjdk&logoColor=white"/>
<img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white"/>
<img src="https://img.shields.io/badge/Quarkus-4695EB?style=flat-square&logo=quarkus&logoColor=white"/>
<img src="https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white"/>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white"/>
<img src="https://img.shields.io/badge/Elasticsearch-005571?style=flat-square&logo=elasticsearch&logoColor=white"/>
<img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/>
</p>

`Estado: ✅ Completado`

<a href="https://github.com/DaniDJ-Hub/Nexus"><img src="https://img.shields.io/badge/Código-181717?style=flat-square&logo=github&logoColor=white"/></a>

</td>
<td width="50%" valign="top">

### 🛒 TradeFlow
*Marketplace distribuido*

Compradores y vendedores con KYC, publicación de productos, búsqueda, órdenes y cobro coordinados de forma asíncrona.

Una orden toca inventario, fraude y pagos a la vez. **SAGA orquestada** con compensaciones explícitas resuelve el fallo parcial sin transacciones distribuidas, sobre CQRS, Event Sourcing y patrón Outbox.

<p>
<img src="https://img.shields.io/badge/Java_21-007396?style=flat-square&logo=openjdk&logoColor=white"/>
<img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white"/>
<img src="https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white"/>
<img src="https://img.shields.io/badge/SAGA-2563EB?style=flat-square"/>
<img src="https://img.shields.io/badge/CQRS-2563EB?style=flat-square"/>
<img src="https://img.shields.io/badge/Event_Sourcing-2563EB?style=flat-square"/>
<img src="https://img.shields.io/badge/Elasticsearch-005571?style=flat-square&logo=elasticsearch&logoColor=white"/>
</p>

`Estado: ✅ Completado`

<a href="https://github.com/DaniDJ-Hub/Tradeflow"><img src="https://img.shields.io/badge/Código-181717?style=flat-square&logo=github&logoColor=white"/></a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📡 Twitter Stream Analytics
*Analítica de streams en tiempo real*

Un stream continuo alimenta a la vez búsqueda full-text y analítica agregada, sin que un consumidor lento frene al otro ni al productor.

Publicación en Kafka con Avro y Schema Registry, procesamiento con **Kafka Streams**, y dos consumidores desacoplados: Elasticsearch por un lado, PostgreSQL y API REST con Keycloak por el otro.

<p>
<img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white"/>
<img src="https://img.shields.io/badge/Kafka_Streams-231F20?style=flat-square&logo=apachekafka&logoColor=white"/>
<img src="https://img.shields.io/badge/Avro-1A73E8?style=flat-square"/>
<img src="https://img.shields.io/badge/Elasticsearch-005571?style=flat-square&logo=elasticsearch&logoColor=white"/>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/Keycloak-4D4D4D?style=flat-square&logo=keycloak&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
</p>

`Estado: ✅ Completado`

<a href="https://github.com/DaniDJ-Hub/Twitter-Microservicios"><img src="https://img.shields.io/badge/Código-181717?style=flat-square&logo=github&logoColor=white"/></a>

</td>
<td width="50%" valign="top">

### 📦 PaperFlow
*Inventario y punto de venta para papelerías*

Esquema relacional PostgreSQL de 14 entidades. Lecturas paginadas desde Server Components y mutaciones desde Client Components contra Supabase, con **Row Level Security** como capa de autorización en lugar de una API REST intermedia.

<p>
<img src="https://img.shields.io/badge/Next.js_16-000000?style=flat-square&logo=next.js&logoColor=white"/>
<img src="https://img.shields.io/badge/React_19-61DAFB?style=flat-square&logo=react&logoColor=black"/>
<img src="https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white"/>
<img src="https://img.shields.io/badge/Zod-3E67B1?style=flat-square&logo=zod&logoColor=white"/>
<img src="https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white"/>
</p>

`Estado: ✅ Completado`

<a href="https://github.com/DaniDJ-Hub/Inventory-System_MJ"><img src="https://img.shields.io/badge/Código-181717?style=flat-square&logo=github&logoColor=white"/></a>

</td>
</tr>
</table>

<details>
<summary><b>🗺️ Ver el flujo de una orden en TradeFlow (SAGA orquestada)</b></summary>
<br/>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/DaniDJ-Hub/DaniDJ-Hub/main/assets/architecture-dark.svg">
  <img alt="Diagrama del flujo de una orden en TradeFlow: el API Gateway llega al Order Service, que orquesta una SAGA sobre Kafka coordinando los servicios de inventario, fraude y pago, con PostgreSQL por servicio, patrón Outbox y Elasticsearch para búsqueda." src="https://raw.githubusercontent.com/DaniDJ-Hub/DaniDJ-Hub/main/assets/architecture-light.svg">
</picture>

</details>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:2563EB,100:0F172A&height=3&width=100%25" />

## 🚀 Producto y full-stack

<table width="100%">
<tr>
<td width="50%" valign="top">

### 🦁 Zoológico La Trinitaria
*Boletaje con códigos QR*

Venta, generación y validación de boletos con lector de cámara, persistencia en SQLite y autenticación por cookies HMAC. El proyecto donde más trabajé calidad y entrega: pruebas con Vitest, carga con JMeter, colección Postman y **CI/CD** que ejecuta typecheck, lint, pruebas, build y publicación de imagen Docker.

<p>
<img src="https://img.shields.io/badge/Next.js_15-000000?style=flat-square&logo=next.js&logoColor=white"/>
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/>
<img src="https://img.shields.io/badge/Firestore-FFCA28?style=flat-square&logo=firebase&logoColor=black"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/>
</p>

`Estado: ✅ Completado`

<a href="https://github.com/DaniDJ-Hub/Zool-gico_Project"><img src="https://img.shields.io/badge/Código-181717?style=flat-square&logo=github&logoColor=white"/></a>

</td>
<td width="50%" valign="top">

### ⚽ Fut 7 Soccer
*Gestión de liga deportiva*

Equipos, jugadores, jornadas, goles, penales y tabla de posiciones. Migración de una app multipágina en vanilla JS + Express a una sola aplicación Next.js: las API routes hablan directamente con Postgres, sin backend separado.

<p>
<img src="https://img.shields.io/badge/Next.js_15-000000?style=flat-square&logo=next.js&logoColor=white"/>
<img src="https://img.shields.io/badge/React_19-61DAFB?style=flat-square&logo=react&logoColor=black"/>
<img src="https://img.shields.io/badge/Tailwind_v4-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white"/>
<img src="https://img.shields.io/badge/Neon_Postgres-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
</p>

`Estado: ✅ Completado`

<a href="https://github.com/DaniDJ-Hub/Soccer_Match_System"><img src="https://img.shields.io/badge/Código-181717?style=flat-square&logo=github&logoColor=white"/></a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🏋️ FORGE ATHLETICS
*Landing page premium con panel de administración*

Modelo de datos relacional en Django ORM con 9 entidades, panel admin personalizado con django-unfold, internacionalización completa español/inglés sin tocar código y animaciones GSAP/AOS/Swiper.

<p>
<img src="https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white"/>
<img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white"/>
<img src="https://img.shields.io/badge/Alpine.js-8BC0D0?style=flat-square&logo=alpinedotjs&logoColor=black"/>
<img src="https://img.shields.io/badge/GSAP-88CE02?style=flat-square&logo=greensock&logoColor=black"/>
</p>

`Estado: ✅ Completado`

<!-- Sin repositorio público todavía -->

</td>
<td width="50%" valign="top">

### 🎮 Spring Boot Quest
*Juego educativo para aprender Spring Boot*

Retos de código, debugging con stack traces reales, decisiones de arquitectura y batallas finales por módulo. Quince mundos derivados del temario real de un curso, sin backend.

<p>
<img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black"/>
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/>
<img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white"/>
<img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white"/>
</p>

`Estado: ✅ Completado`

<a href="https://github.com/DaniDJ-Hub/Spring-Boot-Quest"><img src="https://img.shields.io/badge/Código-181717?style=flat-square&logo=github&logoColor=white"/></a>

</td>
</tr>
</table>

<details>
<summary><b>📂 Ver el resto de proyectos</b></summary>
<br/>

| Proyecto | Qué es | Stack | Estado |
|---|---|---|---|
| [🍕 PizzaManía POS](https://github.com/DaniDJ-Hub/Pizzeria-Sistem-Pos) | Punto de venta multi-sucursal con roles: admin, cajero, cocina, mesero | `Next.js 15` `React 19` `Firebase` | ✅ |
| [🌮 Tortillería POS](https://github.com/DaniDJ-Hub/Tortilleria_System_POS) | POS de una sola pantalla; migración que eliminó la dependencia de Firebase | `Next.js 15` `React 19` `Tailwind v4` | ✅ |
| [🐾 VetCare Manager](https://github.com/DaniDJ-Hub/VetCare_Manager_Public) | Gestión de pacientes veterinarios con aislamiento de datos por cuenta | `MERN` `JWT` `bcrypt` `MVC` | ✅ |
| [✈️ ViajaYa](https://github.com/DaniDJ-Hub/Agencia-Viajes-Public) | Agencia de viajes con renderizado server-side y catálogo dinámico | `Express` `Pug` `Sequelize` `MySQL` | ✅ |
| [💅 NailStudio Glam](https://github.com/DaniDJ-Hub/Nail_Services_Page) | Landing comercial orientada a configuración, con integración WhatsApp | `Next.js` `TypeScript` `Tailwind` | ✅ |
| [📝 App de Notas](https://github.com/DaniDJ-Hub/App_Notas_Public) | CRUD full-stack con API en Spring Boot y frontend en React | `Spring Boot` `React` `Vite` | ✅ |

</details>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:2563EB,100:0F172A&height=3&width=100%25" />

## 🧰 Stack tecnológico

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/DaniDJ-Hub/DaniDJ-Hub/main/assets/stack-dark.svg">
  <img width="100%" alt="Stack por categoría. Backend: Java, Spring Boot 3, Quarkus, Node.js, Express, Django. Frontend: TypeScript, React 19, Next.js 15/16, Tailwind CSS, shadcn/ui. Datos: PostgreSQL, MySQL, MongoDB, Elasticsearch, Redis, Supabase. Eventos: Kafka, Kafka Streams, Avro, Schema Registry. Infraestructura: Docker, Terraform, AWS, GitHub Actions, Vercel. Calidad y seguridad: Vitest, JMeter, Postman, Keycloak, JWT, Zod." src="https://raw.githubusercontent.com/DaniDJ-Hub/DaniDJ-Hub/main/assets/stack-light.svg">
</picture>

</div>

<details>
<summary><b>🏗️ Patrones y arquitectura aplicados</b></summary>
<br/>

Microservicios · Arquitectura hexagonal (puertos y adaptadores) · Event-driven ·
SAGA orquestada con compensaciones · CQRS · Event Sourcing · Patrón Outbox ·
MVC · REST · Server Components / Route Handlers

</details>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:2563EB,100:0F172A&height=3&width=100%25" />

## 📊 Roadmap de aprendizaje

```
Frontend Sólido       ████████████████████ 100%
Sistemas distribuidos ████████████████░░░░  80%
Backend (Java/Spring) ███████████████░░░░░  75%
Event-driven (Kafka)  ██████████████░░░░░░  70%
DevOps / Cloud        ██████████░░░░░░░░░░  50%
```

## 🎯 Actualmente

- 🔨 **Construyendo** — <!-- PENDIENTE: proyecto activo, objetivo en una línea y estado. -->
- 🌱 **Aprendiendo** — Spring Framework 6 y Spring Boot 3 a fondo; el temario está reconstruido como juego en [Spring Boot Quest](https://github.com/DaniDJ-Hub/Spring-Boot-Quest)
- 🧭 **Siguiente foco** — despliegue en la nube y diseño de sistemas
- 💬 **Pregúntame sobre** — Arquitectura de microservicios o Next.js App Router

<details>
<summary><b>🎓 Formación y certificaciones</b></summary>
<br/>

Ingeniería en Sistemas Computacionales — TecNM, Campus Comitán (2022–2027)
Participación en Torneo Local de Programación

| Curso | Plataforma | Año |
|---|---|---|
| HTML y CSS | Udemy | 2024 |
| JavaScript | Udemy | 2024 |
| Tailwind CSS | Udemy | 2025 |
| React.js | Udemy | 2025 |

</details>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:2563EB,100:0F172A&height=3&width=100%25" />

## 📈 GitHub Analytics

<div align="center">

<img height="160" alt="Estadísticas de contribución de DaniDJ-Hub en GitHub" src="https://github-readme-stats.vercel.app/api?username=DaniDJ-Hub&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=60A5FA&icon_color=60A5FA" />
<img height="160" alt="Racha de contribuciones de DaniDJ-Hub" src="https://github-readme-streak-stats.herokuapp.com/?user=DaniDJ-Hub&theme=tokyonight&hide_border=true&background=0D1117&ring=60A5FA&fire=2563EB" />

<img width="49%" alt="Lenguajes más usados por DaniDJ-Hub" src="https://github-readme-stats.vercel.app/api/top-langs/?username=DaniDJ-Hub&layout=compact&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=60A5FA&langs_count=8" />
<img width="49%" alt="Gráfico de actividad de DaniDJ-Hub" src="https://github-readme-activity-graph.vercel.app/graph?username=DaniDJ-Hub&theme=tokyo-night&hide_border=true&bg_color=0D1117&color=60A5FA&line=2563EB&point=ffffff" />

</div>

<div align="center">
<img src="https://github-profile-trophy.vercel.app/?username=DaniDJ-Hub&theme=algolia&no-frame=true&row=1&column=7&margin-w=8" />
</div>

<!-- Contribution Snake — requiere GitHub Action, ver instrucciones al final -->
<div align="center">
  <img src="https://raw.githubusercontent.com/DaniDJ-Hub/DaniDJ-Hub/output/github-contribution-grid-snake.svg" alt="snake animation" />
</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:2563EB,100:0F172A&height=3&width=100%25" />

## 📫 Contacto

<div align="center">

<a href="https://my-portafolio-fawn.vercel.app"><img src="https://img.shields.io/badge/Portfolio-2563EB?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio"></a>
<a href="https://linkedin.com/in/daniel-de-jes%C3%BAs-moreno-l%C3%B3pez-889a15303"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
<a href="mailto:danielmoreno123g@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>

<br/><br/>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0F172A,50:1E3A8A,100:2563EB&height=120&section=footer" />

</div>
