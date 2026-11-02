# RevoFlux Full-Stack B2B Multi-Tenant SaaS Boilerplate

[![Next.js 15](https://img.shields.io/badge/Next.js-15-black?style=flat-square&logo=next.js)](https://nextjs.org/)
[![Stripe](https://img.shields.io/badge/Stripe-Billing-635BFF?style=flat-square&logo=stripe)](https://stripe.com/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-336791?style=flat-square&logo=postgresql)](https://www.postgresql.org/)
[![Prisma ORM](https://img.shields.io/badge/Prisma-6.x-2D3748?style=flat-square&logo=prisma)](https://www.prisma.io/)
[![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-v4-38B2AC?style=flat-square&logo=tailwind-css)](https://tailwindcss.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)

A production-ready, full-stack multi-tenant SaaS starter kit engineered by [RevoFlux](https://revoflux.app) with automated Stripe subscription billing, team organization workspaces, invite mechanics, and usage-based metered billing.

---

## ⚡ Key Highlights

- **Multi-Tenant Workspaces**: Instant switching between personal accounts and multiple corporate organizations.
- **Stripe Billing Integration**: Self-service customer billing portal, recurring subscriptions, and webhook reconciliation.
- **Team Roles & Permissions**: Owner, Admin, Member, and Viewer role-based security.
- **PostgreSQL & Prisma Core**: Type-safe relational schema with database cascade rules.

---

## 🏗️ Architecture

```text
revoflux-subscription-saas/
├── prisma/
│   └── schema.prisma         # Organization, membership, and subscription schema
├── src/
│   └── app/
│       └── api/
│           └── webhooks/
│               └── stripe/   # Stripe billing lifecycle listeners
├── docker-compose.yml        # PostgreSQL & Next.js service orchestration
├── package.json
└── README.md
```

---

## 🚀 Quick Start

```bash
docker-compose up -d db
npm install
npx prisma generate
npm run dev
```
Open [http://localhost:3002](http://localhost:3002) to access the SaaS boilerplate.

---

## 📄 License
Released under the [MIT License](LICENSE). Built and maintained by [RevoFlux](https://revoflux.app).

**Custom SaaS Architecture & Enterprise Builds:** [revoflux.ai@gmail.com](mailto:revoflux.ai@gmail.com) | [Founder LinkedIn](https://www.linkedin.com/in/muhammad-dawood-dev)
