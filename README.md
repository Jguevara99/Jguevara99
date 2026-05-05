<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&pause=1200&color=3670FF&center=true&vCenter=true&width=750&lines=Jairo+Guevara+%E2%80%94+Full+Stack+Developer;.NET+%7C+Angular+%7C+Enterprise+Systems;Building+systems+that+actually+scale.)](https://git.io/typing-svg)

<img src="https://komarev.com/ghpvc/?username=Jguevara99&label=Profile+Views&color=3670ff&style=for-the-badge" alt="Profile views" />

</div>

---

## Who I Am

Full Stack Developer with **3+ years of experience** building production systems across different teams and contexts.

At **INETER** *(Feb 2023 – present)* — a technical-scientific institution in Nicaragua — I develop internal tools with **.NET and Razor**: operational workflows, data management and institutional reporting.

In parallel, I collaborate with a separate development team on a **baseball stadium ticketing POS** — a full multi-module system built with **.NET Core 10 + Angular 21**, deployed on a private network VM with Docker. Independent project, different team, different stack.

---

## 📍 Current & Past Systems

**💼 INETER** *(Feb 2023 – present · Full-time)*

| System | What it does | Stack |
|---|---|---|
| 🏛️ **Institutional Management Apps** | Internal workflows, data management and reporting at institutional scale | .NET · Razor · SQL Server |

**🤝 External Team Projects** *(independent collaborations)*

| System | What it does | Stack |
|---|---|---|
| ⚾ **Baseball Stadium Ticketing POS** | Full POS for a stadium — events, seating maps, cashier sessions, barcode tickets, entry validation. Private network deployment | .NET Core 10 · Angular 21 · PrimeNG · SQL Server · Docker |
| 🔐 **Auth & Access Module** | JWT auth with role/claims, refresh token flow, Angular guards, policy-based authorization | .NET Identity · JWT · Angular |
| 📋 **Enterprise Modules** | Multi-module apps — asset tracking, inventory control, approval workflows | .NET · Angular · SQL Server |

### Stadium POS — Architecture at a Glance

```
Private Network VM
├── .NET Core 10 API  →  Domain / Application / Infrastructure / API
├── Angular 21 SPA    →  Feature modules, lazy loading, JWT interceptors
├── SQL Server        →  Docker container, EF Core migrations
└── Reverse Proxy     →  Internal routing, no public exposure
```

On-premise · Role-based access (Admin / Operator / Manager) · Barcode validation at entry gates · `Base Price + Section Addon ± Discounts + IVA` · PDF/Excel reports per cashier and event

---

## ⚙️ How I Build

| Layer | Approach |
|---|---|
| **Backend structure** | Clean layered architecture — Domain · Application · Infrastructure · API |
| **Data access** | Repository pattern — business logic never touches DbContext directly |
| **API contracts** | DTOs at every boundary, versioned routes (`/api/v1/`), Swagger on every project |
| **Auth** | JWT + ASP.NET Identity — role/claims-based, refresh tokens, middleware validation |
| **Reliability** | Global exception middleware, EF Core Migrations per environment, never manual in prod |
| **Testing** | xUnit + Moq on the Application layer — use cases tested in isolation from infrastructure |
| **Frontend** | Feature modules, lazy loading, HTTP Interceptors for JWT + error handling, Reactive Forms |

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
