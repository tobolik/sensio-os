---
title: "Architektura repozitare Business OS"
type: blueprint
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
owner: "Miroslav Tobolka"
tags: [architecture, repository, blueprint]
domain: infrastructure
summary: "Architektura repozitare Sensio.cz Business OS"
---

# Architektura repozitare Business OS

## Uccel repozitare

Tento repozitar slouzi jako **operacni system firmy** — centralni misto pro vsechny znalosti, procesy, sablony a AI agenty firmy Sensio.cz.

## Design principy

1. **Flat and findable** — minimalni zanoreni, maximalni prehlednost
2. **AI-first** — struktura optimalizovana pro navigaci AI agenty (CLAUDE.md)
3. **Convention over configuration** — jasne konvence misto slozitych konfiguracnich nastroju
4. **Single source of truth** — kazda informace na jednom miste, referencovana odjinud

## Adresarova struktura

```
sensio-os/
├── CLAUDE.md              # [META] AI routing tabulka
├── README.md              # [META] Prehled repozitare
├── .gitignore             # [META] Ignorovane soubory
│
├── docs/                  # [DOMENA: Dokumentace]
│   ├── conventions.md     #   Pravidla a konvence
│   └── SOUL.md            #   Identita AI agenta
│
├── context/               # [DOMENA: Kontext]
│   ├── company/           #   Firemni profil
│   ├── products/          #   Produkty a sluzby
│   ├── clients/           #   Klientske profily
│   ├── market/            #   Trh a konkurence
│   └── evaluation/        #   Hodnoticí kriteria
│
├── strategy/              # [DOMENA: Strategie]
│   ├── vision.md          #   Mise a vize
│   ├── roadmap.md         #   Roadmapa
│   ├── goals.md           #   Strategicke cile
│   └── decisions/         #   ADR zaznamy
│
├── processes/             # [DOMENA: Procesy]
│   ├── sales/             #   Obchodni procesy
│   ├── delivery/          #   Dodavkove procesy
│   ├── development/       #   Vyvojove procesy
│   ├── operations/        #   Provozni procesy
│   └── finance/           #   Financni procesy
│
├── templates/             # [DOMENA: Sablony]
│   ├── _meta/             #   Meta sablony
│   ├── sales/             #   Obchodni sablony
│   └── delivery/          #   Dodavkove sablony
│
├── agents/                # [DOMENA: AI agenti]
│   ├── personas/          #   Persony agentu
│   ├── prompts/           #   System prompty
│   └── tools/             #   Nastroje
│
├── blueprints/            # [DOMENA: Blueprinty]
│   ├── infrastructure/    #   Infrastruktura
│   └── solutions/         #   Katalog reseni
│
├── reference/             # [DOMENA: Reference]
│   ├── glossary.md        #   Slovnik pojmu
│   └── tech-stack.md      #   Tech stack
│
└── .github/               # [META] GitHub konfigurace
    └── pull_request_template.md
```

## Domeny

| Domena | Adresar | Ucel |
|--------|---------|------|
| Dokumentace | `docs/` | Pravidla, konvence, identita |
| Kontext | `context/` | Firemni znalosti a data |
| Strategie | `strategy/` | Vize, cile, rozhodnuti |
| Procesy | `processes/` | Jak delame veci |
| Sablony | `templates/` | Znovupouzitelne vzory |
| AI agenti | `agents/` | AI persony, prompty, nastroje |
| Blueprinty | `blueprints/` | Architektura a reseni |
| Reference | `reference/` | Slovniky a technicke reference |

## Navigace

### Pro lidi
- Zacni s [README.md](../../README.md)
- Pak viz [CLAUDE.md](../../CLAUDE.md) pro routing tabulku

### Pro AI agenty
- Zacni s [CLAUDE.md](../../CLAUDE.md) — routing tabulka dle potreb
- Viz [conventions.md](../../docs/conventions.md) — pravidla pro obsah
- Viz [SOUL.md](../../docs/SOUL.md) — identita a ton

## Rozsiritelnost

Repozitar je navrzeny tak, aby mohl rust:
- Nove domeny = nove adresare na prvni urovni
- Nove podoblasti = nove podadresare s README.md
- Kazdy novy soubor musi respektovat konvence

## Souvisejici rozhodnuti

- [ADR-001: Proc Git+Markdown](../../strategy/decisions/adr-001-repo-structure.md)
