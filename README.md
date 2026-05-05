<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&pause=1200&color=3670FF&center=true&vCenter=true&width=750&lines=Jairo+Guevara+%E2%80%94+Full+Stack+Developer;.NET+%7C+Angular+%7C+Enterprise+Systems;Building+systems+that+actually+scale.)](https://git.io/typing-svg)

<img src="https://komarev.com/ghpvc/?username=Jguevara99&label=Profile+Views&color=3670ff&style=for-the-badge" alt="Profile views" />

</div>

---

## Who I Am

Full Stack Developer with **4+ years of experience** designing and shipping production systems. I build backend APIs and Angular frontends for enterprise and institutional environments — systems that handle real operational complexity, run on private networks, and stay maintainable past the first deploy.

Currently at **INETER** (Nicaragua) building internal tools with **.NET + Razor**. On the side, leading architecture on a full **stadium ticketing POS** — 7 modules, Docker deployment, barcode validation, on-premise network.

---

## 📍 Current & Past Systems

| System | What it does | Stack |
|---|---|---|
| ⚾ **Stadium Ticketing POS** | Full POS for a baseball stadium — events, seating, cashier sessions, barcode tickets, entry validation. Runs on a private VM, no internet dependency. | .NET Core 10 · Angular 21 · PrimeNG · SQL Server · Docker |
| 🏛️ **INETER Internal Tools** | Institutional workflows, data management and reporting for a government technical org | .NET · Razor · SQL Server |
| 🔐 **Auth & Access Module** | JWT auth with role/claims, refresh token flow, Angular guards, policy-based authorization | .NET Identity · JWT · Angular |
| 📋 **Enterprise Modules** | Multi-module apps built with teams — asset tracking, inventory, approval workflows | .NET · Angular · SQL Server |

### Stadium POS — Architecture at a Glance

```
Private Network VM
├── .NET Core 10 API     → Layered: Domain / Application / Infrastructure / API
├── Angular 21 SPA       → Feature modules, lazy loading, JWT interceptors
├── SQL Server           → Docker container, EF Core migrations
└── Reverse Proxy        → Internal routing, no public exposure
```

- On-premise deployment — no cloud dependency, air-gapped network
- Role-based access: Admin · Sales Operator · Manager
- Barcode generation + real-time scanner validation at entry gates
- Pricing engine: `Base Event Price + Section Addon ± Discounts + IVA`
- PDF/Excel reporting per cashier, section, and event

---

## ⚙️ Engineering Principles

```
Solution/
├── Domain/          # Entities, value objects
├── Application/     # Use cases, DTOs, validators
├── Infrastructure/  # EF Core, repos, file storage
└── API/             # Controllers, middleware, DI
```

- **Repository pattern** — business logic never touches DbContext directly
- **DTOs at every boundary** — domain models don't leak into responses
- **EF Core Migrations** per environment — schema changes tracked, never manual in prod
- **Global exception middleware** — consistent error shape across all endpoints
- **API versioning** via route prefix — consumers don't break on updates
- **xUnit + Moq** on the Application layer — use cases tested in isolation

```
src/
├── core/       # Auth, guards, interceptors
├── shared/     # Reusable components, pipes
└── features/   # Lazy-loaded feature modules
```

- HTTP Interceptors handle JWT injection and error normalization globally
- Reactive Forms for complex modules, services own state, components stay lean

---

## 🛠️ Stack

**Backend**
![.NET](https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white)
![Razor](https://img.shields.io/badge/Razor-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)
![EF Core](https://img.shields.io/badge/EF%20Core-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black)

**Frontend**
![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![RxJS](https://img.shields.io/badge/RxJS-B7178C?style=for-the-badge&logo=reactivex&logoColor=white)
![PrimeNG](https://img.shields.io/badge/PrimeNG-DD0031?style=for-the-badge&logo=primeng&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

**Infra & Tools**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![DevExpress](https://img.shields.io/badge/DevExpress-FF7200?style=for-the-badge&logo=devexpress&logoColor=white)
![Visual Studio](https://img.shields.io/badge/Visual%20Studio-5C2D91?style=for-the-badge&logo=visual-studio&logoColor=white)

**Testing**
![xUnit](https://img.shields.io/badge/xUnit-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![Moq](https://img.shields.io/badge/Moq-239120?style=for-the-badge&logo=c-sharp&logoColor=white)

**Also worked with**
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-0078D4?style=for-the-badge&logo=visual-studio-code&logoColor=white)

---

## 📊 GitHub Stats

<div align="center">
  <img height="180px" src="https://github-stats-alpha.vercel.app/api?username=Jguevara99&cc=000&tc=ff6ec7&ic=fff&bc=000" />
  <img height="180px" src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Jguevara99&theme=radical" />
</div>

---

## Let's Talk

Open to **remote opportunities** in the .NET + Angular space — full-time or freelance. Based in Nicaragua.

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jairo-guevara)
[![Portfolio](https://img.shields.io/badge/Portfolio-Vercel-3670ff?style=for-the-badge&logo=vercel&logoColor=white)](https://portafolio-kappa-six-51.vercel.app/)
[![Instagram](https://img.shields.io/badge/Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/jairguev27/)
[![X](https://img.shields.io/badge/X-%23000000?style=for-the-badge&logo=x&logoColor=white)](https://twitter.com/guevara_a1/)
[![Facebook](https://img.shields.io/badge/Facebook-%231877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/jairoantonio.guevaraampie)

</div>

---

<div align="center">
  <sub><i>"Talk is cheap. Show me the code." — Linus Torvalds</i></sub>
</div>

  <sub><i>"Talk is cheap. Show me the code." — Linus Torvalds</i></sub>
</div>
