---
title: "Vývojový proces"
type: process
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
owner: "Miroslav Tobolka"
tags: [development, git, code-review, ci-cd, testing]
domain: development
summary: "Vývojový proces — git flow, code review, CI/CD, testing"
---

# Vývojový proces

## Tech stack

Detaily viz [tech-stack.md](../../reference/tech-stack.md).

- **Backend**: PHP / Laravel
- **Frontend**: Vue.js
- **Databáze**: PostgreSQL
- **Infrastruktura**: Docker
- **Verzování**: GitHub

## Git Flow

### Strategie větví

```
main ─────────────────────────────────────────────► (produkce)
  │
  ├── develop ────────────────────────────────────► (staging)
  │     │
  │     ├── feature/nazev-funkce ──► merge do develop
  │     ├── feature/dalsi-funkce ──► merge do develop
  │     │
  │     ├── bugfix/nazev-bugu ─────► merge do develop
  │     │
  │     └── release/v1.2.0 ────────► merge do main + develop
  │
  └── hotfix/kriticka-oprava ──────► merge do main + develop
```

### Konvence pojmenování větví
| Typ | Formát | Příklad |
|-----|--------|---------|
| Feature | `feature/popis` | `feature/student-export` |
| Bugfix | `bugfix/popis` | `bugfix/login-error` |
| Hotfix | `hotfix/popis` | `hotfix/payment-crash` |
| Release | `release/vX.Y.Z` | `release/v2.1.0` |

### Commit messages
- Jazyk: čeština
- Formát: stručný popis změny
- Příklad: `Přidání exportu žáků do CSV`
- Příklad: `Oprava chyby při přihlašování`

## Code Review

### Proces
1. Vývojář vytvoří Pull Request na GitHubu
2. Vyplní [PR šablonu](../../.github/pull_request_template.md)
3. Reviewer zkontroluje kód
4. Diskuze a opravy
5. Schválení a merge

### Co kontrolujeme
- [ ] Funkcionalita — dělá to, co má?
- [ ] Čitelnost — je kód srozumitelný?
- [ ] Testovatelnost — jsou testy?
- [ ] Bezpečnost — žádné zranitelnosti?
- [ ] Výkon — žádné performance problémy?
- [ ] Konvence — dodrženy coding standardy?

### Pravidla
- Každý PR musí mít alespoň 1 review
- Autor nemůže schválit vlastní PR
- TODO — další pravidla

## CI/CD

### Pipeline

```
Push → Lint → Test → Build → Deploy (staging) → Deploy (production)
```

### Detaily
| Krok | Nástroj | Popis |
|------|---------|-------|
| Lint | TODO | Kontrola stylu kódu |
| Test | TODO | Automatické testy |
| Build | Docker | Sestavení aplikace |
| Deploy staging | TODO | Nasazení na staging |
| Deploy production | TODO | Nasazení do produkce |

## Testing

### Typy testů
| Typ | Popis | Nástroj |
|-----|-------|---------|
| Unit testy | Testování jednotlivých funkcí | PHPUnit |
| Feature testy | Testování celých funkcí | Laravel Tests |
| Frontend testy | Testování Vue komponent | TODO |
| E2E testy | Testování celých scénářů | TODO |

### Pokrytí
- Cíl: TODO % code coverage
- Aktuální: TODO %

## Prostředí

| Prostředí | Účel | URL |
|-----------|------|-----|
| Local | Vývoj | localhost |
| Staging | Testování | TODO |
| Production | Ostrý provoz | TODO |

## Nástroje

| Nástroj | Účel |
|---------|------|
| GitHub | Verzování, PR, issues |
| Docker | Kontejnerizace |
| TODO | Projektové řízení |
| TODO | Monitoring |
| TODO | Logování |
