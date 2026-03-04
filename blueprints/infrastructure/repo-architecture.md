---
title: "Architektura repozitáře Business OS"
type: blueprint
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
owner: "Miroslav Tobolka"
tags: [architecture, repository, blueprint]
domain: infrastructure
summary: "Architektura repozitáře Sensio.cz Business OS"
---

# Architektura repozitáře Business OS

## Účel repozitáře

Tento repozitář slouží jako **operační systém firmy** — centrální místo pro všechny znalosti, procesy, šablony a AI agenty firmy Sensio.cz.

## Design principy

1. **Flat and findable** — minimální zanoření, maximální přehlednost
2. **AI-first** — struktura optimalizovaná pro navigaci AI agenty (CLAUDE.md)
3. **Convention over configuration** — jasné konvence místo složitých konfiguračních nástrojů
4. **Single source of truth** — každá informace na jednom místě, referencovaná odjinud

## Adresářová struktura

```
sensio-os/
├── CLAUDE.md              # [META] AI routing tabulka
├── README.md              # [META] Přehled repozitáře
├── .gitignore             # [META] Ignorované soubory
│
├── docs/                  # [DOMÉNA: Dokumentace]
│   ├── conventions.md     #   Pravidla a konvence
│   └── SOUL.md            #   Identita AI agenta
│
├── context/               # [DOMÉNA: Kontext]
│   ├── company/           #   Firemní profil
│   ├── products/          #   Produkty a služby
│   ├── clients/           #   Klientské profily
│   ├── market/            #   Trh a konkurence
│   └── evaluation/        #   Hodnoticí kritéria
│
├── strategy/              # [DOMÉNA: Strategie]
│   ├── vision.md          #   Mise a vize
│   ├── roadmap.md         #   Roadmapa
│   ├── goals.md           #   Strategické cíle
│   └── decisions/         #   ADR záznamy
│
├── processes/             # [DOMÉNA: Procesy]
│   ├── sales/             #   Obchodní procesy
│   ├── delivery/          #   Dodávkové procesy
│   ├── development/       #   Vývojové procesy
│   ├── operations/        #   Provozní procesy
│   └── finance/           #   Finanční procesy
│
├── templates/             # [DOMÉNA: Šablony]
│   ├── _meta/             #   Meta šablony
│   ├── sales/             #   Obchodní šablony
│   └── delivery/          #   Dodávkové šablony
│
├── agents/                # [DOMÉNA: AI agenti]
│   ├── personas/          #   Persony agentů
│   ├── prompts/           #   System prompty
│   └── tools/             #   Nástroje
│
├── blueprints/            # [DOMÉNA: Blueprinty]
│   ├── infrastructure/    #   Infrastruktura
│   └── solutions/         #   Katalog řešení
│
├── reference/             # [DOMÉNA: Reference]
│   ├── glossary.md        #   Slovník pojmů
│   └── tech-stack.md      #   Tech stack
│
└── .github/               # [META] GitHub konfigurace
    └── pull_request_template.md
```

## Domény

| Doména | Adresář | Účel |
|--------|---------|------|
| Dokumentace | `docs/` | Pravidla, konvence, identita |
| Kontext | `context/` | Firemní znalosti a data |
| Strategie | `strategy/` | Vize, cíle, rozhodnutí |
| Procesy | `processes/` | Jak děláme věci |
| Šablony | `templates/` | Znovupoužitelné vzory |
| AI agenti | `agents/` | AI persony, prompty, nástroje |
| Blueprinty | `blueprints/` | Architektura a řešení |
| Reference | `reference/` | Slovníky a technické reference |

## Navigace

### Pro lidi
- Začni s [README.md](../../README.md)
- Pak viz [CLAUDE.md](../../CLAUDE.md) pro routing tabulku

### Pro AI agenty
- Začni s [CLAUDE.md](../../CLAUDE.md) — routing tabulka dle potřeb
- Viz [conventions.md](../../docs/conventions.md) — pravidla pro obsah
- Viz [SOUL.md](../../docs/SOUL.md) — identita a tón

## Rozšiřitelnost

Repozitář je navržený tak, aby mohl růst:
- Nové domény = nové adresáře na první úrovni
- Nové podoblasti = nové podadresáře s README.md
- Každý nový soubor musí respektovat konvence

## Související rozhodnutí

- [ADR-001: Proč Git+Markdown](../../strategy/decisions/adr-001-repo-structure.md)
