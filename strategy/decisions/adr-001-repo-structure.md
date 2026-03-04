---
title: "ADR-001: Git+Markdown místo Notion/Wiki"
type: decision
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
owner: "Miroslav Tobolka"
tags: [adr, architecture, tooling]
domain: infrastructure
summary: "Rozhodnutí použít Git repozitář s Markdown soubory jako základ Business OS"
---

# ADR-001: Git+Markdown místo Notion/Wiki

## Status

Navrhováno (proposed)

## Kontext

Potřebujeme centrální místo pro firemní znalosti, procesy, šablony a strategické dokumenty. Zvažovali jsme několik přístupů:

1. **Notion** — populární all-in-one workspace
2. **Confluence / Wiki** — tradiční firemní wiki
3. **Git repozitář + Markdown** — verzované soubory v Gitu
4. **Google Docs** — sdílené dokumenty

## Rozhodnutí

Používáme **Git repozitář s Markdown soubory** jako základ Business OS.

## Důvody

### Pro Git+Markdown

1. **Verzování** — kompletní historie změn, možnost vrátit se k jakékoliv verzi
2. **Review proces** — Pull Requesty umožňují strukturovaný review
3. **AI-ready** — Markdown soubory jsou ideální pro práci s AI agenty (CLAUDE.md)
4. **Developer-friendly** — tým už pracuje s Gitem denně
5. **Vlastnictví dat** — data jsou naše, žádná závislost na SaaS poskytovateli
6. **Offline přístup** — funguje bez připojení k internetu
7. **Automatizace** — možnost automatizovat validaci, generování a publikování
8. **Structured frontmatter** — YAML frontmatter umožňuje strojové zpracování

### Proti Notion

1. **Vendor lock-in** — data jsou v proprietárním formátu
2. **Omezený export** — ztrácíte formátování a strukturu
3. **Cena** — platí se za uživatele
4. **AI integrace** — omezené možnosti pro custom AI agenty
5. **Verzování** — omezená historie změn

### Proti Confluence

1. **Složitost** — overengineered pro malou firmu
2. **Cena** — vyšší náklady
3. **UX** — pomalý a neohrabaný editor

### Proti Google Docs

1. **Struktura** — těžké udržet konzistentní strukturu
2. **Verzování** — nepřehledné
3. **AI integrace** — omezené

## Důsledky

### Pozitivní
- Tým může využívat známý workflow (git add, commit, push, PR)
- AI agent může číst a upravovat soubory přímo
- Možnost automatizovat validaci frontmatteru
- Kompletní audit trail

### Negativní
- Vyžaduje základní znalost Gitu a Markdownu
- Méně vizuálně atraktivní než Notion
- Není tak přístupný pro netechnické členy týmu
- Chybí real-time spoluedirace

## Zmírňování rizik

- Vytvořit srozumitelné konvence ([conventions.md](../../docs/conventions.md))
- Poskytnout šablony pro běžné typy dokumentů
- Zvážit GitHub Pages pro publikování obsahu
- Poskytnout školení pro netechnické členy týmu
