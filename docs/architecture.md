# Advenno - Agency Platform with Client and Employee Portals - architecture

One PHP 8 codebase serving a server-rendered marketing site alongside a JSON API backend with three role-scoped portals. Sessions secure the portals, JWT secures the API, and a PDO layer fails soft so a database issue degrades a page rather than the whole site. No build step, which keeps deployment on shared hosting reliable.

## Components

### Marketing site

50+ server-rendered pages with shared PHP includes

### backend-php API

JSON endpoints secured with JWT

### Portals

Separate admin, client and employee surfaces

### Scheduled jobs

Cron-driven email queue and cache maintenance

### Data layer

PDO singleton with fail-soft behaviour

## Stack

| Layer | Technology |
| --- | --- |
| Backend | PHP 8.3 |
| Database | MySQL via PDO |
| Auth | JWT for API, sessions for portals |
| Frontend | Vanilla JavaScript and CSS, no framework |
| Ops | Cron workers, page cache |

Designed and implemented by Muhammad Tanveer - Full-Stack AI Automation Engineer.