---
title: "Šablona: Znalostní článek"
type: template
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
tags: [template, knowledge, article]
domain: meta
summary: "Šablona pro vytvoření znalostního článku v Business OS"
---

# Šablona: Znalostní článek

## Použití

Tuto šablonu použijte pro vytváření nových znalostních článků v adresáři `context/`.

## Šablona

```markdown
---
title: "NÁZEV ČLÁNKU"
type: knowledge
status: ai-generated
version: "0.1"
created: YYYY-MM-DD
updated: YYYY-MM-DD
owner: "JMÉNO VLASTNÍKA"
tags: [tag1, tag2]
domain: DOMÉNA
summary: "Stručný popis obsahu"
---

# NÁZEV ČLÁNKU

## Přehled

Stručný úvod — o čem článek je a proč je důležitý.

## Obsah

### Sekce 1

Obsah sekce...

### Sekce 2

Obsah sekce...

## Související dokumenty

- [Odkaz na související dokument](relativní/cesta.md)

## Změny

| Datum | Verze | Popis změny |
|-------|-------|-------------|
| YYYY-MM-DD | 0.1 | První verze |
```

## Checklist před publikací

- [ ] Frontmatter je kompletní a validní
- [ ] Typ je správný (`knowledge`)
- [ ] Obsah je v češtině
- [ ] Všechny odkazy jsou relativní
- [ ] Neznámá data označena TODO
- [ ] Soubor je pojmenován v kebab-case
