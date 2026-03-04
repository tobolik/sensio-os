---
title: "Proces dodávky projektu"
type: process
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
owner: "Miroslav Tobolka"
tags: [delivery, project, process, development]
domain: delivery
summary: "Proces dodávky projektu od kickoffu po předání"
---

# Proces dodávky projektu

## Přehled

Strukturovaný proces pro dodávku softwarových projektů (převážně B2B PRO, ale aplikovatelný i na interní projekty).

## Fáze projektu

### 1. Kickoff

**Cíl**: Sladit očekávání a nastavit spolupráci.

**Aktivity**:
- Kickoff meeting s klientem ([šablona](../../templates/delivery/project-kickoff.md))
- Definice cílů a kritérií úspěchu
- Nastavení komunikačních kanálů
- Určení kontaktních osob na obou stranách
- Nastavení přístupů do nástrojů

**Výstup**: Zápis z kickoffu, projektový plán

### 2. Analýza a návrh

**Cíl**: Detailně pochopit požadavky a navrhnout řešení.

**Aktivity**:
- Sběr a analýza požadavků
- Tvorba wireframů / mockupů
- Technický návrh architektury
- Odsouhlasení s klientem

**Výstup**: Specifikace, wireframy, technický návrh

### 3. Vývoj

**Cíl**: Implementovat řešení dle specifikace.

**Aktivity**:
- Vývoj po sprintech / iteracích (TODO — délka sprintu)
- Pravidelné demo klientovi
- Code review a testování
- Průběžná komunikace o postupu

**Proces vývoje**: Viz [software-development.md](../development/software-development.md)

**Výstup**: Funkční software

### 4. Testování

**Cíl**: Ověřit kvalitu a funkcionalitu.

**Aktivity**:
- Interní testování (manuální + automatické)
- UAT (User Acceptance Testing) s klientem
- Oprava nalezených chyb
- Performance testování (pokud relevantní)

**Výstup**: Otestovaný software připravený k nasazení

### 5. Nasazení

**Cíl**: Dostat software do produkce.

**Aktivity**:
- Příprava produkčního prostředí
- Nasazení (deployment)
- Migrace dat (pokud relevantní)
- Smoke testing v produkci

**Výstup**: Software běžící v produkci

### 6. Předání a podpora

**Cíl**: Předat projekt klientovi a nastavit podporu.

**Aktivity**:
- Školení uživatelů
- Předání dokumentace
- Nastavení podpůrného režimu (SLA)
- Retrospektiva projektu

**Výstup**: Spokojený klient, dokumentace, SLA

## Komunikace během projektu

| Co | Frekvence | Formát | Účastníci |
|---|-----------|--------|-----------|
| Status update | Týdenní | Email/zpráva | PM + klient |
| Demo | Konec sprintu | Video/osobně | Tým + klient |
| Eskalace | Ad hoc | Hovor | Jednatel + klient |

## Řízení rizik

| Riziko | Prevence | Reakce |
|--------|----------|--------|
| Změna požadavků | Jasná specifikace, change request proces | Nacenění a odsouhlasení změny |
| Zpoždění | Buffer v harmonogramu, průběžný monitoring | Komunikace s klientem, reprioritizace |
| Technické problémy | Code review, testování, architektura | Eskalace v týmu, alternativní řešení |
