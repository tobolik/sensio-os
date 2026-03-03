---
title: "ADR-001: Git+Markdown misto Notion/Wiki"
type: decision
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
owner: "Miroslav Tobolka"
tags: [adr, architecture, tooling]
domain: infrastructure
summary: "Rozhodnuti pouzit Git repozitar s Markdown soubory jako zaklad Business OS"
---

# ADR-001: Git+Markdown misto Notion/Wiki

## Status

Navrhovano (proposed)

## Kontext

Potrebujeme centralni misto pro firemni znalosti, procesy, sablony a strategicke dokumenty. Zvazovali jsme nekolik pristupu:

1. **Notion** — popularni all-in-one workspace
2. **Confluence / Wiki** — tradicni firemni wiki
3. **Git repozitar + Markdown** — verzovane soubory v Gitu
4. **Google Docs** — sdilene dokumenty

## Rozhodnuti

Pouzivame **Git repozitar s Markdown soubory** jako zaklad Business OS.

## Duvody

### Pro Git+Markdown

1. **Verzovani** — kompletni historie zmien, moznost vratit se k jakékoliv verzi
2. **Review proces** — Pull Requesty umoznuji strukturovany review
3. **AI-ready** — Markdown soubory jsou idealni pro praci s AI agenty (CLAUDE.md)
4. **Developer-friendly** — tym uz pracuje s Gitem denne
5. **Vlastnictvi dat** — data jsou nase, zadna zavislost na SaaS poskytovateli
6. **Offline pristup** — funguje bez pripojeni k internetu
7. **Automatizace** — moznost automatizovat validaci, generovani a publikovani
8. **Structured frontmatter** — YAML frontmatter umoznuje strojove zpracovani

### Proti Notion

1. **Vendor lock-in** — data jsou v proprietarnim formatu
2. **Omezeny export** — ztracite formatovani a strukturu
3. **Cena** — plati se za uzivatele
4. **AI integrace** — omezene moznosti pro custom AI agenty
5. **Verzovani** — omezena historie zmen

### Proti Confluence

1. **Slozitost** — overengineered pro malou firmu
2. **Cena** — vyssi naklady
3. **UX** — pomaly a neohrabany editor

### Proti Google Docs

1. **Struktura** — tezke udrzet konzistentni strukturu
2. **Verzovani** — neprehledne
3. **AI integrace** — omezene

## Dusledky

### Pozitivní
- Tym muze vyuzivat znamy workflow (git add, commit, push, PR)
- AI agent muze cist a upravovat soubory primo
- Moznost automatizovat validaci frontmatteru
- Kompletní audit trail

### Negativni
- Vyzaduje zakladni znalost Gitu a Markdownu
- Mene vizualne atraktivni nez Notion
- Neni tak pristupny pro ne-technicke cleny tymu
- Chybi real-time spolueditace

## Zmirnovani rizik

- Vytvorit srozumitelne konvence ([conventions.md](../../docs/conventions.md))
- Poskytnout sablony pro bezne typy dokumentu
- Zvazit GitHub Pages pro publikovani obsahu
- Poskytnout skoleni pro ne-technicke cleny tymu
