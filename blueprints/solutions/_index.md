---
title: "Katalog řešení"
type: blueprint
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
owner: "Miroslav Tobolka"
tags: [solutions, catalog, blueprint]
domain: solutions
summary: "Katalog řešení a architektonických vzorů"
---

# Katalog řešení

## Přehled

Katalog ověřených řešení a architektonických vzorů, které používáme v projektech Sensio.cz.

## Softwarová řešení

### SaaS aplikace (iZUŠ vzor)

| Aspekt | Řešení |
|--------|--------|
| Architektura | Monolitická Laravel aplikace s Vue.js frontendem |
| Multi-tenancy | TODO (schema-based / row-based / instance-based) |
| Autentizace | TODO |
| Autorizace | TODO (role-based) |
| API | TODO (REST / GraphQL) |
| Databáze | PostgreSQL |
| Cache | TODO |
| Queue | TODO |
| Deployment | Docker |

### Webová aplikace na míru (B2B PRO vzor)

| Aspekt | Řešení |
|--------|--------|
| Architektura | Laravel + Vue.js (SPA nebo SSR) |
| Autentizace | TODO |
| API | REST API |
| Databáze | PostgreSQL |
| Deployment | Docker |
| Monitoring | TODO |

## Infrastrukturní řešení

### Hosting

| Aspekt | Řešení |
|--------|--------|
| Provider | TODO |
| Kontejnerizace | Docker |
| Orchestrace | TODO |
| CI/CD | TODO |
| Monitoring | TODO |
| Backup | TODO |

### Bezpečnost

| Aspekt | Řešení |
|--------|--------|
| SSL/TLS | TODO |
| WAF | TODO |
| DDoS ochrana | TODO |
| Penetrační testy | TODO |
| GDPR | TODO |

## Procesní řešení

| Proces | Řešení |
|--------|--------|
| Projektové řízení | TODO |
| Komunikace | TODO |
| Dokumentace | Git + Markdown (tento repozitář) |
| Fakturace | TODO |

## Jak přidat nové řešení

1. Vytvoř nový soubor v této složce
2. Použij frontmatter s `type: blueprint`
3. Popiš problém, řešení, alternativy a důvody
4. Přidej odkaz do tohoto indexu
