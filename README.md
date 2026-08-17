<div align="center">

# Muhammad Awais Ashraf

### Full-Stack Software Engineer

Building secure, production-deployed web applications end to end —
APIs, databases, background jobs, and the interfaces on top of them.

[![Portfolio](https://img.shields.io/badge/Portfolio-awais--ashraf.dev-6D28D9?style=flat-square&logo=vercel&logoColor=white)](https://awais-ashraf.dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/muhammad-awais-ashraf/)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:mhawais431@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/awais1019)

![Profile Views](https://komarev.com/ghpvc/?username=awais1019&style=flat-square)

</div>

---

## About

I'm a Computer Science graduate from UET Lahore, building full-stack web applications end to end — REST APIs, authentication systems, and database schemas on the backend; responsive, type-safe interfaces on the frontend.

Most of my projects are solo-built and production-deployed, not tutorial-scale: real authentication (JWT, OAuth, RBAC), real background job processing (BullMQ/Redis), real CI/CD gating releases on a passing test suite. My strongest area is backend architecture and authorization design — I've caught and fixed a real privilege-escalation bug in one of my own APIs, which is the kind of thing you only learn to watch for by shipping.

I work comfortably across two backend stacks (NestJS/Express, PostgreSQL/MongoDB) and two frontend frameworks (React/Next.js, Vue 3), and I'm currently seeking **Software Engineer**, **Full-Stack**, or **Backend Developer** opportunities.

---

## Now

- Built and deployed [**Dev-Collab**](https://github.com/awais1019/dev-collab), a solo full-stack team collaboration platform, in August 2026
- Sharpening backend architecture: transactions, background workers, caching, and system design
- Writing more tests earlier — Dev-Collab shipped with 123 backend tests gating its CI/CD pipeline
- Open to Software Engineering, Full-Stack, and Backend Developer roles

---

## Tech Stack

**Languages**
`TypeScript` `JavaScript (ES2023+)` `SQL`

**Frontend**
`React` `Next.js` `Vue 3` `Pinia` `Tailwind CSS` `shadcn/ui` `React Query` `React Hook Form` `VeeValidate` `Chart.js`

**Backend**
`NestJS` `Express.js` `Node.js` `REST API Design` `JWT` `OAuth 2.0` `Passport.js` `RBAC` `Zod`

**Databases & Data**
`PostgreSQL` `Prisma ORM` `MongoDB` `Mongoose` `Redis` `BullMQ`

**Testing & CI/CD**
`Jest` `Supertest` `GitHub Actions`

**Tools & Platforms**
`Git` `Docker` `Vercel` `Heroku` `Turborepo` `pnpm workspaces`

---

## Featured Projects

### [Dev-Collab](https://github.com/awais1019/dev-collab) — Team Collaboration Platform
**Solo project** · Live at [dev-collab.tech](https://dev-collab.tech)

A GitHub/Linear-inspired collaboration platform — teams, projects, Kanban tasks, comments, notifications, and analytics — built as a pnpm monorepo with a shared Zod schema package used by both the API and the client.

- Two independent permission systems (JWT-only platform role, database-checked team role) chained through four access middlewares
- Found and closed a real privilege-escalation path where self-assigning a task silently granted delete rights
- MongoDB transactions for cascading deletes and multi-document status changes
- BullMQ + Redis notification worker running as a separate process from the API
- 123 Jest + Supertest tests against a real in-memory MongoDB replica set
- Deployed to Heroku (API + worker dynos) and Vercel, released through a GitHub Actions pipeline gated on the full test suite

**Stack:** Vue 3 · TypeScript · Express.js · MongoDB · Redis · BullMQ · Zod · Tailwind CSS

---

### [PetSoft](https://github.com/awais1019/PetSoft) — Pet Daycare Management Platform
**Solo project** · Live at [pet-soft-beige.vercel.app](https://pet-soft-beige.vercel.app/)

A full-stack pet management SaaS with authenticated CRUD, Stripe-gated premium subscriptions, and Server Actions throughout.

- CRUD workflows via Next.js Server Actions and Prisma, with a reusable shadcn/ui component library
- Stripe subscription payments verified server-side through webhook signatures, not client-reported state
- Solved a Next.js 15 edge middleware bundle-size limit with a two-layer auth check — lightweight JWT at the edge, full NextAuth v5 session validation in-app
- Found and fixed a real production bug: a gap in the middleware's authorization logic let one specific request state fall through to an implicit `false`, crashing a live Server Action instead of redirecting

**Stack:** Next.js 15 · TypeScript · Prisma · NextAuth v5 · Stripe · Tailwind CSS

---

### [Evento](https://github.com/awais1019/Evento) — Event Discovery Platform
**Solo project** · Live at [evento-pi-ashen.vercel.app](https://evento-pi-ashen.vercel.app/)

A server-rendered event discovery platform with dynamic city-based routing.

- Server Components for Prisma-backed, paginated event listings — no separate API route
- Zod-validated data boundaries between the database and UI
- Responsive interface with Framer Motion page transitions
- Came back a year after shipping to patch a critical Next.js RCE (React Flight protocol) plus several SSRF/DoS/cache-poisoning CVEs — dependency maintenance, not just initial delivery

**Stack:** Next.js 15 · TypeScript · Prisma · Zod · Tailwind CSS · Framer Motion

---

### NanoLink — AI-Powered URL Management Platform *(Final Year Project)*
**4-person team** · Primary contributor for authentication · Repository private (academic team project)

A URL management, analytics, and monetization platform built as a capstone project in a Turborepo monorepo. My contribution was the authentication system end to end — the platform's short-link, analytics, and AI features were built by my teammates.

- Local + Google/GitHub OAuth login via Passport.js strategies, unified into a single TokenService
- 6-digit OTP email verification and rate-limited password reset
- Role-based access control via custom NestJS Guards
- Shared Zod validation schemas between the NestJS API and Next.js frontend

**Stack:** Next.js · NestJS · TypeScript · PostgreSQL · Prisma · Turborepo

---

## Engineering Philosophy

I approach problems by understanding the data and the API contract first, then building the interface around it — not the other way around. I prioritize:

- **Clarity over cleverness** — code that's readable six months later
- **Consistent API design** — predictable, well-structured REST endpoints
- **Data integrity** — thoughtful schema design before writing business logic, transactional writes where a partial update would corrupt state
- **Iterative delivery** — shipping working increments, gated by tests, over big-bang releases

---

## Contribution Activity

<div align="center">
<img src="https://raw.githubusercontent.com/awais1019/awais1019/output/github-contribution-grid-snake.svg" alt="contribution graph" />
</div>

---

## GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=awais1019&show_icons=true&theme=default&hide_border=true&count_private=true" height="165" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=awais1019&layout=compact&theme=default&hide_border=true" height="165" />

<br/>

[![GitHub Streak](https://streak-stats.demolab.com/?user=awais1019&theme=default&hide_border=true&date_format=j%20M%5B%20Y%5D)](https://git.io/streak-stats)

</div>

---

## Let's Connect

I'm always interested in discussing software engineering, backend architecture, and full-stack development. If you're hiring or would like to collaborate, feel free to reach out.

- [Portfolio](https://awais-ashraf.dev)
- [LinkedIn](https://www.linkedin.com/in/muhammad-awais-ashraf/)
- [Email](mailto:mhawais431@gmail.com)
