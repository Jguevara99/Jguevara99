<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&pause=1200&color=3670FF&center=true&vCenter=true&width=750&lines=Jairo+Guevara+%E2%80%94+Full+Stack+Developer;.NET+%7C+Angular+%7C+Enterprise+Systems;Building+systems+that+actually+scale.)](https://git.io/typing-svg)

<img src="https://komarev.com/ghpvc/?username=Jguevara99&label=Profile+Views&color=3670ff&style=for-the-badge" alt="Profile views" />

</div>

---

## Who I Am

Full Stack Developer with experience across enterprise and institutional systems. I work at **INETER** — a technical-scientific institution in Nicaragua — where I develop internal applications using **.NET and Razor**, handling real operational workflows and data management at institutional scale.

Outside of INETER, I collaborate on larger full-stack projects with **.NET APIs and Angular**, covering everything from architecture decisions to production deployment. My current focus project is a multi-module **baseball stadium ticketing system** being built on **.NET Core 10 + Angular 21**, deployed on a private network VM with Docker.

I care about how systems are structured before a line of code is written — layer separation, API design, auth flows, and building things that hold up in production.

---

## What I Build

| System | Context | Stack |
|---|---|---|
| 🏛️ **Institutional Management Apps** | Internal tools at INETER — workflows, data management, reporting for a technical-scientific org | .NET · Razor · SQL Server |
| ⚾ **Baseball Stadium Ticketing System** | Full POS for a stadium: events, seating maps, barcode ticket validation, cashier sessions, reports. Private network deployment | .NET Core 10 · Angular 21 · PrimeNG · SQL Server · Docker |
| 🔐 **Auth & Access Layer** | JWT-based auth with role and claims management. Refresh token flow, Angular route guards, policy-based authorization on .NET | .NET Identity · JWT · Angular Guards |
| 📋 **Collaborative Enterprise Modules** | Multi-module systems built with teams — approval workflows, inventory control, asset tracking | .NET · Angular · SQL Server |

---

## Stadium Ticketing System — Architecture Snapshot

> *Current project. In development. Private network deployment.*

A multi-module POS for baseball stadiums, designed to run on a local VM within the stadium's private network. No internet dependency — everything runs on-premise.

**7 modules in scope:**
- 🗓️ **Events** — event catalog, team management, base pricing per event
- 🗺️ **Locations** — stadium seating map, sections/rows/seats, per-section pricing addons
- 🎫 **Ticket Sales** — cashier session open/close, seat selection, IVA, barcode ticket generation, courtesy tickets
- 📄 **Documents** — logo/image storage, auto-compression, local VM storage
- 📊 **Reports** — sales by section, by event type, by cashier; PDF + Excel export; real-time dashboards
- 🔒 **Security** — user/role management, audit trails, session policies
- 📡 **Entry Validation** — barcode scanner integration, real-time ticket validation, offline sync

**Infrastructure:**
```
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

**Pricing logic:**
```
Final Price = Event Base Price + Section Price Addon + Discounts - IVA
```

---

## Engineering Approach

### Backend (.NET)

Layered architecture with clean separation between domain logic, application services, and infrastructure. At INETER I work primarily with Razor for server-rendered views; on API projects I structure around RESTful endpoints with proper contracts.

```
Solution/
├── Domain/          # Entities, value objects
├── Application/     # Use cases, DTOs, validators, interfaces
├── Infrastructure/  # EF Core, repositories, file storage, external services
└── API/             # Controllers, middleware, DI config
```

- **Repository pattern** — business logic never touches DbContext directly.
- **DTOs at every boundary** — domain models don't leak into responses.
- **JWT authentication** with ASP.NET Core Identity: role/claims-based authorization, token refresh, middleware-level validation.
- **Global exception handling** via middleware — consistent error responses across all endpoints.
- **Swagger/OpenAPI** on every API project — documented, versioned, consumer-ready.
- **Unit testing** on the Application layer with **xUnit + Moq**.

### Frontend (Angular)

Feature-based module organization, lazy loading by default, smart/dumb component split.

```
src/
├── core/            # Auth, guards, interceptors, global services
├── shared/          # Reusable components, pipes, directives
└── features/
    ├── events/
    ├── ticketing/
    └── reports/
```

- **HTTP Interceptors** handle JWT injection and global error normalization.
- **Route Guards** enforce role-based access at routing level.
- **Reactive Forms** for complex modules — template-driven only for trivial cases.
- **Services own state** — components stay lean and presentational.

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

## GitHub Stats

<div align="center">
  <img width="49%" src="https://github-readme-stats.vercel.app/api?username=Jguevara99&show_icons=true&theme=radical&hide_border=true&count_private=true" />
  <img width="49%" src="https://streak-stats.demolab.com/?user=Jguevara99&theme=radical&hide_border=true" />
</div>

<div align="center">
  <img width="42%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Jguevara99&layout=compact&theme=radical&hide_border=true&langs_count=8" />
</div>

---

## Trophies

<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=Jguevara99&theme=radical&no-frame=true&no-bg=true&margin-w=6&row=1" />
</div>

---

## Contribution Graph

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Jguevara99&theme=react-dark&hide_border=true&area=true" />
</div>

---

## Let's Talk

If you're working on something in the **.NET + Angular** space — enterprise apps, system design, architecture decisions — I'm open to a conversation.

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
