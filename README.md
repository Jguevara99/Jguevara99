<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&pause=1200&color=3670FF&center=true&vCenter=true&width=750&lines=Jairo+Guevara+%E2%80%94+Full+Stack+Developer;.NET+%7C+Angular+%7C+Enterprise+Systems;Building+systems+that+actually+scale.)](https://git.io/typing-svg)

<img src="https://komarev.com/ghpvc/?username=Jguevara99&label=Profile+Views&color=3670ff&style=for-the-badge" alt="Profile views" />

</div>

---

## Who I Am

Full Stack Developer specialized in **enterprise and institutional software**.

At **INETER** (Nicaragua), I build internal systems with **.NET + Razor**, focused on:
- operational workflows,
- institutional data management,
- reporting pipelines,
- and production reliability.

Outside INETER, I collaborate on full-stack platforms using **.NET APIs + Angular**, covering architecture decisions, authentication design, module boundaries, and production deployment.

> Current focus: multi-module **Baseball Stadium Ticketing System** built with **.NET Core 10 + Angular 21**, deployed on a private network VM with Docker.

---

## What I Build

| System | Context | Stack |
|---|---|---|
| 🏛️ **Institutional Management Apps** | Internal tools at INETER — workflows, data management, and reporting for a technical-scientific institution | .NET · Razor · SQL Server |
| ⚾ **Baseball Stadium Ticketing System** | End-to-end stadium POS: events, seat maps, ticket validation, cashier sessions, and reporting | .NET Core 10 · Angular 21 · PrimeNG · SQL Server · Docker |
| 🔐 **Auth & Access Layer** | JWT auth with roles/claims, refresh token flow, route guards, and policy-based authorization | .NET Identity · JWT · Angular Guards |
| 📋 **Collaborative Enterprise Modules** | Team-built modules: approvals, inventory control, and asset tracking | .NET · Angular · SQL Server |

---

## Stadium Ticketing System — Architecture Snapshot

> *Current project. In development. Private network deployment (on-premise).*  
> *Designed to operate without internet dependency inside stadium infrastructure.*

### 7 Modules in Scope

- 🗓️ **Events** — event catalog, team management, base pricing per event
- 🗺️ **Locations** — stadium map, sections/rows/seats, per-section pricing addons
- 🎫 **Ticket Sales** — cashier open/close sessions, seat selection, IVA, barcode ticket generation, courtesy tickets
- 📄 **Documents** — logo/image storage, auto-compression, local VM storage
- 📊 **Reports** — sales by section/event type/cashier, PDF + Excel exports, near real-time dashboards
- 🔒 **Security** — user/role management, audit trails, session policies
- 📡 **Entry Validation** — scanner integration, real-time validation, offline sync strategies

### Infrastructure

```text
Private Stadium Network
└── VM (Production)
    ├── .NET Core 10 API
    ├── Angular 21 Frontend
    ├── SQL Server (Docker)
    ├── Reverse Proxy
    └── Local Document Storage

└── Docker Containers (Testing/Staging)
    ├── Test API
    └── Test Database
```

### Pricing Logic

```text
Final Price = Event Base Price + Section Price Addon + Discounts - IVA
```

---

## Engineering Approach

### Backend (.NET)

Layered architecture with clear separation between business rules, application orchestration, infrastructure concerns, and API surface.

```text
Solution/
├── Domain/          # Entities, value objects
├── Application/     # Use cases, DTOs, validators, interfaces
├── Infrastructure/  # EF Core, repositories, file storage, external services
└── API/             # Controllers, middleware, DI config
```

- **Repository pattern** — business rules do not access DbContext directly.
- **DTO boundaries** — domain entities never leak to transport responses.
- **JWT + ASP.NET Core Identity** — role/claims authorization with refresh token lifecycle.
- **Global exception middleware** — standardized API error contracts.
- **Swagger/OpenAPI** — versioned, consumer-ready endpoint documentation.
- **Application-layer testing** — unit tests with **xUnit + Moq**.

### Frontend (Angular)

Feature-driven module organization with lazy loading and clear split of responsibilities.

```text
src/
├── core/            # Auth, guards, interceptors, global services
├── shared/          # Reusable components, pipes, directives
└── features/
    ├── events/
    ├── ticketing/
    └── reports/
```

- **HTTP Interceptors** for JWT attachment and global error normalization.
- **Route Guards** for role-based navigation control.
- **Reactive Forms** for complex transactional workflows.
- **Service-centric state** so UI components remain lean and focused.

---

## Tech Stack

### ⚙️ Backend
![.NET](https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white)
![Razor](https://img.shields.io/badge/Razor-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)
![Entity Framework](https://img.shields.io/badge/Entity%20Framework-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black)

### 🌐 Frontend
![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![RxJS](https://img.shields.io/badge/RxJS-B7178C?style=for-the-badge&logo=reactivex&logoColor=white)

### 🎨 UI / Design
![PrimeNG](https://img.shields.io/badge/PrimeNG-DD0031?style=for-the-badge&logo=primeng&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind%20CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)

### 🧪 Testing
![xUnit](https://img.shields.io/badge/xUnit-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![Moq](https://img.shields.io/badge/Moq-239120?style=for-the-badge&logo=c-sharp&logoColor=white)

### 🔁 Also in the toolbox
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)

### 🧰 Tools
![Visual Studio](https://img.shields.io/badge/Visual%20Studio-5C2D91?style=for-the-badge&logo=visual-studio&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-0078D4?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![DevExpress](https://img.shields.io/badge/DevExpress-FF7200?style=for-the-badge&logo=devexpress&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)

---

## 🔨 Currently Building

> *Active project — in development as of 2026*

**⚾ Baseball Stadium Ticketing System** — full POS running on a private network VM. Current implementation focus:
- cashier session lifecycle,
- barcode generation pipeline,
- entry validation flow with scanner integration.

`#dotnet` `#angular21` `#primeng` `#sqlserver` `#docker` `#jwt`

---

## 🌐 Portfolio

<div align="center">

[![Portfolio](https://img.shields.io/badge/Portfolio-portafolio--kappa--six--51.vercel.app-3670ff?style=for-the-badge&logo=vercel&logoColor=white)](https://portafolio-kappa-six-51.vercel.app/)

</div>

---

## 📊 GitHub Stats

<div align="center">
  <img height="195px" src="https://github-stats-alpha.vercel.app/api?username=Jguevara99&cc=000&tc=ff6ec7&ic=fff&bc=000" />
  <img height="195px" src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Jguevara99&theme=radical" />
</div>

<div align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Jguevara99&theme=radical" />
</div>

---

## 🏆 Trophies

<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=Jguevara99&theme=radical&no-frame=true&no-bg=true&margin-w=6&column=7" />
</div>

---

## 📈 Contribution Graph

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Jguevara99&theme=react-dark&hide_border=true&area=true&color=ff6ec7&line=3670ff&point=ffffff" />
</div>

---

## Let's Talk

If you're building in the **.NET + Angular** space — enterprise apps, system design, architecture decisions — I'm open to collaboration.

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jairo-guevara)
[![Instagram](https://img.shields.io/badge/Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/jairguev27/)
[![X](https://img.shields.io/badge/X-%23000000?style=for-the-badge&logo=x&logoColor=white)](https://twitter.com/guevara_a1/)
[![Facebook](https://img.shields.io/badge/Facebook-%231877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/jairoantonio.guevaraampie)

</div>

---

<div align="center">
  <sub><i>"Talk is cheap. Show me the code." — Linus Torvalds</i></sub>
</div>
