---
title: "Šablona: Architecture Decision Record"
type: template
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
tags: [template, adr, decision]
domain: meta
summary: "Šablona pro ADR (Architecture Decision Record)"
---

# Šablona: Architecture Decision Record (ADR)

## Použití

Tuto šablonu použijte pro zaznamenávání klíčových architektonických a strategických rozhodnutí. Soubory ukládejte do `strategy/decisions/` s názvem `adr-NNN-nazev.md`.

## Šablona

```markdown
---
title: "ADR-NNN: NÁZEV ROZHODNUTÍ"
type: decision
status: ai-generated
version: "0.1"
created: YYYY-MM-DD
updated: YYYY-MM-DD
owner: "JMÉNO VLASTNÍKA"
tags: [adr, DALŠÍ_TAGY]
domain: DOMÉNA
summary: "Stručný popis rozhodnutí"
---

# ADR-NNN: NÁZEV ROZHODNUTÍ

## Status

Navrhováno (proposed) | Přijato (accepted) | Zamítnuto (rejected) | Nahrazeno (superseded by ADR-XXX)

## Kontext

Jaký je kontext nebo problém, který vede k tomuto rozhodnutí?

## Zvažované alternativy

### Alternativa 1: NÁZEV
- **Pro**: ...
- **Proti**: ...

### Alternativa 2: NÁZEV
- **Pro**: ...
- **Proti**: ...

## Rozhodnutí

Co jsme se rozhodli udělat a proč.

## Důvody

Hlavní důvody pro toto rozhodnutí.

## Důsledky

### Pozitivní
- ...

### Negativní
- ...

## Související rozhodnutí

- [ADR-XXX](adr-XXX-nazev.md) — popis vztahu
```

## Checklist

- [ ] Číslo ADR je unikátní a následuje sekvenci
- [ ] Kontext jasně popisuje problém
- [ ] Jsou uvedeny alespoň 2 alternativy
- [ ] Rozhodnutí je jasně formulováno
- [ ] Důsledky jsou realistické
