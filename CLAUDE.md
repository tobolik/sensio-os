# CLAUDE.md — Sensio.cz Business OS

## AI Routing Table

| I need to... | Go to |
|---|---|
| Pochopit firmu a její hodnoty | [context/company/about.md](context/company/about.md), [context/company/values.md](context/company/values.md) |
| Zjistit organizační strukturu | [context/company/organizational-structure.md](context/company/organizational-structure.md), [context/company/team.md](context/company/team.md) |
| Pochopit obchodní jednotky | [context/company/business-units.md](context/company/business-units.md) |
| Zjistit detaily produktu iZUŠ | [context/products/izus.md](context/products/izus.md) |
| Zjistit detaily EOS ZUŠ | [context/products/eos.md](context/products/eos.md) |
| Zjistit detaily B2B PRO | [context/products/b2b-pro.md](context/products/b2b-pro.md) |
| Zjistit detaily MyCello | [context/products/mycello.md](context/products/mycello.md) |
| Zjistit o 3D tisku | [context/products/3d-printing.md](context/products/3d-printing.md) |
| Vidět katalog služeb | [context/products/service-catalog.md](context/products/service-catalog.md) |
| Identifikovat ideálního klienta | [context/clients/ideal-client-profile.md](context/clients/ideal-client-profile.md) |
| Analyzovat konkurenci | [context/market/competitors.md](context/market/competitors.md) |
| Hodnotit produkt/partnera/nástroj | [context/evaluation/criteria.md](context/evaluation/criteria.md) |
| Pochopit vizi a strategii | [strategy/vision.md](strategy/vision.md) |
| Vidět roadmapu | [strategy/roadmap.md](strategy/roadmap.md) |
| Pochopit strategické cíle | [strategy/goals.md](strategy/goals.md) |
| Zjistit architektonická rozhodnutí | [strategy/decisions/](strategy/decisions/) |
| Provést discovery s klientem | [processes/sales/discovery-framework.md](processes/sales/discovery-framework.md) |
| Vytvořit nabídku | [processes/sales/proposal-creation.md](processes/sales/proposal-creation.md) |
| Onboardovat nového klienta | [processes/delivery/onboarding.md](processes/delivery/onboarding.md) |
| Řídit dodávku projektu | [processes/delivery/project-delivery.md](processes/delivery/project-delivery.md) |
| Vývoj software | [processes/development/software-development.md](processes/development/software-development.md) |
| Publikovat obsah | [processes/operations/content-publishing.md](processes/operations/content-publishing.md) |
| Fakturace | [processes/finance/invoicing.md](processes/finance/invoicing.md) |
| Najít šablonu nabídky | [templates/sales/proposal-template.md](templates/sales/proposal-template.md) |
| Najít šablonu kickoffu | [templates/delivery/project-kickoff.md](templates/delivery/project-kickoff.md) |
| Napsat znalostní článek | [templates/_meta/knowledge-article.md](templates/_meta/knowledge-article.md) |
| Napsat ADR | [templates/_meta/adr-template.md](templates/_meta/adr-template.md) |
| Jednat jako zákaznická podpora | [agents/personas/support-agent.md](agents/personas/support-agent.md), [agents/prompts/customer-support.md](agents/prompts/customer-support.md) |
| Jednat jako obchodník | [agents/personas/sales-agent.md](agents/personas/sales-agent.md) |
| Zjistit AI nástroje | [agents/tools/tool-inventory.md](agents/tools/tool-inventory.md) |
| Pochopit architekturu repozitáře | [blueprints/infrastructure/repo-architecture.md](blueprints/infrastructure/repo-architecture.md) |
| Najít řešení | [blueprints/solutions/_index.md](blueprints/solutions/_index.md) |
| Vyhledat pojem | [reference/glossary.md](reference/glossary.md) |
| Zjistit tech stack | [reference/tech-stack.md](reference/tech-stack.md) |
| Zjistit finanční model | [context/company/financial-model.md](context/company/financial-model.md) |
| Zjistit KPI | [context/company/kpis.md](context/company/kpis.md) |
| Kontaktní údaje firmy | [context/company/contacts.md](context/company/contacts.md) |

## Common Workflows

### Nový klient (discovery → nabídka → kickoff)
1. Identifikuj segment klienta → [context/clients/ideal-client-profile.md](context/clients/ideal-client-profile.md)
2. Proveď discovery → [processes/sales/discovery-framework.md](processes/sales/discovery-framework.md)
3. Vytvoř nabídku → [processes/sales/proposal-creation.md](processes/sales/proposal-creation.md) + [templates/sales/proposal-template.md](templates/sales/proposal-template.md)
4. Kickoff projektu → [templates/delivery/project-kickoff.md](templates/delivery/project-kickoff.md)
5. Onboarding → [processes/delivery/onboarding.md](processes/delivery/onboarding.md)

### Zákaznická podpora
1. Načti personu → [agents/personas/support-agent.md](agents/personas/support-agent.md)
2. Použij system prompt → [agents/prompts/customer-support.md](agents/prompts/customer-support.md)
3. Kontext produktu → [context/products/](context/products/)

### Dodávka projektu
1. Kickoff → [templates/delivery/project-kickoff.md](templates/delivery/project-kickoff.md)
2. Vývoj → [processes/development/software-development.md](processes/development/software-development.md)
3. Dodávka → [processes/delivery/project-delivery.md](processes/delivery/project-delivery.md)

## Key Files

| Soubor | Účel |
|---|---|
| `docs/conventions.md` | Konvence a pravidla pro obsah |
| `docs/SOUL.md` | Identita AI agenta |
| `context/company/about.md` | Kdo jsme |
| `strategy/vision.md` | Kam směřujeme |
| `reference/tech-stack.md` | Čím pracujeme |

## Content Rules

- **Jazyk obsahu**: čeština
- **Jazyk YAML klíčů**: angličtina
- **Frontmatter**: povinný pro všechny soubory kromě README.md (viz [docs/conventions.md](docs/conventions.md))
- **Interní odkazy**: vždy relativní markdown linky
- **Neznámá data**: označit `TODO`
- **YAML uvozovky**: nikdy české uvozovky, používat standardní `"` nebo `'`
- **Verzování**: formát `Epoch.Revision` (viz [docs/conventions.md](docs/conventions.md))

## Git Workflow Rules

- Každá změna přes Pull Request
- PR šablona v `.github/pull_request_template.md`
- Commit messages v češtině, stručné a výstižné
- Branch naming: `feature/popis`, `fix/popis`, `docs/popis`

## Collaboration Model

- **Vlastník repozitáře**: Miroslav Tobolka
- **AI agent**: pomáhá s tvorbou a údržbou obsahu dle [docs/SOUL.md](docs/SOUL.md)
- **Review proces**: AI generuje → člověk reviduje → schválení

## DO NOT

- **NEMĚŇ** frontmatter schema bez aktualizace [docs/conventions.md](docs/conventions.md)
- **NEVYTVÁŘEJ** soubory bez povinného frontmatter
- **NEPOUŽÍVEJ** absolutní odkazy místo relativních
- **NEMĚŇ** status na `approved` — to může udělat pouze člověk
- **NEODSTRAŇUJ** `TODO` značky bez doplnění skutečných dat
- **NEPIŠ** obsah v angličtině (kromě YAML klíčů a technických termínů)
- **NEPOUŽÍVEJ** české uvozovky v YAML frontmatter
- **NEGENERUJ** fiktivní data — raději označ `TODO`
