<div align="center">

# 🎓 TeachMeter

**Empowering students, educators, and academic institutions through transparent, structured, and constructive evaluations.**

[![Fastify](https://img.shields.io/badge/Fastify-5.x-000000?style=for-the-badge&logo=fastify&logoColor=white)](https://github.com/Teach-Meter/teachmeter-server)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://github.com/Teach-Meter/teachmeter-web)
[![Flutter](https://img.shields.io/badge/Flutter-3.x-02569B?style=for-the-badge&logo=flutter&logoColor=white)](https://github.com/Teach-Meter/teachmeter-mobile)
[![Prisma](https://img.shields.io/badge/Prisma-7.x-2D3748?style=for-the-badge&logo=prisma&logoColor=white)](https://www.prisma.io/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)

</div>

---

## 🌟 About TeachMeter

TeachMeter is a full-stack social platform that enables students to constructively rate, review, and evaluate academic instructors, faculty, deans, and educational institutions (universities, colleges, and schools). 

Designed with enterprise-grade modular architecture, TeachMeter provides seamless experiences across web and mobile platforms with real-time sync, strict validation, and multi-layered profanity filtering.

---

## 🏛️ System Architecture

```mermaid
graph TD
    subgraph Clients ["Client Applications"]
        Web["🌐 Web Client<br/>(React 19 + Vite + Chakra UI)"]
        Mobile["📱 Mobile Client<br/>(Flutter + Riverpod)"]
    end

    subgraph Backend ["Core API Gateway"]
        Server["⚡ Fastify REST Server<br/>(TypeScript + TypeBox + Sentry)"]
    end

    subgraph Data ["Data & Storage Layer"]
        DB[("🐘 PostgreSQL<br/>Prisma 7 ORM")]
        Cache[("⚡ Redis<br/>Sessions & Caching")]
    end

    Web -->|HTTP / JSON| Server
    Mobile -->|HTTP / JSON| Server
    Server --> DB
    Server --> Cache
```

---

## 📦 Repositories

| Repository | Description | Primary Stack | Status |
| :--- | :--- | :--- | :---: |
| **[`teachmeter-server`](https://github.com/Teach-Meter/teachmeter-server)** | High-performance backend REST API, validation engine, and auth service. | Fastify, TypeScript, Prisma, Redis | Active |
| **[`teachmeter-web`](https://github.com/Teach-Meter/teachmeter-web)** | Modern, accessible web application and administrative dashboard. | React 19, Vite, TanStack, Chakra UI | Active |
| **[`teachmeter-mobile`](https://github.com/Teach-Meter/teachmeter-mobile)** | Native cross-platform mobile client for iOS and Android. | Flutter, Dart, Riverpod, Dio | Active |

---

## 🚀 Key Features

- **Multi-Factor Evaluations**: Rate instructors across clarity, grading fairness, helpfulness, and course workload.
- **Institutional Benchmarking**: Explore institutions and departments with aggregated sentiment metrics.
- **Automated Moderation**: Content moderation with English and multilingual profanity filtering.
- **Secure Authentication**: Strict JWT authentication with token rotation and Redis session management.
- **Progressive Standards**: Unified Agent Skills configured across all projects for streamlined continuous development.

---

<div align="center">
<sub>Maintained with ❤️ by the <a href="https://github.com/Teach-Meter">TeachMeter</a> Team.</sub>
</div>
