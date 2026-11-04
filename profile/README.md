# ក្រុមសារណាបញ្ចប់ការសិក្សា — Group Capstone

គម្រោងស្រាវជ្រាវសារណា និងការអភិវឌ្ឍប្រព័ន្ធគ្រប់គ្រងសាលារៀនពហុបរិវេណ **SNPI School Management System (SNP-SMS)** សម្រាប់ការបញ្ចប់ថ្នាក់បរិញ្ញាបត្របច្ចេកវិទ្យាព័ត៌មានវិទ្យា។

A culminating team research dissertation and capstone project submitted in partial fulfillment of the requirements for the degree, demonstrating full-stack system architecture and enterprise school management.

---

## របៀបបញ្ចេញសំឡេង និងអត្ថន័យ (Pronunciation & Meaning)

| ផ្នែក (Aspect) | ព័ត៌មានលម្អិត (Details) | ការពន្យល់ (Explanation) |
| :--- | :--- | :--- |
| **ឈ្មោះជាភាសាអង់គ្លេស** | **Group Capstone** | ឈ្មោះផ្លូវការនៃអង្គការ GitHub |
| **ការបញ្ចេញសំឡេង (IPA)** | `/ɡruːp ˈkæp.stoʊn/` | សំឡេងអន្តរជាតិ (International Phonetic Alphabet) |
| **អានជាភាសាខ្មែរ** | **គ្រុប ខេបស្ទូន** | `គ្រុប` (Group) + `ខេប-ស្ទូន` (Cap-stone) |
| **អត្ថន័យជាភាសាខ្មែរ** | **ក្រុមសារណាបញ្ចប់ការសិក្សា** | ក្រុមនិស្សិតដែលរួមគ្នាសិក្សាស្រាវជ្រាវ និងកសាងប្រព័ន្ធជាក់ស្តែងដើម្បីបញ្ចប់ថ្នាក់ឧត្តមសិក្សា |
| **អត្ថន័យជាភាសាអង់គ្លេស** | **Culminating Dissertation Team** | The final crowning project demonstrating complete engineering and architectural competence |

> **ចំណាំសំឡេង (Pronunciation Tip)**: ពាក្យ **Cap** អានដូចមួកកាតឹប (Cap) ហើយពាក្យ **Stone** អានដូចដុំថ្ម (Stone)។

---

## ព័ត៌មានទូទៅអំពីគម្រោង (Project Overview)

អង្គការ **Group Capstone** បង្កើតឡើងដើម្បីគ្រប់គ្រងកូដប្រភព ឯកសារស្ថាបត្យកម្ម និងដំណើរការអភិវឌ្ឍប្រព័ន្ធគ្រប់គ្រងសាលារៀន **SNP-SMS (SNPI School Management System)** ដែលជាប្រព័ន្ធកម្រិតសហគ្រាសសម្រាប់គ្រឹះស្ថានអប់រំនៅកម្ពុជា។

- **ស្ថានភាព (Status)**: កំពុងអភិវឌ្ឍន៍ និងផ្ទៀងផ្ទាត់គុណភាពកម្រិតខ្ពស់ (Active Development & Verification)
- **គេហទំព័រតេស្តប្រព័ន្ធ (Testing Domain)**: [snpis.kesararamwithdigital.tech](https://snpis.kesararamwithdigital.tech)
- **វិបផតថលឯកសារ & រចនាបថ (Design Portal)**: [snpis.kesararamwithdigital.tech/document/design](https://snpis.kesararamwithdigital.tech/document/design)
- **ទីតាំង (Location)**: កម្ពុជា (Cambodia)
- **ក្រុមការងារ (Team)**: ក្រុមស្រាវជ្រាវសារណា (`@GroupCapstone/team-research-dissertation`)

---

## ស្ថាបត្យកម្មប្រព័ន្ធស្នូល (Core System Architecture)

ប្រព័ន្ធនេះត្រូវបានរៀបចំឡើងតាមទម្រង់ស្ថាបត្យកម្មបំបែកស្រទាប់ Hybrid រវាង Next.js Frontend និង 7-Layer Modular Monolith Backend API:

```
+-------------------------------------------------------------------------+
|                          ស្រទាប់អ្នកប្រើប្រាស់ (Client Tier)                |
|   Next.js 16 (App Router) - React 19 - Tailwind CSS - Radix UI         |
|   ផតថលរចនាបថ: https://snpis.kesararamwithdigital.tech/document/design  |
+-------------------------------------------------------------------------+
                                    |
                  Server-Side Proxy Rewrite (/api/v1/*)
                                    |
+-------------------------------------------------------------------------+
|                        ស្រទាប់សេវាកម្ម API (Backend Tier)               |
|   Express 5 - TypeScript - 7-Layer Modular Monolith Architecture       |
|   ចំនួនម៉ូឌុល: 47 Domain Modules - 193 REST API Endpoints              |
+-------------------------------------------------------------------------+
                                    |
+-------------------------------------------------------------------------+
|                         មូលដ្ឋានទិន្នន័យ (Persistence Tier)             |
|   MongoDB Replica Set (rs0) - ប្រតិបត្តិការ ACID Distributed Transaction|
+-------------------------------------------------------------------------+
```

---

## ឃ្លាំងផ្ទុកកូដគម្រោង (Repositories)

| ឈ្មោះ Repository | តួនាទីក្នុងប្រព័ន្ធ (Role) | បច្ចេកវិទ្យាស្នូល (Stack) |
| :--- | :--- | :--- |
| **`SNPI-Web`** | កម្មវិធីផ្ទៃមុខសម្រាប់អ្នកប្រើប្រាស់ (Frontend Web) | Next.js 16, React 19, TypeScript, Tailwind CSS, SWR |
| **`SNPI-API`** | សេវាកម្ម Backend និងគ្រប់គ្រងទិន្នន័យ (API Services) | Express 5, TypeScript, Mongoose, MongoDB Replica Set, Zod |
| **`.github`** | កម្រងព័ត៌មានអង្គការ និងស្តង់ដាររួម (Profile & Standards) | Organization Profile, PR/Issue Templates, Security Policies |

---

## គោលការណ៍វិស្វកម្ម និងសុវត្ថិភាព (Core Engineering Standards)

- **Zero-Bridge Architecture**: ការបំបែកផ្តាច់រវាង GitHub Version Control និង Vercel Production Hosting ដោយប្រើប្រាស់ CLI Workflow ផ្ទាល់។
- **7-Layer Modular Monolith**: ការរៀបចំហ្វាល់តាមលំដាប់លំដោយតឹងរ៉ឹង `route -> controller -> service -> repository -> model -> validation -> types`។
- **Multi-Tenant Data Scoping**: ការពារព្រំដែនទិន្នន័យតាមសាលា និងសាខា (`schoolId`, `branchId`) នៅគ្រប់សំណើទិន្នន័យទាំងអស់។
- **Zero-Emoji Policy**: ការអនុវត្តស្តង់ដារកូដកម្រិតវិជ្ជាជីវៈខ្ពស់ ដោយមិនប្រើប្រាស់រូបសញ្ញា emoji ក្នុងកូដ ឯកសារ ឬ commit message។

---

## សមាជិកក្រុមការងារ (Team & Governance)

- **អង្គការ (Organization)**: [Group Capstone](https://github.com/GroupCapstone)
- **សមាជិកដឹកនាំគម្រោង (Lead Contributors)**:
  - `shiliaiwei` (Full-Stack Architecture & Systems Engineering)
  - `Tan-Saphea` (Core Development & Systems Collaboration)
- **ក្រុមការងារផ្លូវការ (Team)**: `team-research-dissertation`
