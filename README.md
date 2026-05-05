<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&pause=1200&color=3670FF&center=true&vCenter=true&width=850&lines=Jairo+Guevara+%E2%80%94+Full+Stack+Developer;.NET+%7C+Angular+%7C+Enterprise+Systems;Building+systems+that+actually+scale.)](https://git.io/typing-svg)

<img src="https://komarev.com/ghpvc/?username=Jguevara99&label=Profile+Views&color=3670ff&style=for-the-badge" alt="Profile views" />

</div>

---

## 👋 About Me

I’m a Full Stack Developer focused on **enterprise and institutional systems**.
At **INETER** (Nicaragua), I build internal software with **.NET + Razor** for real-world operational workflows, reporting, and data governance.

Beyond INETER, I collaborate on full-stack products using **.NET APIs + Angular**—from architecture and auth flows to deployment and operations.

I’m especially interested in:
- clean architecture and maintainable codebases,
- scalable backend design,
- production-ready frontend workflows,
- and systems that perform reliably in real environments.

---

## 🚀 What I’m Building Now

> Active project (2026): **Baseball Stadium Ticketing System**

A multi-module POS platform designed for stadium operations on a **private on-premise network**:

- Event and team management
- Seating map + dynamic section pricing
- Cashier sessions and ticket issuance
- Barcode validation at entry points
- Sales analytics and exportable reports

**Stack:** `.NET Core 10` · `Angular 21` · `PrimeNG` · `SQL Server` · `Docker` · `JWT`

---

## 🧩 Systems I Build

| System | Context | Stack |
|---|---|---|
| 🏛️ **Institutional Management Apps** | Internal tools at INETER: workflows, reporting, data management | .NET · Razor · SQL Server |
| ⚾ **Stadium Ticketing Platform** | End-to-end POS: events, seats, barcode access, cashier sessions, reports | .NET Core 10 · Angular 21 · PrimeNG · SQL Server · Docker |
| 🔐 **Authentication & Authorization** | JWT auth, refresh tokens, role/claims policies, guarded routes | ASP.NET Identity · JWT · Angular Guards |
| 📋 **Enterprise Modules** | Approval flows, inventory, asset tracking, audit-friendly operations | .NET · Angular · SQL Server |

---

## 🏗️ Architecture Snapshot (Ticketing Project)

```text
Private Stadium Network
└── Production VM
    ├── .NET Core 10 API
    ├── Angular 21 Frontend
    ├── SQL Server (Docker)
    ├── Reverse Proxy
    └── Local Document Storage

└── Docker (Test/Staging)
    ├── Test API
    └── Test Database
```

### Core Modules in Scope

1. **Events** — catalog, teams, base pricing
2. **Locations** — sections/rows/seats, section addons
3. **Ticket Sales** — cashier open/close, seat selection, barcode generation, courtesy tickets
4. **Documents** — logo/image storage and compression
5. **Reports** — by section/event/cashier + PDF/Excel exports
6. **Security** — users, roles, audit trails, policy controls
7. **Entry Validation** — scanner integration and ticket status checks

---

## ⚙️ Engineering Approach

### Backend (.NET)

```text
Solution/
├── Domain/          # Entities, value objects
├── Application/     # Use cases, DTOs, validators, interfaces
├── Infrastructure/  # EF Core, repositories, file/document services
└── API/             # Controllers, middleware, DI config
```

- Layered architecture with strict boundary separation
- Repository pattern (no direct business-layer DbContext usage)
- DTO-driven contracts to avoid domain leakage
- JWT + Identity with role/claims-based authorization
- Centralized exception handling middleware
- Swagger/OpenAPI-first API documentation
- Application-layer unit testing with **xUnit + Moq**

### Frontend (Angular)

```text
src/
├── core/            # Auth, guards, interceptors, global services
├── shared/          # Reusable components, pipes, directives
└── features/
    ├── events/
    ├── ticketing/
    └── reports/
```

- Feature-first modular organization
- Lazy loading by default
- Route-level access control with guards
- Interceptors for auth token injection and error normalization
- Reactive forms for complex workflows

---

## 🛠️ Tech Stack

### Backend
![.NET](https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white)
![Razor](https://img.shields.io/badge/Razor-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)
![Entity Framework](https://img.shields.io/badge/Entity%20Framework-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black)

### Frontend
![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![RxJS](https://img.shields.io/badge/RxJS-B7178C?style=for-the-badge&logo=reactivex&logoColor=white)
![PrimeNG](https://img.shields.io/badge/PrimeNG-DD0031?style=for-the-badge&logo=primeng&logoColor=white)

### Testing & Tooling
![xUnit](https://img.shields.io/badge/xUnit-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![Moq](https://img.shields.io/badge/Moq-239120?style=for-the-badge&logo=c-sharp&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)

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

## 🤝 Let’s Connect

If you’re building in the **.NET + Angular** space and need help with architecture, implementation, or scaling, I’m open to collaborate.

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
