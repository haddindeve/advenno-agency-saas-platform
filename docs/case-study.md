# Advenno - Agency Platform with Client and Employee Portals - case study

**Engineer:** Muhammad Tanveer - Full-Stack AI Automation Engineer  
**Repository:** https://github.com/haddindeve/advenno-agency-saas-platform

## Context

A software agency ran its public site, client communication, employee management and invoicing as separate tools. Clients had no single place to see project status or invoices, and staff records lived outside any system tied to the work being delivered.

## What I built

One PHP 8 codebase serving a server-rendered marketing site alongside a JSON API backend with three role-scoped portals. Sessions secure the portals, JWT secures the API, and a PDO layer fails soft so a database issue degrades a page rather than the whole site. No build step, which keeps deployment on shared hosting reliable.

## Capabilities delivered

- Role-scoped admin, client and employee portals
- JWT-secured JSON API
- Invoice generation and download
- Email queue drained by cron
- Page caching for the marketing site
- Google Search Console integration utilities

## Outcome

- Public site, client delivery and internal administration unified in one deployable codebase
- No build toolchain, so deployment stays viable on standard PHP hosting
- Database failures degrade gracefully instead of taking pages down

## Source

The implementation is held in a private repository. Access can be arranged on request - [mtanveertahir66@gmail.com](mailto:mtanveertahir66@gmail.com) or [LinkedIn](https://www.linkedin.com/in/muhammad-tanveer-advenno/).