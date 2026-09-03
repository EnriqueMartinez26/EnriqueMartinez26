<div align="center">

# Enrique Leonel Martínez
### Backend / Full Stack Developer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/enrique-leonel-martinez)
[![Email](https://img.shields.io/badge/Email-1e293b?style=flat-square&logo=maildotru&logoColor=white)](mailto:emartinez.03@hotmail.com)
[![Live Demo](https://img.shields.io/badge/Live_Demo-4Fun_Store-1e3a8a?style=flat-square)](https://4fun-store-web.vercel.app)

</div>

<br>

## About

Backend / full stack developer from San Miguel de Tucumán, Argentina. Associate Degree in Programming (UTN, June 2026) — now studying Information Systems Engineering at the same university.

I work with Node.js and TypeScript. What I care about is backend that holds up: well-modeled data, predictable endpoints, and security from the start instead of patched in at the end.

English C1, certified by [EF SET](https://cert.efset.org/mTGDKN).

<br>

## Tech Stack

<div align="center">

![Node.js](https://img.shields.io/badge/Node.js-1e293b?style=flat-square&logo=nodedotjs&logoColor=339933)
![TypeScript](https://img.shields.io/badge/TypeScript-1e293b?style=flat-square&logo=typescript&logoColor=3178C6)
![Express](https://img.shields.io/badge/Express-1e293b?style=flat-square&logo=express&logoColor=white)
![React](https://img.shields.io/badge/React-1e293b?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-1e293b?style=flat-square&logo=nextdotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-1e293b?style=flat-square&logo=postgresql&logoColor=4169E1)
![Prisma](https://img.shields.io/badge/Prisma-1e293b?style=flat-square&logo=prisma&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-1e293b?style=flat-square&logo=docker&logoColor=2496ED)

</div>

<br>

## Featured Project — 4Fun Store

Digital video game marketplace. Associate Degree thesis, built in a two-person team: catalog, authentication, cart, checkout, orders and digital key delivery.

<div align="center">

[![Live](https://img.shields.io/badge/Live-4fun--store--web.vercel.app-1e3a8a?style=for-the-badge)](https://4fun-store-web.vercel.app)
[![API Health](https://img.shields.io/badge/API-health_check-1e3a8a?style=for-the-badge)](https://4fun-store-api.vercel.app/health)

</div>

| | |
| --- | --- |
| API | Node.js · Express · Prisma · PostgreSQL |
| Client | Next.js 15 · React 18 · TypeScript · Zod |
| Auth | JWT in HttpOnly cookies |
| Hardening | Per-IP rate limiting, origin-restricted CORS |
| Tests | 20 with Jest (API) · 43 with Vitest (client) |

Repos: [4fun-store-api](https://github.com/EnriqueMartinez26/4fun-store-api) · [4fun-store-web](https://github.com/EnriqueMartinez26/4fun-store-web)

<br>

## Real problems I've solved

<details open>
<summary><b>Production was running an old version</b></summary>
<br>

The 4Fun Store API started returning 30 products where the count said 28. Two of them should not have been public: one was a draft, the other was suspended. I read the code twice and found nothing. Then I ran the same API locally against the same database and got 28 and 28. The bug was not in the code — the deploy was stale. Now I check what is deployed before I check what is written.

</details>

<details>
<summary><b>A race condition that sat there for three years</b></summary>
<br>

I came back to Komorebi in 2026, three years after finishing it. Two simultaneous purchases could push stock below zero, because reading the stock and writing it were separate operations. I replaced them with an atomic update, made the JWT secret mandatory in production, and moved to secure cookies.

</details>

<details>
<summary><b>A line in .gitignore that hid every test</b></summary>
<br>

The 4Fun frontend had no tests in its entire history. Not because nobody wrote them: `**/*.test.ts` had been in `.gitignore` since April, so every test written for months was silently dropped before it ever reached a commit. I removed the line and wrote the suite.

</details>

<br>

## Other Projects

**[Komorebi](https://komorebi-front.netlify.app)** — full stack e-commerce. Final project for Rolling Code School. REST API in Express and MongoDB with JWT authentication, React 18 client built with Vite. Refactored for security in 2026 — the race condition above.
Repos: [komorebi-back](https://github.com/EnriqueMartinez26/komorebi-back) · [komorebi-front](https://github.com/EnriqueMartinez26/komorebi-front)

**[Shoe store management system](https://github.com/EnriqueMartinez26/proyecto-final-laboratorio-2)** — desktop application in three layers: data access, business logic and presentation. C#, .NET, Windows Forms, SQL Server. Final project for Laboratorio 2 at UTN.

**[Shifty](https://github.com/EnriqueMartinez26/shifty)** — multi-tenant appointment scheduler with integrated payments, built as a team. Python, FastAPI, SQLAlchemy, PostgreSQL, React, TypeScript, Docker.

<br>

<div align="center">

Looking for my first developer role — remote, or on-site in Tucumán, Argentina.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/enrique-leonel-martinez)
[![Email](https://img.shields.io/badge/Email-1e293b?style=flat-square&logo=maildotru&logoColor=white)](mailto:emartinez.03@hotmail.com)

</div>
