---
title: "Hodnoticí kritéria"
type: reference
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
owner: "Miroslav Tobolka"
tags: [evaluation, criteria, decision-making]
domain: strategy
summary: "Hodnoticí kritéria pro produkty, partnery, nástroje a rozhodování"
---

# Hodnoticí kritéria

## Hodnocení produktů / funkcí

Používáme pro rozhodování o prioritizaci funkcí a produktových rozhodnutí.

| Kritérium | Váha | Popis |
|-----------|------|-------|
| Hodnota pro zákazníka | 30% | Jak moc funkce řeší skutečný problém zákazníků? |
| Strategický soulad | 20% | Je v souladu s naší vizí a strategií? |
| Náročnost implementace | 20% | Kolik času a zdrojů to vyžaduje? |
| Revenue potenciál | 15% | Jaký je přímý nebo nepřímý dopad na příjem? |
| Technický dluh | 15% | Přidává nebo snižuje technický dluh? |

### Bodování
- 5 = Vynikající
- 4 = Dobré
- 3 = Průměrné
- 2 = Podprůměrné
- 1 = Nevyhovující

### Minimální skóre pro schválení: TODO

## Hodnocení partnerů / dodavatelů

| Kritérium | Váha | Popis |
|-----------|------|-------|
| Odbornost | 25% | Prokázané zkušenosti v relevantní oblasti |
| Spolehlivost | 25% | Dodržování termínů a kvality |
| Cenová přiměřenost | 20% | Hodnota za peníze |
| Kulturní fit | 15% | Soulad s našimi hodnotami a způsobem práce |
| Reference | 15% | Ověřitelné reference a portfolio |

## Hodnocení nástrojů / technologií

| Kritérium | Váha | Popis |
|-----------|------|-------|
| Funkcionalita | 25% | Pokrývá naše potřeby? |
| Integrace | 20% | Jak dobře se integruje s naším stackem? |
| Cena | 20% | TCO (Total Cost of Ownership) |
| Komunita a podpora | 15% | Aktivní komunita, dokumentace, podpora |
| Bezpečnost | 10% | Bezpečnostní standardy a certifikace |
| Škálovatelnost | 10% | Zvládne růst našich potřeb? |

## Hodnocení projektů (go/no-go)

Pro rozhodnutí, zda přijmout B2B projekt:

| Kritérium | Váha | Popis |
|-----------|------|-------|
| Strategický soulad | 20% | Odpovídá naší strategii a hodnotám? |
| Kapacita týmu | 20% | Máme lidi a čas? |
| Technická proveditelnost | 20% | Umíme to technicky zvládnout? |
| Finanční atraktivita | 20% | Je to finančně zajímavé? |
| Referenční potenciál | 10% | Může se stát referenčním projektem? |
| Dlouhodobý potenciál | 10% | Je příležitost pro dlouhodobou spolupráci? |

### Go/No-Go práh
- **Go**: Vážený průměr >= 3.5
- **Podmíněný Go**: Vážený průměr 2.5-3.5 (vyžaduje souhlas jednatele)
- **No-Go**: Vážený průměr < 2.5

## Proces hodnocení

1. **Sběr dat** — shromáždit relevantní informace
2. **Bodování** — každý hodnotitel oboduje nezávisle
3. **Diskuze** — probrat rozpory v hodnocení
4. **Rozhodnutí** — finální rozhodnutí na základě váženého průměru
5. **Dokumentace** — zaznamenat rozhodnutí a důvody (viz [ADR šablona](../../templates/_meta/adr-template.md))
