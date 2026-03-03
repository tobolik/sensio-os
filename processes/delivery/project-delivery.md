---
title: "Proces dodavky projektu"
type: process
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
owner: "Miroslav Tobolka"
tags: [delivery, project, process, development]
domain: delivery
summary: "Proces dodavky projektu od kickoffu po predani"
---

# Proces dodavky projektu

## Prehled

Strukturovany proces pro dodavku softwarovych projektu (prevazne B2B PRO, ale aplikovatelny i na interni projekty).

## Faze projektu

### 1. Kickoff

**Cil**: Sladit ocekavani a nastavit spolupra|ci.

**Aktivity**:
- Kickoff meeting s klientem ([sablona](../../templates/delivery/project-kickoff.md))
- Definice cilů a kritérií uspechu
- Nastaveni komunikacnich kanalu
- Urceni kontaktnich osob na obou stranach
- Nastaveni pristupu do nastroju

**Vystup**: Zapis z kickoffu, projektovy plan

### 2. Analyza a navrh

**Cil**: Detailne pochopit pozadavky a navrhnout reseni.

**Aktivity**:
- Sber a analyza pozadavku
- Tvorba wireframu / mockupu
- Technicky navrh architektury
- Odsouhlaseni s klientem

**Vystup**: Specifikace, wireframy, technicky navrh

### 3. Vyvoj

**Cil**: Implementovat reseni dle specifikace.

**Aktivity**:
- Vyvoj po sprintech / iteracich (TODO — delka sprintu)
- Pravidelne demo klientovi
- Code review a testovani
- Prubezna komunikace o postupu

**Proces vyvoje**: Viz [software-development.md](../development/software-development.md)

**Vystup**: Funkcni software

### 4. Testovani

**Cil**: Overit kvalitu a funkcionalitu.

**Aktivity**:
- Interni testovani (manualni + automaticke)
- UAT (User Acceptance Testing) s klientem
- Oprava nalezenych chyb
- Performance testovani (pokud relevantni)

**Vystup**: Otestovany software pripraveny k nasazeni

### 5. Nasazeni

**Cil**: Dostat software do produkce.

**Aktivity**:
- Priprava produkčního prostredi
- Nasazeni (deployment)
- Migrace dat (pokud relevantni)
- Smoke testing v produkci

**Vystup**: Software bezici v produkci

### 6. Predani a podpora

**Cil**: Predat projekt klientovi a nastavit podporu.

**Aktivity**:
- Skoleni uzivatelu
- Predani dokumentace
- Nastaveni podpurneho rezimu (SLA)
- Retrospektiva projektu

**Vystup**: Spokojeny klient, dokumentace, SLA

## Komunikace behem projektu

| Co | Frekvence | Format | Ucastnici |
|---|-----------|--------|-----------|
| Status update | Tydenni | Email/zprava | PM + klient |
| Demo | Konec sprintu | Video/osobne | Tym + klient |
| Eskalace | Ad hoc | Hovor | Jednatel + klient |

## Rizeni rizik

| Riziko | Prevence | Reakce |
|--------|----------|--------|
| Zmena pozadavku | Jasna specifikace, change request proces | Nacenení a odsouhlaseni zmeny |
| Zpozdeni | Buffer v harmonogramu, prubezny monitoring | Komunikace s klientem, reprioritizace |
| Technicke problemy | Code review, testovani, architektura | Eskalace v tymu, alternativni reseni |
