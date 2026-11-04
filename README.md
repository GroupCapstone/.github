# Group Capstone

A culminating team research dissertation and capstone project submitted in partial fulfillment of the requirements for the degree, demonstrating full-stack system architecture and enterprise school management.

---

## Overview

The Group Capstone organization hosts the source code repositories, engineering specifications, and architectural documentation for the **SNPI School Management System (SNP-SMS)**, an enterprise-grade multi-tenant educational administration platform designed for Cambodian academic institutions.

- **Status**: Active Development & Quality Verification
- **Testing Domain**: [snpis.kesararamwithdigital.tech](https://snpis.kesararamwithdigital.tech)
- **Location**: Cambodia
- **Team**: Team Research Dissertation (`@GroupCapstone/team-research-dissertation`)

---

## Core System Architecture

The project implements a decoupled hybrid architecture comprising a high-performance Next.js web application and a 7-layer modular monolith backend API:

```
+-------------------------------------------------------------------------+
|                                Client Tier                              |
|   Next.js 16 (App Router) - React 19 - Tailwind CSS - Radix UI         |
|   Domain: https://snpis.kesararamwithdigital.tech                       |
+-------------------------------------------------------------------------+
                                    |
                    Server-Side Proxy (/api/v1/*)
                                    |
+-------------------------------------------------------------------------+
|                                Backend API                              |
|   Express 5 - TypeScript - 7-Layer Modular Monolith Architecture       |
|   Modules: 47 Domain Modules - 193 REST API Endpoints                  |
+-------------------------------------------------------------------------+
                                    |
+-------------------------------------------------------------------------+
|                               Persistence                               |
|   MongoDB Replica Set (rs0) - ACID Distributed Transactions            |
+-------------------------------------------------------------------------+
```

---

## Repositories

| Repository | Role | Technology Stack |
| :--- | :--- | :--- |
| **`SNPI-Web`** | Frontend Web Application | Next.js 16 (App Router), React 19, TypeScript, Tailwind CSS, SWR |
| **`SNPI-API`** | Modular Monolith Backend API | Express 5, TypeScript, Mongoose, MongoDB Replica Set, Zod, JWT |
| **`.github`** | Organization Profile & Workflows | Global community health files, issue templates, organization standards |

---

## Architecture & Security Principles

- **Zero-Bridge Architecture**: Strict operational decoupling between GitHub version control and Vercel hosting. Production deployments are executed via explicit CLI workflows with zero automated webhook triggers.
- **7-Layer Backend Hierarchy**: Strict structural separation across `route -> controller -> service -> repository -> model -> validation -> types`.
- **RBAC & Multi-Tenancy**: Tenant boundary isolation enforcing `schoolId` and `branchId` scoping on all data access patterns.
- **Cryptographic Key Hygiene**: Timing-safe comparisons via `crypto.timingSafeEqual` and zero-leakage credential isolation.
- **CI/CD Quality Gates**: 100% green verification requiring zero ESLint errors, zero TypeScript errors, passing Vitest suites, and pre-deployment manifest audits.

---

## Team & Governance

- **Organization**: [Group Capstone](https://github.com/GroupCapstone)
- **Lead Contributors**:
  - `shiliaiwei` (Full-Stack Architecture & Systems Engineering)
  - `Tan-Saphea` (Core Development & Systems Collaboration)
- **Team**: `team-research-dissertation`
