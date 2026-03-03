---
title: "Fakturacni proces"
type: process
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
owner: "Miroslav Tobolka"
tags: [finance, invoicing, process]
domain: finance
summary: "Fakturacni proces pro vsechny produktove rady"
---

# Fakturacni proces

## Prehled

Fakturacni proces se lisi podle produktove rady. Kazda ma specificka pravidla a frekvenci.

## iZUS — SaaS fakturace

### Typ: Recurring (opakovana)

| Parametr | Hodnota |
|----------|---------|
| Frekvence | Mesicni / rocni (dle smlouvy) |
| Splatnost | TODO dni |
| Zpusob uhrady | Prevod na ucet |
| Automaticka fakturace | TODO (ano/ne) |
| Nastroj | TODO |

### Proces
1. **Generovani faktury** — automaticky na zacatku fakturacniho obdobi (TODO)
2. **Odeslani** — email s fakturou klientovi
3. **Sledovani** — kontrola uhrady
4. **Upominka** — po TODO dnech po splatnosti
5. **Eskalace** — po TODO dnech bez uhrady

## EOS ZUS — Fakturace licence

### Typ: Rocni licence

| Parametr | Hodnota |
|----------|---------|
| Frekvence | Rocni |
| Splatnost | TODO dni |
| Zpusob uhrady | Prevod na ucet |

### Proces
1. Vystaveni faktury pred zacatkem licencniho obdobi
2. Odeslani klientovi
3. Sledovani uhrady

## B2B PRO — Projektova fakturace

### Typ: Milestonova nebo mesicni

| Parametr | Hodnota |
|----------|---------|
| Model | Dle smlouvy (fixni milestony nebo T&M) |
| Splatnost | TODO dni |
| Zalohova faktura | Ano (TODO % z celkove ceny) |

### Proces — Fixni cena
1. **Zalohova faktura** — TODO % pred zahajenim
2. **Prubezne faktury** — po dokonceni milestonu
3. **Konecna faktura** — po predani a akceptaci

### Proces — Time & Material
1. **Mesicni faktura** — na zaklade reportu odpracovanych hodin
2. **Priloha** — detailni report hodin a cinnosti

## MyCello / 3D tisk — Produktova fakturace

### Typ: Jednorazova

| Parametr | Hodnota |
|----------|---------|
| Fakturace | Pri objednavce / po dodani |
| Splatnost | TODO dni |
| Zpusob uhrady | Prevod / TODO |

### Proces
1. Potvrzeni objednavky
2. Vystaveni faktury (proforma nebo ostra)
3. Uhrada
4. Dodani

## Nastroje

| Nastroj | Ucel |
|---------|------|
| TODO | Fakturacni system |
| TODO | Ucetni system |
| TODO | Banka |

## Ucetni uzavierka

- **Mesicni**: TODO
- **Rocni**: TODO
- **Externi ucetni**: TODO (ano/ne, kdo)
