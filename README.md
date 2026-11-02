# RevoFlux Full-Stack Multi-Tenant SaaS & Commerce Monorepo

[![Next.js 15](https://img.shields.io/badge/Next.js-15-black?style=flat-square&logo=next.js)](https://nextjs.org/)
[![Turborepo](https://img.shields.io/badge/Turborepo-Active-EF4444?style=flat-square&logo=turborepo)](https://turbo.build/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-blue?style=flat-square&logo=typescript)](https://www.typescriptlang.org/)
[![Prisma ORM](https://img.shields.io/badge/Prisma-6.x-2D3748?style=flat-square&logo=prisma)](https://www.prisma.io/)
[![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-v4-38B2AC?style=flat-square&logo=tailwind-css)](https://tailwindcss.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)

An enterprise-grade, full-stack multi-tenant commerce and subscription management platform built with Turborepo monorepo architecture by [RevoFlux](https://revoflux.app). Features high-converting customer storefronts and comprehensive administrative CMS control panels.

---

## ⚡ Architecture & Monorepo Workspaces

```text
revoflux-subscription-saas/
├── apps/
│   ├── admin/                # Executive CMS admin dashboard (Products, Orders, Customers)
│   └── storefront/           # Customer-facing shopping storefront (Next.js App Router)
├── packages/
│   ├── mail/                 # Transactional email dispatcher
│   ├── oauth/                # Social authentication provider adapters
│   ├── sms/                  # SMS gateway integrations
│   └── regex/                # Data validation utilities
├── prisma/                   # PostgreSQL schema & database migrations
├── docker-compose.yml        # PostgreSQL & service orchestration
├── package.json
└── README.md
```

---

## 🚀 Quick Start

### 1. Install Dependencies Across Monorepo
```bash
npm install
```

### 2. Generate Prisma Client & Run Migrations
```bash
npx prisma generate
npx prisma migrate dev
```

### 3. Launch Monorepo Applications
```bash
npm run dev
```
- **Storefront Application:** [http://localhost:3000](http://localhost:3000)
- **Executive Admin CMS:** [http://localhost:3001](http://localhost:3001)

---

## 📄 License
Released under the [MIT License](LICENSE). Maintained by [RevoFlux](https://revoflux.app).

**Custom SaaS Architecture & Enterprise Monorepos:** [revoflux.ai@gmail.com](mailto:revoflux.ai@gmail.com) | [Founder LinkedIn](https://www.linkedin.com/in/muhammad-dawood-dev)
