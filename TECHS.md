# Techs Used

This document outlines all major technologies used in the **ERP Monorepo**, grouped by domain and functionality.  
Each technology includes a short description and its official documentation link.

---

## 1. Core Monorepo & Tooling

| Technology | Purpose | Documentation |
|-------------|----------|----------------|
| **Turborepo** | High-performance monorepo build system for managing multiple apps and packages. | [Docs](https://turbo.build/repo/docs) |
| **PNPM** | Fast, disk-efficient package manager supporting workspace linking. | [Docs](https://pnpm.io) |
| **TypeScript** | Strongly typed JavaScript for maintainable, scalable codebases. | [Docs](https://www.typescriptlang.org/docs) |
| **ESLint** | Static code analysis tool to identify problematic patterns. | [Docs](https://eslint.org/docs/latest) |
| **Prettier** | Opinionated code formatter for consistent style. | [Docs](https://prettier.io/docs/en/) |
| **Husky** | Git hooks for pre-commit checks. | [Docs](https://typicode.github.io/husky/) |
| **lint-staged** | Runs linters only on staged files. | [Docs](https://github.com/okonet/lint-staged) |
| **Changesets** | Versioning and changelog management for monorepos. | [Docs](https://github.com/changesets/changesets) |
| **Fumadocs** | Modern documentation generator for dev and API docs. | [Docs](https://fumadocs.vercel.app/docs) |

---

## 2. Backend Stack (NestJS Microservices)

| Technology | Purpose | Documentation |
|-------------|----------|----------------|
| **NestJS** | Scalable backend framework for modular server-side apps. | [Docs](https://docs.nestjs.com) |
| **Fastify** | High-performance HTTP server adapter for NestJS. | [Docs](https://www.fastify.io/docs/latest/) |
| **Prisma ORM** | Type-safe ORM for PostgreSQL. | [Docs](https://www.prisma.io/docs) |
| **PostgreSQL** | Reliable open-source relational database. | [Docs](https://www.postgresql.org/docs/) |
| **NATS** | Lightweight pub/sub messaging for microservices. | [Docs](https://docs.nats.io) |
| **BullMQ** | Job queue built on Redis for background jobs and scheduling. | [Docs](https://docs.bullmq.io) |
| **Redis** | In-memory data store for caching and queues. | [Docs](https://redis.io/docs) |
| **Meilisearch** | Fast, typo-tolerant search engine. | [Docs](https://www.meilisearch.com/docs) |
| **Zod** | Schema validation and type inference for DTOs. | [Docs](https://zod.dev) |
| **Swagger (NestJS)** | Auto-generated API documentation for REST endpoints. | [Docs](https://docs.nestjs.com/openapi/introduction) |
| **Stripe** | Subscription and billing integration. | [Docs](https://stripe.com/docs) |
| **@nestjs-modules/mailer** | Mailer module for NestJS using NodeMailer. | [Docs](https://github.com/nest-modules/mailer) |
| **NodeMailer** | Node.js library for sending emails. | [Docs](https://nodemailer.com/about/) |
| **@nestjs/config** | Configuration management for environment variables. | [Docs](https://docs.nestjs.com/techniques/configuration) |
| **Pino** | High-performance JSON logger. | [Docs](https://getpino.io/#/) |
| **Sentry** | Error tracking and performance monitoring. | [Docs](https://docs.sentry.io) |
| **Terminus (NestJS)** | Health check endpoints for microservices. | [Docs](https://docs.nestjs.com/recipes/terminus) |
| **Prometheus** | Metrics collection and monitoring system. | [Docs](https://prometheus.io/docs/) |
| **Grafana** | Visualization and analytics dashboards. | [Docs](https://grafana.com/docs/) |
| **Faker.js** | Fake data generation for testing and seeding. | [Docs](https://fakerjs.dev/guide/) |

---

## 3. Frontend (Next.js + Shadcn + Tailwind)

| Technology | Purpose | Documentation |
|-------------|----------|----------------|
| **Next.js** | React framework for SSR, SSG, and App Router. | [Docs](https://nextjs.org/docs) |
| **Tailwind CSS** | Utility-first CSS framework for building responsive UIs. | [Docs](https://tailwindcss.com/docs) |
| **Shadcn/UI** | Reusable and accessible React components built on Radix + Tailwind. | [Docs](https://ui.shadcn.com/docs) |
| **Zustand** | Lightweight state management library. | [Docs](https://docs.pmnd.rs/zustand/getting-started/introduction) |
| **NextAuth.js** | Authentication for Next.js with OAuth and credentials support. | [Docs](https://authjs.dev/reference/nextjs) |
| **React Hook Form** | Flexible and performant form management. | [Docs](https://react-hook-form.com/get-started) |
| **Framer Motion** | Animation and transition library for React. | [Docs](https://www.framer.com/motion/) |
| **nuqs** | Query parameter state management for Next.js. | [Docs](https://nuqs.47ng.com/) |
| **Evil Charts** | Custom charts built with Recharts and Shadcn UI. | [Docs](https://recharts.org/en-US/) |
| **Gemini API** | AI-powered assistant integration for analytics and automation. | [Docs](https://ai.google.dev/gemini-api/docs) |
| **@react-pdf/renderer** | PDF generation and rendering in React. | [Docs](https://react-pdf.org/) |
| **qrcode.react** | Generate QR codes for invoices and product labels. | [Docs](https://github.com/zpao/qrcode.react) |
| **next-intl** | Internationalization (i18n) for Next.js apps. | [Docs](https://next-intl-docs.vercel.app/docs) |
| **next-themes** | Dark/light theme management for Next.js. | [Docs](https://github.com/pacocoursey/next-themes) |
| **Socket.IO** | Real-time event communication between client and server. | [Docs](https://socket.io/docs/v4/) |

---

## 4. Shared Packages & Architecture

| Package | Purpose | Documentation |
|----------|----------|----------------|
| **@erp/db** | Prisma Client and database utilities. | [Docs](https://www.prisma.io/docs) |
| **@erp/validation** | Shared Zod-based schemas and DTOs. | [Docs](https://zod.dev) |
| **@erp/events** | Event schemas and NATS wrappers for pub/sub. | [Docs](https://docs.nats.io) |
| **@erp/tenancy** | Multi-tenant context handling and isolation logic. | [Docs](https://docs.nestjs.com/fundamentals/custom-providers) |
| **@erp/logger** | Unified logging with Pino and Sentry integration. | [Docs](https://getpino.io/#/) |
| **@erp/config** | Centralized configuration and environment management. | [Docs](https://docs.nestjs.com/techniques/configuration) |
| **@erp/auth** | Authentication utilities, guards, and strategies. | [Docs](https://authjs.dev/reference/nextjs) |
| **@erp/utils** | Common utility functions (date, currency, formatting, etc.). | [Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript) |
| **@erp/ui** | Shared Shadcn UI components and design system. | [Docs](https://ui.shadcn.com/docs) |

---

## 5. DevOps & Infrastructure

| Technology | Purpose | Documentation |
|-------------|----------|----------------|
| **Docker Compose** | Containerized local development for databases, queues, and services. | [Docs](https://docs.docker.com/compose/) |
| **GitHub Actions** | CI/CD pipelines for build, test, and deploy. | [Docs](https://docs.github.com/en/actions) |
| **AWS S3** | Object storage for uploads, invoices, and documents. | [Docs](https://docs.aws.amazon.com/s3/) |
| **Mailgun / AWS SES** | Production-ready email delivery. | [Mailgun Docs](https://documentation.mailgun.com/en/latest/) / [AWS SES Docs](https://docs.aws.amazon.com/ses/) |
| **Prometheus + Grafana** | Monitoring and visualization for system metrics. | [Prometheus Docs](https://prometheus.io/docs/) / [Grafana Docs](https://grafana.com/docs/) |
| **Sentry** | Application monitoring and error tracking. | [Docs](https://docs.sentry.io) |

---

## Summary

This monorepo architecture combines **Next.js, NestJS, Prisma, NATS, Meilisearch, and Stripe** under **Turborepo** with a shared **TypeScript + Zod** ecosystem.  
It ensures scalability, strong typing, modular separation, real-time updates, and modern UI/UX powered by **Tailwind + Shadcn + Framer Motion**.
