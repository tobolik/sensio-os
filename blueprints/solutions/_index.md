---
title: "Katalog reseni"
type: blueprint
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
owner: "Miroslav Tobolka"
tags: [solutions, catalog, blueprint]
domain: solutions
summary: "Katalog reseni a architektonickych vzoru"
---

# Katalog reseni

## Prehled

Katalog overených reseni a architektonickych vzoru, ktere pouzivame v projektech Sensio.cz.

## Softwarova reseni

### SaaS aplikace (iZUS vzor)

| Aspekt | Reseni |
|--------|--------|
| Architektura | Monoliticka Laravel aplikace s Vue.js frontendem |
| Multi-tenancy | TODO (schema-based / row-based / instance-based) |
| Autentizace | TODO |
| Autorizace | TODO (role-based) |
| API | TODO (REST / GraphQL) |
| Databaze | PostgreSQL |
| Cache | TODO |
| Queue | TODO |
| Deployment | Docker |

### Webova aplikace na miru (B2B PRO vzor)

| Aspekt | Reseni |
|--------|--------|
| Architektura | Laravel + Vue.js (SPA nebo SSR) |
| Autentizace | TODO |
| API | REST API |
| Databaze | PostgreSQL |
| Deployment | Docker |
| Monitoring | TODO |

## Infrastrukturni reseni

### Hosting

| Aspekt | Reseni |
|--------|--------|
| Provider | TODO |
| Kontejnerizace | Docker |
| Orchestrace | TODO |
| CI/CD | TODO |
| Monitoring | TODO |
| Backup | TODO |

### Bezpecnost

| Aspekt | Reseni |
|--------|--------|
| SSL/TLS | TODO |
| WAF | TODO |
| DDoS ochrana | TODO |
| Penetracni testy | TODO |
| GDPR | TODO |

## Procesni reseni

| Proces | Reseni |
|--------|--------|
| Projektove rizeni | TODO |
| Komunikace | TODO |
| Dokumentace | Git + Markdown (tento repozitar) |
| Fakturace | TODO |

## Jak pridat nove reseni

1. Vytvor novy soubor v teto slozce
2. Pouzij frontmatter s `type: blueprint`
3. Popis problem, reseni, alternativy a duvody
4. Pridej odkaz do tohoto indexu
