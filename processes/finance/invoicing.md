---
title: "Fakturační proces"
type: process
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
owner: "Miroslav Tobolka"
tags: [finance, invoicing, process]
domain: finance
summary: "Fakturační proces pro všechny produktové řady"
---

# Fakturační proces

## Přehled

Fakturační proces se liší podle produktové řady. Každá má specifická pravidla a frekvenci.

## iZUŠ — SaaS fakturace

### Typ: Recurring (opakovaná)

| Parametr | Hodnota |
|----------|---------|
| Frekvence | Měsíční / roční (dle smlouvy) |
| Splatnost | TODO dní |
| Způsob úhrady | Převod na účet |
| Automatická fakturace | TODO (ano/ne) |
| Nástroj | TODO |

### Proces
1. **Generování faktury** — automaticky na začátku fakturačního období (TODO)
2. **Odeslání** — email s fakturou klientovi
3. **Sledování** — kontrola úhrady
4. **Upomínka** — po TODO dnech po splatnosti
5. **Eskalace** — po TODO dnech bez úhrady

## EOS ZUŠ — Fakturace licence

### Typ: Roční licence

| Parametr | Hodnota |
|----------|---------|
| Frekvence | Roční |
| Splatnost | TODO dní |
| Způsob úhrady | Převod na účet |

### Proces
1. Vystavení faktury před začátkem licenčního období
2. Odeslání klientovi
3. Sledování úhrady

## B2B PRO — Projektová fakturace

### Typ: Milestoneová nebo měsíční

| Parametr | Hodnota |
|----------|---------|
| Model | Dle smlouvy (fixní milestony nebo T&M) |
| Splatnost | TODO dní |
| Zálohová faktura | Ano (TODO % z celkové ceny) |

### Proces — Fixní cena
1. **Zálohová faktura** — TODO % před zahájením
2. **Průběžné faktury** — po dokončení milestonu
3. **Konečná faktura** — po předání a akceptaci

### Proces — Time & Material
1. **Měsíční faktura** — na základě reportu odpracovaných hodin
2. **Příloha** — detailní report hodin a činností

## MyCello / 3D tisk — Produktová fakturace

### Typ: Jednorázová

| Parametr | Hodnota |
|----------|---------|
| Fakturace | Při objednávce / po dodání |
| Splatnost | TODO dní |
| Způsob úhrady | Převod / TODO |

### Proces
1. Potvrzení objednávky
2. Vystavení faktury (proforma nebo ostrá)
3. Úhrada
4. Dodání

## Nástroje

| Nástroj | Účel |
|---------|------|
| TODO | Fakturační systém |
| TODO | Účetní systém |
| TODO | Banka |

## Účetní uzávěrka

- **Měsíční**: TODO
- **Roční**: TODO
- **Externí účetní**: TODO (ano/ne, kdo)
