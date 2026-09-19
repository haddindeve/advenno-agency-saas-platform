# Advenno - Agency Platform with Client and Employee Portals

> Marketing site, JSON API and admin, client and employee portals for a software agency, on PHP 8 and MySQL.

Built by **[Muhammad Tanveer](https://www.linkedin.com/in/muhammad-tanveer-advenno/)** - Full-Stack AI Automation Engineer.

[![Source](https://img.shields.io/badge/source-private%20repository-lightgrey)](#source-code-and-access) [![Role](https://img.shields.io/badge/built%20by-Muhammad%20Tanveer-blue)](https://github.com/haddindeve)

## Contents

- [The problem](#the-problem)
- [The approach](#the-approach)
- [Architecture](#architecture)
- [Tech stack](#tech-stack)
- [Key capabilities](#key-capabilities)
- [Results](#results)
- [FAQ](#faq)
- [Source code and access](#source-code-and-access)
- [About the engineer](#about-the-engineer)
- [Related projects](#related-projects)

## The problem

A software agency ran its public site, client communication, employee management and invoicing as separate tools. Clients had no single place to see project status or invoices, and staff records lived outside any system tied to the work being delivered.

## The approach

One PHP 8 codebase serving a server-rendered marketing site alongside a JSON API backend with three role-scoped portals. Sessions secure the portals, JWT secures the API, and a PDO layer fails soft so a database issue degrades a page rather than the whole site. No build step, which keeps deployment on shared hosting reliable.

## Architecture

| Component | Responsibility |
| --- | --- |
| **Marketing site** | 50+ server-rendered pages with shared PHP includes |
| **backend-php API** | JSON endpoints secured with JWT |
| **Portals** | Separate admin, client and employee surfaces |
| **Scheduled jobs** | Cron-driven email queue and cache maintenance |
| **Data layer** | PDO singleton with fail-soft behaviour |

## Tech stack

| Layer | Technology |
| --- | --- |
| Backend | PHP 8.3 |
| Database | MySQL via PDO |
| Auth | JWT for API, sessions for portals |
| Frontend | Vanilla JavaScript and CSS, no framework |
| Ops | Cron workers, page cache |

## Key capabilities

- Role-scoped admin, client and employee portals
- JWT-secured JSON API
- Invoice generation and download
- Email queue drained by cron
- Page caching for the marketing site
- Google Search Console integration utilities

## Results

- Public site, client delivery and internal administration unified in one deployable codebase
- No build toolchain, so deployment stays viable on standard PHP hosting
- Database failures degrade gracefully instead of taking pages down

## FAQ

### Why no JavaScript framework?

The site is content-heavy and SEO-critical. Server-rendered PHP with vanilla JS gives fast first paint and removes an entire build and hydration layer.

### How are the three portals separated?

Each has its own session scope and route namespace; the shared API enforces role checks independently of the UI.

### What secures the API?

JWT bearer tokens, distinct from the session cookies used by the portals.

### Can I review the code?

It is private - client data is involved. Access can be discussed.

## Source code and access

This repository is the public case study for **Advenno - Agency Platform with Client and Employee Portals**. The full implementation - application code, database schema, tests and deployment configuration - lives in a **private repository** on this account, alongside the rest of the work shown here.

Source access can be arranged for hiring conversations, technical review or client due diligence. The quickest route is a short message on [LinkedIn](https://www.linkedin.com/in/muhammad-tanveer-advenno/) or an email to [mtanveertahir6666@gmail.com](mailto:mtanveertahir6666@gmail.com).

## About the engineer

**Muhammad Tanveer - Full-Stack AI Automation Engineer**

Full-stack AI automation engineer. I build agentic systems, browser and workflow automation, RAG pipelines and the production web platforms they run on - from Rust and Python services to Next.js dashboards and PHP/MySQL business systems.

- GitHub: [haddindeve](https://github.com/haddindeve)
- LinkedIn: [Muhammad Tanveer](https://www.linkedin.com/in/muhammad-tanveer-advenno/)
- Email: [mtanveertahir6666@gmail.com](mailto:mtanveertahir6666@gmail.com)
- Location: Pakistan

## Related projects

- [AI Lab Support and Campus Routing Assistant](https://github.com/haddindeve/ai-lab-support-campus-routing)
- [ARMenu - Augmented Reality Restaurant Menu SaaS](https://github.com/haddindeve/armenu-augmented-reality-menu-saas)
- [VideoFactory - Automated AI Video Generation](https://github.com/haddindeve/videofactory-ai-video-generator)
- [Doctern - AI Document OCR and Table Extraction](https://github.com/haddindeve/doctern-document-ocr-ai)
- [Tahir Collection - Stockinette Manufacturer Web Platform](https://github.com/haddindeve/tahir-collection-stockinette-manufacturer)
- [Business OS - AI-Native Multi-Branch ERP](https://github.com/haddindeve/business-os-multi-branch-erp)

---

<sub>Advenno - Agency Platform with Client and Employee Portals - case study by Muhammad Tanveer - Full-Stack AI Automation Engineer. Keywords: agency management platform, client portal, employee portal, PHP 8 SaaS, JWT API, invoice management system.</sub>