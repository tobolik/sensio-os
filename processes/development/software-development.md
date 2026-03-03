---
title: "Vyvojovy proces"
type: process
status: ai-generated
version: "0.1"
created: 2026-03-03
updated: 2026-03-03
owner: "Miroslav Tobolka"
tags: [development, git, code-review, ci-cd, testing]
domain: development
summary: "Vyvojovy proces — git flow, code review, CI/CD, testing"
---

# Vyvojovy proces

## Tech stack

Detaily viz [tech-stack.md](../../reference/tech-stack.md).

- **Backend**: PHP / Laravel
- **Frontend**: Vue.js
- **Databaze**: PostgreSQL
- **Infrastruktura**: Docker
- **Verzovani**: GitHub

## Git Flow

### Vetev strategie

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

### Konvence pojmenovani vetvi
| Typ | Format | Priklad |
|-----|--------|---------|
| Feature | `feature/popis` | `feature/student-export` |
| Bugfix | `bugfix/popis` | `bugfix/login-error` |
| Hotfix | `hotfix/popis` | `hotfix/payment-crash` |
| Release | `release/vX.Y.Z` | `release/v2.1.0` |

### Commit messages
- Jazyk: cestina
- Format: strucny popis zmeny
- Priklad: `Pridani exportu zaku do CSV`
- Priklad: `Oprava chyby pri prihlasovani`

## Code Review

### Proces
1. Vyvojar vytvori Pull Request na GitHubu
2. Vyplni [PR sablonu](../../.github/pull_request_template.md)
3. Reviewer zkontroluje kod
4. Diskuze a opravy
5. Schvaleni a merge

### Co kontrolujeme
- [ ] Funkcionalita — dela to, co ma?
- [ ] Citelnost — je kod srozumitelny?
- [ ] Testovatelnost — jsou testy?
- [ ] Bezpecnost — zadne zranitelnosti?
- [ ] Výkon — zadne performance problemy?
- [ ] Konvence — dodrzeny coding standardy?

### Pravidla
- Kazdy PR musi mit alespon 1 review
- Autor nemuze schvalit vlastni PR
- TODO — dalsi pravidla

## CI/CD

### Pipeline

```
Push → Lint → Test → Build → Deploy (staging) → Deploy (production)
```

### Detaily
| Krok | Nastroj | Popis |
|------|---------|-------|
| Lint | TODO | Kontrola stylu kodu |
| Test | TODO | Automaticke testy |
| Build | Docker | Sestaveni aplikace |
| Deploy staging | TODO | Nasazeni na staging |
| Deploy production | TODO | Nasazeni do produkce |

## Testing

### Typy testu
| Typ | Popis | Nastroj |
|-----|-------|---------|
| Unit testy | Testovani jednotlivych funkci | PHPUnit |
| Feature testy | Testovani celych funkci | Laravel Tests |
| Frontend testy | Testovani Vue komponent | TODO |
| E2E testy | Testovani celych scenaru | TODO |

### Pokryti
- Cil: TODO % code coverage
- Aktualni: TODO %

## Prostredi

| Prostredi | Ucel | URL |
|-----------|------|-----|
| Local | Vyvoj | localhost |
| Staging | Testovani | TODO |
| Production | Ostry provoz | TODO |

## Nastroje

| Nastroj | Ucel |
|---------|------|
| GitHub | Verzovani, PR, issues |
| Docker | Kontejnerizace |
| TODO | Projektove rizeni |
| TODO | Monitoring |
| TODO | Logovani |
