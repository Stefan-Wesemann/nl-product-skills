---
name: north-star-metric
description: Bepaal je North Star Metric, identificeer sub-metrics en bouw een KPI-boom. Van business game classificatie tot meetplan.
tags:
  - north-star-metric
  - metrics
  - kpi
  - measuring
  - strategy
triggers:
  - north star
  - nsm
  - north star metric
  - kernmetric
  - kpi boom
  - metric tree
  - meten
  - metrics
---

# North Star Metric

## Metadata

**Triggers:** north star, nsm, north star metric, kernmetric, kpi boom, metric tree, meten, metrics

**Doel:** Bepaal jouw North Star Metric (NSM) — de ene metriek die de gezondheid van jouw product weerspiegelt — en bouw een volledige KPI-boom met sub-metrics en actionable maatstaven.

**Output:**
1. North Star Metric met duidelijke rationale
2. 3-5 sub-metrics die omlaag leiden naar de NSM
3. KPI-boom beschrijving (visueel of tekstueel)
4. Meetplan: hoe gaan we dit meten? Tools, frequentie, ownership

---

## Instructies

### Fase 1: Doorvragen over Business Context

Voordat ik een metriek voorstel, moet ik jouw business model snappen.

1. **Welk soort bedrijf ben je?** (SaaS, marketplace, media, e-commerce, etc.)
   - Dit bepaalt welk "business game" je speelt

2. **Hoe verdien je geld?** (Subscriptions, transaction fees, advertising, hybrid?)
   - Dit bepaalt welk gedrag cruciaal is

3. **Wat is je langetermijn-visie?** 
   - Waarom bestaat jouw product? (Inspiratie → North Star moet daar naar wijzen)
   - Wat willen gebruikers echt bereiken met jouw product?

4. **Wie zijn jouw doelgebruikers?** (Rol, segment, use case)
   - NSM moet relevant zijn voor HUN succesvolle outcome

5. **Wat zijn je huidas bottlenecks?** (Churn, activation, monetization, virality?)
   - NSM moet juist die bottleneck aanroeren

Ik wacht op **antwoorden** voordat ik verder ga. Als je onzeker bent → dat is info die ik nodig heb.

---

### Fase 2: Business Game Classificatie

Elke business behoort tot een van drie "games". Dit bepaalt je NSM:

#### Game 1: ATTENTION (Media, Creator, Entertainment)
**Wie:** News, podcasts, TikTok, Spotify, YouTube, Substack

**Waarvoor betaalt klant?** Advertenties, subscriptions voor ad-free, sponsorships

**Kernmetrie:** User engagement time / daily active users / session length

**Voorbeeld NSM:** "Average daily session length" (Netflix) of "Daily active users" (YouTube)

**Sub-metrics:** Sessies per user, content completion rate, time per session, repeat visits

#### Game 2: TRANSACTION (E-commerce, Marketplace, Payment, B2B SaaS)
**Wie:** Amazon, Bol.com, Uber, Stripe, HubSpot, Figma

**Waarvoor betaalt klant?** Per transactie, per seats, per volume

**Kernmetrie:** Transaction volume / value / frequency / GMV

**Voorbeeld NSM:** "Monthly transaction volume" (Uber) of "Annual contract value" (HubSpot)

**Sub-metrics:** Active buyers/sellers, transaction frequency, order value, repeat purchase rate

#### Game 3: PRODUCTIVITY (Collaboration, Developer tools, Utilities)
**Wie:** Slack, Notion, Airtable, Linear, Asana, Exact Online

**Waarvoor betaalt klant?** Seats, usage, features, integration

**Kernmetrie:** User adoption / "jobs completed" / team size / retention

**Voorbeeld NSM:** "Monthly active team members" (Slack) of "Daily active workspaces" (Notion)

**Sub-metrics:** Team invitations, integrations added, content created, collaboration events

---

**Doorvraag:** Welk game speel je? (Combinaties zijn mogelijk — bijv. marketplace + ads)

---

### Fase 3: 7 Criteria voor een Goede NSM

Niet elke metriek is geschikt. Een sterke NSM moet voldoen aan:

| Criterium | Waarom? | Check |
|-----------|--------|-------|
| **1. Begrijpelijk** | Elke teamlid (eng, design, PM, finance) snapt wat het betekent | Kun je het in 1 zin uitleggen? |
| **2. Klantgericht** | Reflecteert het succes van JOUW KLANT, niet alleen jouw business | Is de klant beter af? Of alleen jij? |
| **3. Duurzaam** | Niet easy-gamed. Klanten kunnen het niet kunstmatig inflateren | Wat gebeurt als iemand vals aanbod creëert? |
| **4. Visie-aligned** | Points naar je langetermijn-aspiratie, niet quickwin | Komt deze metriek voort uit je why? |
| **5. Kwantitatief** | Meetbaar, niet subjectief | Kun je hem tracken? Ja/nee? |
| **6. Actionable** | Product team kan ernaar handelen | Wat zou je veranderen om hem te verbeteren? |
| **7. Leading** | Corrigeert met toekomstig succes (niet lagging) | Stijgt deze metriek voor een week, gaat retention ook omhoog? |

---

**Doorvraag per kandidaat-metriek:**
- Snapt jouw team dit zonder uitleg?
- Kan iemand dit vervalsen door slecht gedrag?
- Welke actie zou je nemen om dit omhoog te brengen?

---

### Fase 4: Kandidaat-metriek Evalueren

Normaal gesproken zijn er 3-5 kandidaten. Laat mij ze together evalueren tegen de 7 criteria.

**Template:**

| Metriek | Begrijpelijk | Klantgericht | Duurzaam | Visie-aligned | Kwantitatief | Actionable | Leading | **Score** |
|--------|------|------|------|------|------|------|------|--------|
| Daily active users | 9/10 | 8/10 | 6/10 (easy gamed) | 7/10 | 10/10 | 8/10 | 7/10 | **55/70** |
| Session completion rate | 8/10 | 9/10 | 8/10 | 9/10 | 10/10 | 9/10 | 8/10 | **61/70** ✓ |
| Net retention rate | 6/10 (complex) | 9/10 | 9/10 | 10/10 | 10/10 | 7/10 | 8/10 | **59/70** |

**Doorvraag:** Waarom scoort jouw winnaar hoger dan de rest?

---

### Fase 5: North Star Metric Definiëren

Nu selecteren we de NSM en schrijven we het op.

**Format:**

```
**North Star Metric:** [Metriek naam]

**Definitie:** [Hoe meten we dit precies?]
- Numerator: [Teller: wat tellen we?]
- Denominator: [Noemer: waar delen we door?]
- Frequentie: [Dagelijks? Wekelijks? Maandelijks?]
- Target: [Waar willen we naartoe in 12 maanden?]

**Rationale:** [Waarom deze metriek?]
- Welk business game?
- Hoe refleceert dit klantensucces?
- Hoe align dit met onze visie?

**Visualisering:** [Grafiek hoe dit eruit ziet over de afgelopen 3-6 maanden]
```

**Concreet voorbeeld (SaaS):**
```
North Star Metric: Monthly Active Users per Workspace

Definitie:
- Numerator: Unieke users met minimaal 1 actie (invite sent, task created, comment) per maand
- Denominator: Per workspace/account
- Frequentie: Maandelijks gemeten, dagelijks getracked
- Target: MAU per workspace van 3.5 → 8 in 12 maanden

Rationale:
- Dit is het Game 3 (Productivity) metric
- Reflects groei van team adoption (klant succes)
- Link naar retention (teams met 5+ MAU hebben 95% retention, < 2 MAU churn)
- Haalbaar door: team invites, better onboarding, feature discovery
```

---

### Fase 6: Sub-Metrics Identificeren (de KPI-boom)

De NSM is ONE metriek. Maar je team kan er niet direct op handelen. Je nodig sub-metrics.

**Logica:** 
- NSM = het einddoel
- Sub-metrics = de onderdelen die naar NSM leiden
- Elk sub-metric moet een team kunnen verbeteren

**Template: 3-5 Sub-metrics**

```
NSM: Monthly Active Users per Workspace
├─ Sub-metric 1: Signup completion rate
│  └ Action: Optimize onboarding flow
│  └ Owner: Onboarding PM
│
├─ Sub-metric 2: Team invitation rate per user
│  └ Action: Surface invite in key moments
│  └ Owner: Product Designer
│
├─ Sub-metric 3: Feature adoption (% users using collab features)
│  └ Action: Better feature discovery, tutorials
│  └ Owner: Growth PM
│
└─ Sub-metric 4: Weekly retention rate
   └ Action: Reduce churn from inactive users
   └ Owner: Retention PM
```

**Doorvraag:** Wat doen we als NSM daalt? Welk sub-metric onderzoeken we EERST?

---

### Fase 7: KPI-Boom Visualisering

Je bouwt een boom die toont:
- NSM bovenaan
- Sub-metrics eromheen
- Actionable metrics/initiatives onderaan (wat gaan teams echt doen?)

**Format A: Tekstueel**
```
NORTH STAR: Monthly Active Users per Workspace (9.2 → 15 by Dec)

├─ GROWTH PILLAR (New user activation)
│  ├─ Signup-to-first-action: 72% → 85%
│  │  ├─ Email activation sequence: 45% → 60%
│  │  ├─ In-app tutorial completion: 60% → 75%
│  │  └─ Invite acceptance rate: 85% → 92%
│  └─ Days-to-5th-action: 14 → 7 days
│
├─ ENGAGEMENT PILLAR (Active usage)
│  ├─ Tasks created per user: 3.2 → 5
│  ├─ Comments per task: 1.1 → 1.8
│  └─ Integrations per workspace: 1.2 → 2.0
│
└─ RETENTION PILLAR (Keep them)
   ├─ Weekly retention (cohort): 72% → 82%
   ├─ Monthly retention (cohort): 45% → 60%
   └─ Churn rate: 6% → 3%
```

**Format B: Visueel** (Beschrijving voor diagram)
- Bovenkant: NSM als groot doelwit
- 3-4 branches: Growth, Engagement, Retention (of jouw pillars)
- Per branch: 2-4 sub-metrics
- Onderaan: Concrete initiatives/experiments

---

### Fase 8: Meetplan

Nu praktisch: hoe gaan we dit echt meten?

**Template:**

| Metriek | Tool | Frequentie | Owner | Ownership |
|---------|------|-----------|-------|-----------|
| NSM: MAU per workspace | Amplitude (funnel) | Daily dashboard, monthly review | Product Manager | PMO updates metrics every Monday |
| Signup completion rate | Mixpanel | Daily | Onboarding PM | Weekly check-in, alert if < 75% |
| Team invitations | Custom dashboard (Metabase) | Daily | Growth PM | Investigate weekly trends |
| Retention cohort | Amplitude cohort analysis | Weekly | Data Analyst | Monthly retention review |

**Praktische vragen:**
- Welke tools heb je al? (Amplitude, Mixpanel, Tableau, custom?)
- Wie beheert metrics? (Data analyst, PM, shared responsibility?)
- Hoe melden we dit? (Slack bot? Weekly email? Public dashboard?)
- Welke alerts zetten we? (NSM -10%? → investigate)

---

### Fase 9: Begin Hier, Verfijn Later

**Dit is BELANGRIJK:** Je hoeft dit niet perfect te hebben.

**Wat je deze week doet:**
1. Business game bepalen ✓
2. 3-5 kandidaten evalueren ✓
3. Winnaar selecteren + rationale schrijven ✓
4. 3 sub-metrics bepalen (niet alle 10) ✓
5. Basics meten starten ✓

**Wat je volgende maand doet:**
- Data valideren (Is NSM echt leading indicator?)
- Sub-metrics verfijnen (Welke werken echt?)
- Alerts instellen
- Team alignment sessie

**Wat je Q2 doet:**
- Volledige KPI-boom uitbouwen
- Link naar OKRs koppelen
- Predict models bouwen

Start simple. Verfijn als je data hebt.

---

## Output

Jij levert af:

1. **North Star Metric Definition** (naam, numerator/denominator, target, rationale)
2. **Sub-metrics (3-5)** met per metric: definition, owner, target
3. **KPI-Boom Beschrijving** (tekstueel of visueel)
4. **Meetplan** (welke tools, frequentie, ownership)
5. **Validatie-plan** (Welke aannames testen we over 3 maanden?)

---

## Bronnen

- **Amplitude North Star Framework** — https://amplitude.com/blog/north-star-metric
- **Product Faculty AI Northstar Framework** — Lecture notes
- **Sean Ellis & Morgan Brown**, Lean Analytics - Metrics that matter per business model
- **Reforge**, Product Analytics - KPI-boom structuring
- **Stripe, Figma, Slack** — Public North Star metrics (case studies)
