---
title: "Konvence a pravidla obsahu"
type: reference
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
owner: "Miroslav Tobolka"
tags: [conventions, meta, rules]
domain: documentation
summary: "Pravidla pro tvorbu a strukturu obsahu v Business OS"
---

# Konvence a pravidla obsahu

## Frontmatter Schema

Každý soubor (kromě README.md) musí obsahovat YAML frontmatter s následujícími poli.

### Povinná pole

| Pole | Typ | Popis |
|------|-----|-------|
| `title` | string | Název dokumentu |
| `type` | enum | Typ dokumentu (viz níže) |
| `status` | enum | Status dokumentu (viz níže) |
| `version` | string | Verze ve formátu `Epoch.Revision` |
| `created` | date | Datum vytvoření (YYYY-MM-DD) |
| `updated` | date | Datum poslední aktualizace (YYYY-MM-DD) |

### Volitelná pole

| Pole | Typ | Popis |
|------|-----|-------|
| `owner` | string | Vlastník dokumentu |
| `tags` | list | Štítky pro kategorizaci |
| `domain` | string | Doména (sales, delivery, development, ...) |
| `summary` | string | Stručný popis obsahu |

### Příklad

```yaml
---
title: "Název dokumentu"
type: knowledge
status: draft
version: "1.0"
created: 2026-03-03
updated: 2026-03-03
owner: "Miroslav Tobolka"
tags: [tag1, tag2]
domain: sales
summary: "Stručný popis"
---
```

## Typy dokumentů (type)

| Typ | Popis | Typické umístění |
|-----|-------|-----------------|
| `persona` | Persona AI agenta | `agents/personas/` |
| `prompt` | System prompt pro AI | `agents/prompts/` |
| `workflow` | Popis workflow/procesu | `processes/` |
| `tool` | Popis nástroje | `agents/tools/` |
| `knowledge` | Znalostní článek | `context/` |
| `process` | Firemní proces | `processes/` |
| `blueprint` | Architektonický plán | `blueprints/` |
| `template` | Šablona dokumentu | `templates/` |
| `strategy` | Strategický dokument | `strategy/` |
| `decision` | Rozhodovací záznam (ADR) | `strategy/decisions/` |
| `reference` | Referenční materiál | `reference/` |

## Statusy dokumentů (status)

| Status | Popis | Kdo může nastavit |
|--------|-------|-------------------|
| `ai-generated` | Vygenerováno AI, čeká na review | AI agent |
| `draft` | Rozpracovaný dokument | Kdokoli |
| `review` | Čeká na schválení | Autor |
| `approved` | Schváleno a platné | Pouze člověk (vlastník) |
| `archived` | Archivováno, již neplatné | Vlastník |

### Přechodový diagram

```
ai-generated → draft → review → approved → archived
                 ↑        ↓
                 └────────┘ (vráceno k přepracování)
```

## Verzování

Používáme formát **Epoch.Revision**:

- **Epoch** (celé číslo): Zvyšuje se při zásadní koncepční změně dokumentu
- **Revision** (celé číslo): Zvyšuje se při každé úpravě obsahu v rámci stejné koncepce

### Příklady

| Verze | Význam |
|-------|--------|
| `0.1` | První AI-generovaná verze |
| `0.2` | Úprava po review |
| `1.0` | První schválená verze |
| `1.1` | Drobná úprava schválené verze |
| `2.0` | Zásadní přepracování konceptu |

## Pravidla pojmenování souborů

- Používat **kebab-case** (malá písmena, slova oddělená pomlčkou)
- Pouze ASCII znaky (bez diakritiky)
- Přípona `.md` pro všechny dokumenty
- Příklady: `discovery-framework.md`, `ideal-client-profile.md`, `adr-001-repo-structure.md`
- ADR soubory: `adr-NNN-nazev.md` (třímístné číslo)

## Pravidla pro obsah

- **Jazyk obsahu**: čeština
- **Jazyk YAML klíčů**: angličtina
- **Uvozovky v YAML**: nikdy české uvozovky (`„"` nebo `‚'`), vždy standardní (`"` nebo `'`)
- **Interní odkazy**: vždy relativní markdown linky (např. `[text](../company/about.md)`)
- **Neznámá data**: označit slovem `TODO`
- **Emoji**: nepoužívat, pokud to není výslovně požadováno
