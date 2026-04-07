# NL Product Skills

Dit is een verzameling Nederlandstalige product management skills voor AI-assistenten.

## Conventies

- Alle skills zijn geschreven in het Nederlands
- Engelse vaktermen worden gebruikt waar ze gangbaar zijn in de Nederlandse PM-praktijk (stakeholder, roadmap, sprint, backlog, moat, leverage, etc.)
- Nederlandse termen waar het natuurlijk klinkt (waardepropositie, doelgroep, concurrentieanalyse, aannames, etc.)
- Voorbeelden gebruiken Nederlandse bedrijfsnamen en marktcontext
- Elke skill volgt de Agent Skills open standaard (YAML frontmatter + markdown instructies)
- Skills zijn zelfstandig bruikbaar — geen onderlinge afhankelijkheden vereist
- Toon: professioneel, direct, geen wollig taalgebruik

## Kernprincipes

Skills moeten **diep** gaan. Liever langer, meer vragen stellen, meer doorvragen dan snel en oppervlakkig. Een skill is geen shortcut — het moet kwalitatief waardevol zijn.

Skills zijn **context-first**. Elke skill begint met Fase 0: scan eerst uploads, gedeelde mappen en workspace op relevante bestanden. Lees wat er is. Stel daarna alleen vragen over wat je nog mist. Als er wél context is, bevestig wat je ziet ("Ik zie [X], klopt dat?") — dat voelt als samenwerken. Als er geen context is, stel de volledige vragenlijst.

## Structuur

```
skills/
  skill-naam/
    SKILL.md          # Hoofdbestand met instructies
```

## Doorlopende frameworks

Sommige frameworks komen in meerdere skills terug:

- **FORCES Framework** (Product Faculty) — 6 krachten: Motivatie, Enablement, Momentum vs Wrijving, Angst, Inertie. Gebruikt in waardepropositie, klantinterview, go-to-market, pre-mortem
- **Seven Powers** (Hamilton Helmer) — 7 bronnen van verdedigbaar voordeel. Gebruikt in product-strategie, concurrentie-analyse, swot-analyse
- **Blue Ocean Strategy** — ERRC Grid, Six Paths, Noncustomers. Gebruikt in positionering

## Kwaliteitseisen

- Description in frontmatter: max 200 tekens, begint met werkwoord
- Elke skill begint met Fase 0: context checken, dan adaptief vragen stellen — nooit direct output genereren
- Duidelijke triggers zodat AI weet wanneer de skill te activeren
- Concrete voorbeelden, geen abstracte theorie
- Bronvermeldingen waar relevant
- AI-specifieke onderdelen zijn conditioneel: alleen tonen als relevant
