---
title: "Sablona: Architecture Decision Record"
type: template
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
tags: [template, adr, decision]
domain: meta
summary: "Sablona pro ADR (Architecture Decision Record)"
---

# Sablona: Architecture Decision Record (ADR)

## Pouziti

Tuto sablonu pouzijte pro zaznamenavani klicovych architektonickych a strategickych rozhodnuti. Soubory ukladejte do `strategy/decisions/` s nazvem `adr-NNN-nazev.md`.

## Sablona

```markdown
---
title: "ADR-NNN: NAZEV ROZHODNUTI"
type: decision
status: ai-generated
version: "0.1"
created: YYYY-MM-DD
updated: YYYY-MM-DD
owner: "JMENO VLASTNIKA"
tags: [adr, DALSI_TAGY]
domain: DOMENA
summary: "Strucny popis rozhodnuti"
---

# ADR-NNN: NAZEV ROZHODNUTI

## Status

Navrhovano (proposed) | Prijato (accepted) | Zamitnuto (rejected) | Nahrazeno (superseded by ADR-XXX)

## Kontext

Jaky je kontext nebo problem, ktery vede k tomuto rozhodnuti?

## Zvazovane alternativy

### Alternativa 1: NAZEV
- **Pro**: ...
- **Proti**: ...

### Alternativa 2: NAZEV
- **Pro**: ...
- **Proti**: ...

## Rozhodnuti

Co jsme se rozhodli udelat a proc.

## Duvody

Hlavni duvody pro toto rozhodnuti.

## Dusledky

### Pozitivni
- ...

### Negativni
- ...

## Souvisejici rozhodnuti

- [ADR-XXX](adr-XXX-nazev.md) — popis vztahu
```

## Checklist

- [ ] Cislo ADR je unikatni a nasleduje sekvenci
- [ ] Kontext jasne popisuje problem
- [ ] Jsou uvedeny alespon 2 alternativy
- [ ] Rozhodnuti je jasne formulovano
- [ ] Dusledky jsou realisticke
