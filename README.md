# Sensio.cz Business OS

Operační systém firmy **Sensio.cz s.r.o.** — strukturovaná znalostní báze, procesy, šablony a AI agenti pro řízení a rozvoj firmy.

## O firmě

**Sensio.cz s.r.o.** je softwarová a technologická firma se sídlem v Přerově. Zaměřujeme se na tři oblasti:

1. **Software pro ZUŠ** — iZUŠ (informační systém, 250+ škol) a EOS ZUŠ (soutěžní systém)
2. **B2B řešení** — B2B PRO (webové aplikace a systémy na míru)
3. **3D tisk a inovace** — MyCello (3D tištěné violoncello) a 3D tiskové služby

## Struktura repozitáře

```
sensio-os/
├── CLAUDE.md                  # AI routing a pravidla
├── README.md                  # Tento soubor
├── docs/                      # Konvence, pravidla, identita
├── context/                   # Kontext firmy
│   ├── company/               # Profil firmy, hodnoty, tým
│   ├── products/              # Produkty a služby
│   ├── clients/               # Klientské profily
│   ├── market/                # Trh a konkurence
│   └── evaluation/            # Hodnoticí kritéria
├── strategy/                  # Vize, roadmapa, rozhodnutí
│   └── decisions/             # Architecture Decision Records
├── processes/                 # Firemní procesy
│   ├── sales/                 # Obchodní procesy
│   ├── delivery/              # Dodávka a onboarding
│   ├── development/           # Vývojové procesy
│   ├── operations/            # Provozní procesy
│   └── finance/               # Finanční procesy
├── templates/                 # Šablony dokumentů
│   ├── _meta/                 # Meta šablony
│   ├── sales/                 # Obchodní šablony
│   └── delivery/              # Dodávkové šablony
├── agents/                    # AI agenti
│   ├── personas/              # Persony agentů
│   ├── prompts/               # System prompts
│   └── tools/                 # Nástroje
├── blueprints/                # Blueprinty a architektury
│   ├── infrastructure/        # Infrastruktura
│   └── solutions/             # Katalog řešení
├── reference/                 # Referenční materiály
└── .github/                   # GitHub šablony
```

## Jak začít

1. **Pochop firmu**: Začni s [context/company/about.md](context/company/about.md) a [context/company/values.md](context/company/values.md)
2. **Prostuduj konvence**: Přečti [docs/conventions.md](docs/conventions.md) pro pravidla tvorby obsahu
3. **Naviguj efektivně**: Použij [CLAUDE.md](CLAUDE.md) jako rozcestník
4. **Přispívej**: Každý nový soubor musí mít YAML frontmatter dle konvencí

## Konvence

- Každý soubor (kromě README) má YAML frontmatter
- Jazyk obsahu: **čeština**
- Jazyk YAML klíčů: **angličtina**
- Interní odkazy: relativní markdown linky
- Verzování: `Epoch.Revision`
- Detaily viz [docs/conventions.md](docs/conventions.md)

## Licence

Interní dokument firmy Sensio.cz s.r.o. Neveřejné.
