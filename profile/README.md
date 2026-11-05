# Group Capstone

A culminating team research dissertation and capstone project submitted in partial fulfillment of the requirements for the degree, demonstrating full-stack system architecture and enterprise software engineering.

---

## Pronunciation and Semantic Identity

| Aspect | Detail | Explanation |
| :--- | :--- | :--- |
| **Organization Name** | **Group Capstone** | Official organization identifier on GitHub |
| **International Phonetic Alphabet (IPA)** | `/ɡruːp ˈkæp.stoʊn/` | International standard phonetic transcription |
| **Syllable Respelling** | **GROOP KAP-stohn** | Pronounced with primary stress on `GROOP` and `KAP` |
| **Definition** | **Culminating Dissertation Project** | A final-year research dissertation and production system demonstrating complete engineering competence |

---

## Overview

The Group Capstone organization hosts the source code repositories, engineering specifications, and architectural documentation for an enterprise-grade multi-tenant web application and modular monolith backend API.

- **Status**: Active Development & Quality Verification
- **Testing Domain**: [snpis.kesararamwithdigital.tech](https://snpis.kesararamwithdigital.tech)
- **Design & Document Portal**: [snpis.kesararamwithdigital.tech/document/design](https://snpis.kesararamwithdigital.tech/document/design)
- **Location**: Cambodia
- **Team**: Team Research Dissertation (`@GroupCapstone/team-research-dissertation`)

---

## Core System Architecture

The platform implements a decoupled hybrid architecture comprising a high-performance Next.js web application and a 7-layer modular monolith backend API:

```
+-------------------------------------------------------------------------+
|                                Client Tier                              |
|   Next.js 16 (App Router) - React 19 - Tailwind CSS - Radix UI         |
|   Design Portal: https://snpis.kesararamwithdigital.tech/document/design|
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

| Repository | Visibility | Role | Technology Stack |
| :--- | :--- | :--- | :--- |


---

## Architecture & Security Principles

- **Zero-Bridge Architecture**: Strict operational decoupling between GitHub version control and Vercel hosting. Production deployments are executed via explicit CLI workflows with zero automated webhook triggers.
- **7-Layer Backend Hierarchy**: Strict structural separation across `route -> controller -> service -> repository -> model -> validation -> types`.
- **RBAC & Multi-Tenancy**: Tenant boundary isolation enforcing organizational scoping on all data access patterns.
- **Branch Protection & Quality Gates**: Main branches protected with pull request review enforcement, deletion prevention, and automated CI quality checks.
- **Zero-Emoji Policy**: Clean textual badges and professional technical documentation across all repositories.

---

## Team & Governance

- **Organization**: [Group Capstone](https://github.com/GroupCapstone)
- **Lead Contributors**:
  - `shiliaiwei` (Full-Stack Architecture & Systems Engineering)
  - `Tan-Saphea` (Core Development & Systems Collaboration)
- **Team**: `team-research-dissertation`
