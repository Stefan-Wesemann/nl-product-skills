---
name: metrics-dashboard
description: "Ontwerp een product metrics dashboard: welke KPI's, hoe visualiseren, welke alert-drempels. Het vervolg op je North Star Metric — van kiezen naar monitoren."
triggers:
  - metrics dashboard
  - kpi dashboard
  - dashboard ontwerpen
  - metrics monitoren
  - product dashboard
  - kpi overzicht
  - welke metrics
  - dashboard bouwen
  - metrics kiezen
---

# Metrics Dashboard

## Metadata

**Doel:** Ontwerp een dashboard dat je team helpt om de juiste beslissingen te nemen op basis van data — niet een dashboard dat er mooi uitziet maar niemand bekijkt.

**Relatie met North Star Metric:**
- **North Star Metric** (skill) = de juiste metric KIEZEN, inclusief sub-metrics en KPI-boom
- **Metrics Dashboard** (deze skill) = HOE je die metrics monitort: welke grafieken, alertdrempels, frequentie
- Eerst North Star, dan dashboard

**Aanpak:** Begin bij de vragen die je team dagelijks/wekelijks moet beantwoorden. Vertaal die naar metrics. Ontwerp de visualisatie die het snelst antwoord geeft.

**Output:** Dashboard-ontwerp met metrics, visualisatie-type per metric, alertdrempels en review-cadans.

---

## Instructies

### Fase 0: Context ophalen

**Stap 1 — Check wat er al is**
Scan uploads, gedeelde mappen en workspace op relevante bestanden (eerdere outputs, research, data). Lees ze door.

**Stap 2 — Slimme vragen stellen**
- **Wel context gevonden →** Bevestig kort wat je ziet ("Ik zie [X], klopt dat?"). Stel alleen vragen over wat je nog mist.
- **Geen context →** Stel onderstaande vragen.

1. **North Star**: Heb je al een North Star Metric en sub-metrics gedefinieerd? Zo ja, welke?
2. **Huidige situatie**: Heb je al een dashboard? Wat bevat het? Wat mist het?
3. **Publiek**: Wie bekijkt dit dashboard? (PM, engineering, C-level, iedereen?)
4. **Frequentie**: Hoe vaak kijken ze? (Real-time, dagelijks, wekelijks?)
5. **Vragen**: Welke vragen moet het dashboard beantwoorden? ("Gaat het goed?", "Waar moeten we ingrijpen?", "Wat is de trend?")
6. **Tooling**: Welke analytics-tools gebruik je? (Amplitude, Mixpanel, Google Analytics, Metabase, custom?)
7. **Data-volwassenheid**: Hoe volwassen is je data-infrastructuur? Heb je al event tracking, een data warehouse, of werk je nog met spreadsheets? Dit bepaalt wat realistisch is.
8. **Onderhoud**: Wie gaat dit dashboard onderhouden? Een dashboard zonder eigenaar wordt binnen een maand genegeerd.

---

## Stap 1: De Vragen Bepalen

Een goed dashboard beantwoordt specifieke vragen. Niet "alles laten zien", maar "deze 5 vragen in 30 seconden beantwoorden".

**De kernvragen voor een product-dashboard:**

| Vraag | Wat het je vertelt | Voorbeeld metric |
|---|---|---|
| Gaat het goed? | Algemene gezondheid | North Star Metric trend |
| Groeien we? | Acquisitie | Nieuwe gebruikers/week |
| Ervaren mensen waarde? | Activatie | % dat kernactie doet in sessie 1 |
| Komen ze terug? | Retentie | Week-1, Week-4 retentie |
| Verdienen we geld? | Monetisatie | MRR, conversie trial→betaald |
| Waar moeten we ingrijpen? | Problemen | Drop-off in funnel, error rates |

**Doorvragen:**
- "Welke vraag beantwoord je nu elke maandagochtend handmatig?"
- "Wanneer heb je voor het laatst een beslissing genomen op basis van data? Welke data was dat?"
- "Welke metric, als die ineens 50% daalt, wil je direct weten?"

---

## Stap 2: Metrics Selecteren

Kies 5-8 metrics voor je primaire dashboard. Meer = ruis. Minder = blinde vlekken.

### Structuur: de metriekpiramide

```
            [North Star Metric]
           /         |          \
    [Input Metric 1] [Input Metric 2] [Input Metric 3]
         |               |               |
    [Operationeel]  [Operationeel]  [Operationeel]
```

**Niveau 1: North Star (1 metric)**
- De ene metric die totale waardecreatie meet
- Altijd bovenaan het dashboard, altijd zichtbaar

**Niveau 2: Input Metrics (3-5 metrics)**
- De drivers die je North Star beïnvloeden
- Dit zijn de metrics waar je team dagelijks op stuurt
- Voorbeeld: als NSM = "wekelijks actieve teams", dan zijn inputs: nieuwe teams/week, activatie-%, retentie-%

**Niveau 3: Operationele metrics (optioneel, 2-3 metrics)**
- Metrics die problemen signaleren maar geen directe KPI zijn
- Voorbeeld: error rate, page load time, support ticket volume

### Per metric definiëren

| Element | Invullen |
|---|---|
| **Naam** | Duidelijke, eenduidige naam |
| **Definitie** | Exacte berekening (geen ambiguïteit) |
| **Bron** | Waar komt de data vandaan? |
| **Huidige waarde** | Baseline — wat is het nu? |
| **Doelwaarde** | Waar wil je naartoe? (gekoppeld aan OKR) |
| **Frequentie** | Hoe vaak update je deze metric? |
| **Eigenaar** | Wie is verantwoordelijk voor deze metric? |

---

## Stap 3: Visualisatie Kiezen

Elk type metric heeft een passende visualisatie. Kies niet op basis van wat mooi is, maar op basis van wat het snelst antwoord geeft.

| Wat je wilt zien | Visualisatie | Wanneer |
|---|---|---|
| Trend over tijd | **Lijngrafiek** | NSM, MRR, WAU — alles dat je over weken/maanden volgt |
| Huidige stand vs. doel | **Getal met sparkline** | Grote KPI's bovenaan: "4.523 WAU (doel: 5.000)" |
| Vergelijking tussen segmenten | **Staafdiagram** | Retentie per cohort, activatie per segment |
| Verhouding/percentage | **Donut of percentage bar** | Conversie-percentages, trial vs. betaald |
| Funnel | **Funnel-visualisatie** | Aanmelding → activatie → retentie → betaling |
| Afwijking signaleren | **Getal met kleurcodering** | Groen = op koers, Oranje = let op, Rood = actie nodig |

**Principes:**
- Bovenaan: North Star + trend (groot, onmisbaar)
- Middenin: Input metrics (de knoppen waaraan je draait)
- Onderaan: Operationeel (alleen kijken als er iets misgaat)
- Elke metric toont: huidige waarde, trend (omhoog/omlaag), vergelijking met vorige periode

---

## Stap 4: Alert-Drempels Instellen

Je wilt niet elke dag handmatig het dashboard checken. Stel alerts in voor wanneer iets buiten de norm valt.

**Per metric definiëren:**

| Drempel | Wat het betekent | Actie |
|---|---|---|
| **Groen** | Binnen verwachting of boven doel | Niets doen |
| **Oranje** | 10-20% onder doel of dalende trend 2+ weken | Onderzoeken |
| **Rood** | >20% onder doel of plotselinge daling | Direct actie |

**Voorbeeld:**
```
North Star: Wekelijks Actieve Teams
- Groen: > 4.000
- Oranje: 3.200 - 4.000 (20% onder doel)
- Rood: < 3.200 of >15% daling week-over-week
- Alert: Slack-notificatie bij oranje, PagerDuty bij rood
```

**Doorvragen:**
- "Bij welke daling zou je alles laten vallen om te onderzoeken?"
- "Welke metric heeft seizoensgebonden schommelingen die je niet als alert wilt?"
- "Wie moet genotificeerd worden bij een rood alert?"

---

## Stap 5: Review-Cadans

Een dashboard zonder review-ritueel is een screensaver.

| Cadans | Wat | Wie | Duur |
|---|---|---|---|
| **Dagelijks** | Snelle blik op North Star en alerts | PM | 2 min |
| **Wekelijks** | Input metrics reviewen, trends bespreken | Productteam | 15 min |
| **Maandelijks** | Diep-analyse, cohort-vergelijking, strategische implicaties | Team + stakeholders | 30-45 min |
| **Kwartaals** | Dashboard herzien: kloppen de metrics nog? Moeten er metrics bij/af? | PM + data | 30 min |

---

## Dashboard-Layout

**Voorgestelde indeling:**

```
┌─────────────────────────────────────────────────────────┐
│                    NORTH STAR METRIC                     │
│            [groot getal] + [trend sparkline]             │
│                   vs. doel: [doel]                       │
├────────────────────┬────────────────────┬────────────────┤
│   INPUT METRIC 1   │   INPUT METRIC 2   │  INPUT METRIC 3│
│   [getal + trend]  │   [getal + trend]  │  [getal + trend]│
├────────────────────┴────────────────────┴────────────────┤
│                    FUNNEL / RETENTIE                      │
│         [funnel-visualisatie of cohort-tabel]            │
├─────────────────────────────────────────────────────────┤
│              OPERATIONEEL (alleen bij alerts)             │
│         [error rate] [load time] [support tickets]       │
└─────────────────────────────────────────────────────────┘
```

---

## Output

Lever het volgende op:

1. **Metrics-lijst** — 5-8 metrics met definitie, bron, baseline en doel
2. **Dashboard-layout** — visueel voorstel met visualisatie-type per metric
3. **Alert-drempels** — groen/oranje/rood per metric
4. **Review-cadans** — wie kijkt wanneer hoe vaak
5. **Implementatie-advies** — welke tool, welke data-bronnen, wat moet er nog gebouwd worden

---

## Veel Voorkomende Fouten

- **Te veel metrics** — een dashboard met 20 grafieken is geen dashboard, het is een datawarehouse. Maximaal 8
- **Vanity metrics** — totaal aantal gebruikers is zinloos als je niet weet of ze actief zijn. Focus op actionable metrics
- **Geen baseline** — "conversie is 12%" zegt niets als je niet weet of dat goed of slecht is. Ken je baseline
- **Mooie grafieken, geen actie** — als het dashboard niet leidt tot beslissingen, is het decoratie
- **Geen alerting** — handmatig checken werkt niet. Automatiseer notificaties bij afwijkingen
- **Dashboard als bijlsluiter** — als het te complex is voor je publiek, versimpel het. C-level wil 3 getallen, niet 15 grafieken
- **Metrics en doelen niet alignen** — als je OKR zegt "verhoog retentie" maar je dashboard toont geen retentie, heb je een probleem

---

## Bronnen

- Sean Ellis — North Star Framework en metriekpiramide
- Amplitude — *North Star Playbook* (gratis gids)
- Stephen Few — *Information Dashboard Design* (2006) — visueel ontwerp van dashboards
- Reforge — Growth Metrics framework
