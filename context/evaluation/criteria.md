---
title: "Hodnotici kriteria"
type: reference
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
owner: "Miroslav Tobolka"
tags: [evaluation, criteria, decision-making]
domain: strategy
summary: "Hodnotici kriteria pro produkty, partnery, nastroje a rozhodovani"
---

# Hodnotici kriteria

## Hodnoceni produktu / funkci

Pouzivame pro rozhodovani o prioritizaci funkci a produktovych rozhodnuti.

| Kriterium | Vaha | Popis |
|-----------|------|-------|
| Hodnota pro zakaznika | 30% | Jak moc funkce resi skutecny problem zakazniku? |
| Strategicky soulad | 20% | Je v souladu s nasi vizi a strategii? |
| Narocnost implementace | 20% | Kolik casu a zdroju to vyzaduje? |
| Revenue potencial | 15% | Jaky je primy nebo neprimy dopad na prijem? |
| Technicky dluh | 15% | Pridava nebo snizuje technicky dluh? |

### Bodovani
- 5 = Vynikajici
- 4 = Dobre
- 3 = Prumerne
- 2 = Podprumerne
- 1 = Nevyhovujici

### Minimalni skore pro schvaleni: TODO

## Hodnoceni partneru / dodavatelu

| Kriterium | Vaha | Popis |
|-----------|------|-------|
| Odbornost | 25% | Prokazane zkusenosti v relevantni oblasti |
| Spolehlivost | 25% | Dodrzovani terminu a kvality |
| Cenova primerenist | 20% | Hodnota za penize |
| Kulturni fit | 15% | Soulad s nasimi hodnotami a zpusobem prace |
| Reference | 15% | Overitelne reference a portfolio |

## Hodnoceni nastroju / technologii

| Kriterium | Vaha | Popis |
|-----------|------|-------|
| Funkcionalita | 25% | Pokryva nase potreby? |
| Integrace | 20% | Jak dobre se integruje s nasim stackem? |
| Cena | 20% | TCO (Total Cost of Ownership) |
| Komunita a podpora | 15% | Aktivni komunita, dokumentace, podpora |
| Bezpecnost | 10% | Bezpecnostni standardy a certifikace |
| Skalovatelnost | 10% | Zvladne rust nasich potreb? |

## Hodnoceni projektu (go/no-go)

Pro rozhodnuti, zda prijmout B2B projekt:

| Kriterium | Vaha | Popis |
|-----------|------|-------|
| Strategicky soulad | 20% | Odpovida nasi strategii a hodnotam? |
| Kapacita tymu | 20% | Mame lidi a cas? |
| Technicka proveditelnost | 20% | Umime to technicky zvladnout? |
| Financni atraktivita | 20% | Je to financne zajimave? |
| Referenční potencial | 10% | Muze se stat referencnim projektem? |
| Dlouhodoby potencial | 10% | Je prilezitost pro dlouhodobou spolupraci? |

### Go/No-Go prah
- **Go**: Vazeny prumer >= 3.5
- **Podmieneny Go**: Vazeny prumer 2.5-3.5 (vyzaduje souhlas jednatele)
- **No-Go**: Vazeny prumer < 2.5

## Proces hodnoceni

1. **Sber dat** — shromazdit relevantni informace
2. **Bodovani** — kazdy hodnotitel oboduje nezavisle
3. **Diskuze** — probrat rozpory v hodnoceni
4. **Rozhodnuti** — finalni rozhodnuti na zaklade vyzeneho prumeru
5. **Dokumentace** — zaznamenat rozhodnuti a duvody (viz [ADR sablona](../../templates/_meta/adr-template.md))
