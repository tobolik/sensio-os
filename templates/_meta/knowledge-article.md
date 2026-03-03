---
title: "Sablona: Znalostni clanek"
type: template
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
tags: [template, knowledge, article]
domain: meta
summary: "Sablona pro vytvoreni znalostniho clanku v Business OS"
---

# Sablona: Znalostni clanek

## Pouziti

Tuto sablonu pouzijte pro vytvareni novych znalostních clanku v adresari `context/`.

## Sablona

```markdown
---
title: "NAZEV CLANKU"
type: knowledge
status: ai-generated
version: "0.1"
created: YYYY-MM-DD
updated: YYYY-MM-DD
owner: "JMENO VLASTNIKA"
tags: [tag1, tag2]
domain: DOMENA
summary: "Strucny popis obsahu"
---

# NAZEV CLANKU

## Prehled

Strucny uvod — o cem clanek je a proc je dulezity.

## Obsah

### Sekce 1

Obsah sekce...

### Sekce 2

Obsah sekce...

## Souvisejici dokumenty

- [Odkaz na souvisejici dokument](relativni/cesta.md)

## Zmeny

| Datum | Verze | Popis zmeny |
|-------|-------|-------------|
| YYYY-MM-DD | 0.1 | Prvni verze |
```

## Checklist pred publikaci

- [ ] Frontmatter je kompletni a validni
- [ ] Typ je spravny (`knowledge`)
- [ ] Obsah je v cestine
- [ ] Vsechny odkazy jsou relativni
- [ ] Neznama data oznacena TODO
- [ ] Soubor je pojmenovan v kebab-case
