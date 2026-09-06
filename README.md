<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/DaniDJ-Hub/DaniDJ-Hub/main/assets/hero-dark.svg">
  <img alt="Daniel Moreno López — Software Engineer. Backend y sistemas distribuidos, full-stack. Java, Spring Boot, Kafka, AWS, Next.js, TypeScript." src="https://raw.githubusercontent.com/DaniDJ-Hub/DaniDJ-Hub/main/assets/hero-light.svg">
</picture>

Construyo sistemas backend orientados a eventos en Java y Spring Boot, y los productos
web que los consumen en Next.js y TypeScript. Mi trabajo más reciente son plataformas
distribuidas con Kafka, arquitectura hexagonal e infraestructura como código.

Ingeniería en Sistemas Computacionales — TecNM, Campus Comitán · Chiapas, México · Español (nativo) / Inglés (B2)

[Portfolio](https://my-portafolio-fawn.vercel.app) · [LinkedIn](https://linkedin.com/in/daniel-de-jes%C3%BAs-moreno-l%C3%B3pez-889a15303) · [Email](mailto:danielmoreno123g@gmail.com)

---

## Sistemas distribuidos y backend

Cuatro plataformas construidas para practicar patrones reales de sistemas distribuidos,
no ejercicios de curso.

### [NEXUS Financial Platform](https://github.com/DaniDJ-Hub/Nexus)

Plataforma fintech de banca digital que cubre el ciclo completo: identidad del cliente,
verificación KYC, apertura de cuentas, transferencias, contabilidad de partida doble,
detección de fraude, scoring de riesgo y pista de auditoría inmutable.

**El problema.** Un núcleo bancario no puede acoplar el registro de clientes con el
motor de pagos ni con la detección de fraude: cada dominio cambia a su propio ritmo y
falla de forma independiente.

**Las decisiones.** 17 servicios (16 Spring Boot + 1 Quarkus en modo nativo) coordinados
por Kafka, con persistencia poliglota — PostgreSQL para lo transaccional, MongoDB para
documentos, Elasticsearch para búsqueda y Redis para caché — y capacidades de IA
integradas vía OpenAI, Ollama y pgvector.

`Java 25` `Spring Boot` `Quarkus` `Kafka` `PostgreSQL` `MongoDB` `Elasticsearch` `Redis` `pgvector`

<!-- PENDIENTE: confirmar estado (terminado / en curso) antes de publicar. -->

---

### [TradeFlow](https://github.com/DaniDJ-Hub/Tradeflow)

Marketplace distribuido tipo Amazon/MercadoLibre: alta de compradores y vendedores con
KYC, publicación de productos, búsqueda, órdenes y cobro coordinados de forma asíncrona.

**El problema.** Una orden toca inventario, fraude y pagos a la vez. Si cualquiera de los
tres falla a mitad del proceso, el sistema tiene que deshacer lo ya hecho sin transacciones
distribuidas.

**Las decisiones.** SAGA orquestada desde el Order Service con compensaciones explícitas,
más CQRS, Event Sourcing y patrón Outbox sobre Kafka. Búsqueda en Elasticsearch y
observabilidad completa del flujo.

`Java 21` `Spring Boot` `Kafka` `SAGA` `CQRS` `Event Sourcing` `Outbox` `Elasticsearch`

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/DaniDJ-Hub/DaniDJ-Hub/main/assets/architecture-dark.svg">
  <img alt="Diagrama del flujo de una orden en TradeFlow: el API Gateway llega al Order Service, que orquesta una SAGA sobre Kafka coordinando los servicios de inventario, fraude y pago, con PostgreSQL por servicio, patrón Outbox y Elasticsearch para búsqueda." src="https://raw.githubusercontent.com/DaniDJ-Hub/DaniDJ-Hub/main/assets/architecture-light.svg">
</picture>

<!-- PENDIENTE: confirmar estado antes de publicar. -->

---

### [NeoBank](https://github.com/DaniDJ-Hub/NeoBank)

Plataforma bancaria con arquitectura hexagonal y un núcleo transaccional serverless
desplegado en AWS, con toda la infraestructura versionada.

**El problema.** Separar la lógica de negocio de la infraestructura lo suficiente como
para que el mismo dominio corra tras una API REST en contenedor o tras funciones Lambda.

**Las decisiones.** Núcleo en Spring Boot 3 / Java 21 con puertos y adaptadores,
8 funciones Lambda (7 en Java 17, 1 en Python 3.11), frontend Next.js 15 / React 19, e
infraestructura completa en Terraform: VPC, RDS, EC2, S3, DynamoDB, SNS, SQS, Cognito y
API Gateway. Incluye pruebas de carga con JMeter.

`Java 21` `Spring Boot 3` `Arquitectura hexagonal` `AWS Lambda` `Terraform` `Next.js 15` `JMeter`

<!-- PENDIENTE: confirmar estado antes de publicar. -->

---

### [Twitter Stream Analytics](https://github.com/DaniDJ-Hub/Twitter-Microservicios)

Analítica de streams en tiempo real: ingesta desde la API de streaming de Twitter,
procesamiento y reparto hacia dos consumidores independientes.

**El problema.** Un stream continuo tiene que alimentar a la vez búsqueda full-text y
analítica agregada, sin que un consumidor lento frene al otro ni al productor.

**Las decisiones.** Publicación en Kafka con Avro y Schema Registry, procesamiento con
Kafka Streams, y dos consumidores desacoplados: uno indexa en Elasticsearch, otro persiste
agregados en PostgreSQL y los expone en una API REST protegida con JWT vía Keycloak. Todo
el stack levanta con Docker Compose.

`Java` `Spring Boot` `Kafka Streams` `Avro` `Schema Registry` `Elasticsearch` `PostgreSQL` `Keycloak` `Docker Compose`

<!-- PENDIENTE: confirmar estado antes de publicar. -->

---

## Producto y full-stack

Aplicaciones completas, varias de ellas en uso real por negocios locales.

### [PaperFlow](https://github.com/DaniDJ-Hub/Inventory-System_MJ)

Sistema de inventario, punto de venta y gestión para papelerías. Lecturas paginadas desde
Server Components y mutaciones desde Client Components contra Supabase, con Row Level
Security como capa de autorización en vez de una API REST intermedia.

`Next.js 16` `React 19` `Tailwind v4` `Supabase` `PostgreSQL + RLS` `Zod` `Vitest`

<!-- PENDIENTE: el README anterior afirmaba "esquema relacional de 14 entidades".
     No pude verificarlo en el repo. Confírmalo y lo añado, o lo dejamos fuera. -->

---

### [Zoológico La Trinitaria](https://github.com/DaniDJ-Hub/Zool-gico_Project)

Sistema de boletaje con códigos QR: venta, generación y validación de boletos con lector
por cámara. Es el proyecto donde más trabajé la parte de calidad y entrega: pruebas
unitarias con Vitest, pruebas de carga con JMeter, colección Postman y un pipeline de
GitHub Actions que ejecuta typecheck, lint, pruebas, build y publicación de imagen Docker.

`Next.js 15` `TypeScript` `Docker` `GitHub Actions` `Vitest` `JMeter`

<!-- PENDIENTE FASE 0: el repo tiene todo dentro de zoo-nextjs/. Los workflows no se
     ejecutan porque GitHub solo lee .github/workflows/ desde la raíz. Subir a raíz. -->
<!-- PENDIENTE: confirmar la fuente de datos real (el README anterior decía SQLite, el
     repo contiene configuración de Firestore). No la menciono hasta confirmarlo. -->

---

### [Fut 7 El Jaguar](https://github.com/DaniDJ-Hub/Soccer_Match_System)

Gestión de liga deportiva: equipos, jugadores, jornadas, goles, penales y tabla de
posiciones. Migración completa de una app multipágina en vanilla JS + Express a una sola
aplicación Next.js, eliminando el backend separado: las API routes hablan directamente
con Postgres. Modo claro/oscuro con toda la paleta en variables CSS.

`Next.js 15` `React 19` `Tailwind v4` `PostgreSQL (Neon)`

---

### Otros proyectos

| Proyecto | Qué es | Stack |
|---|---|---|
| [PizzaManía POS](https://github.com/DaniDJ-Hub/Pizzeria-Sistem-Pos) | Punto de venta multi-sucursal con roles (admin, cajero, cocina, mesero) | `Next.js 15` `React 19` `Firebase` |
| [Tortillería POS](https://github.com/DaniDJ-Hub/Tortilleria_System_POS) | POS de una sola pantalla; migración que eliminó la dependencia de Firebase | `Next.js 15` `React 19` `Tailwind v4` |
| [VetCare Manager](https://github.com/DaniDJ-Hub/VetCare_Manager_Public) | Gestión de pacientes veterinarios con aislamiento de datos por veterinario | `MERN` `JWT` `bcrypt` `MVC` |
| [ViajaYa](https://github.com/DaniDJ-Hub/Agencia-Viajes-Public) | Agencia de viajes con renderizado server-side y catálogo dinámico | `Node.js` `Express` `Pug` `Sequelize` `MySQL` |
| [NailStudio Glam](https://github.com/DaniDJ-Hub/Nail_Services_Page) | Landing comercial orientada a configuración, con integración WhatsApp | `Next.js` `TypeScript` `Tailwind` |
| [App de Notas](https://github.com/DaniDJ-Hub/App_Notas_Public) | CRUD full-stack con API en Spring Boot y frontend en React | `Spring Boot` `React` `Vite` |
| [Spring Boot Quest](https://github.com/DaniDJ-Hub/Spring-Boot-Quest) | Juego educativo para aprender Spring Boot: retos, debugging con stack traces reales y decisiones de arquitectura | `React` `TypeScript` `Vite` `Tailwind` |

<!-- PENDIENTE FASE 0: FORGE ATHLETICS no tiene repositorio público. Si lo publicas,
     se añade aquí; si no, se queda fuera. -->

---

## Stack

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/DaniDJ-Hub/DaniDJ-Hub/main/assets/stack-dark.svg">
  <img alt="Stack por categoría. Backend: Java, Spring Boot 3, Quarkus, Node.js, Express, Django. Frontend: TypeScript, React 19, Next.js 15/16, Tailwind CSS, shadcn/ui. Datos: PostgreSQL, MySQL, MongoDB, Elasticsearch, Redis, Supabase. Eventos: Kafka, Kafka Streams, Avro, Schema Registry. Infraestructura: Docker, Terraform, AWS, GitHub Actions, Vercel. Calidad y seguridad: Vitest, JMeter, Postman, Keycloak, JWT, Zod." src="https://raw.githubusercontent.com/DaniDJ-Hub/DaniDJ-Hub/main/assets/stack-light.svg">
</picture>

<details>
<summary>Patrones y arquitectura aplicados</summary>

Microservicios · Arquitectura hexagonal (puertos y adaptadores) · Event-driven ·
SAGA orquestada con compensaciones · CQRS · Event Sourcing · Patrón Outbox ·
MVC · REST · Server Components / Route Handlers

</details>


---

## Actualmente

**Construyendo** — <!-- PENDIENTE: nombre del proyecto activo, objetivo en una línea y estado. -->

**Aprendiendo** — Spring Framework 6 y Spring Boot 3 a fondo; el temario está reconstruido
como juego en [Spring Boot Quest](https://github.com/DaniDJ-Hub/Spring-Boot-Quest).
Siguiente foco: despliegue en la nube y diseño de sistemas.

<details>
<summary>Formación y certificaciones</summary>

Ingeniería en Sistemas Computacionales — TecNM, Campus Comitán (2022–2027)
Participación en Torneo Regional de Programación

| Curso | Plataforma | Año |
|---|---|---|
| HTML y CSS | Udemy | 2024 |
| JavaScript | Udemy | 2024 |
| Tailwind CSS | Udemy | 2025 |
| React.js | Udemy | 2025 |

</details>

---

## Contacto

**Portfolio** — [my-portafolio-fawn.vercel.app](https://my-portafolio-fawn.vercel.app)
**LinkedIn** — [Daniel de Jesús Moreno López](https://linkedin.com/in/daniel-de-jes%C3%BAs-moreno-l%C3%B3pez-889a15303)
**Email** — [danielmoreno123g@gmail.com](mailto:danielmoreno123g@gmail.com)

<img src="https://github-readme-stats.vercel.app/api?username=DaniDJ-Hub&show_icons=true&hide_border=true&theme=transparent&hide_title=true" alt="Estadísticas de contribución de DaniDJ-Hub en GitHub" height="150" />