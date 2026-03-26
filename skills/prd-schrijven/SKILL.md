---
name: prd-schrijven
description: Schrijf een PRD dat engineering, design en stakeholders op één lijn brengt via een 8-sectie structuur met aannames en hypotheses.
triggers:
  - prd
  - product requirements
  - requirements document
  - feature spec
  - specificatie
  - product spec
---

# PRD Schrijven

## Metadata

**Wanneer activeren:** De gebruiker wil een Product Requirements Document schrijven voor een feature, product of initiative.

**Dit is geen snelle exercise.** Een goede PRD vraagt grondige voorbereiding. Ik ga diep: veel doorvragen, validatie van aannames, en structurering van onzekerheid.

**Verschil schaal:** Een kleine feature PRD (afhankelijkheid fix, UI-tweak) is compacter dan een grote initiative PRD (nieuw product, marktexpansie). Ik pas diepgang aan.

---

## Instructies

### 1. START MET DOORVRAGEN

Voordat ik ook maar één woord van de PRD schrijf, stel ik vragen over:

#### Product & Context
- Welk product/feature spreken we over? (Naam, huidige staat)
- Is dit brand new, een uitbreiding op bestaand, of replacement?
- Wie heeft dit bedacht? (PM, stakeholder, customer feedback, data?)

#### Scope & Doelen
- Wat willen we bereiken met deze feature? (Business outcome, niet "we maken een knop")
- Wie zijn de primaire gebruikers? (Rol, segment, use case)
- Zijn er secundaire doelgroepen?
- Wat meten we om succes te bepalen?

#### Team & Constraints
- Wie zit in het team? (Engineering, design, data, etc.)
- Zijn er technische beperkingen?
- Timeline druk? (Go-to-market deadline, afhankelijkheden)
- Budget/resource constraints?

#### Risico's & Aannames
- Wat zijn je grootste onzekerheden? (Technisch, marktgerelateerd, user behavior)
- Wat veronderstel je dat waar is?
- Zijn er concurrenten die dit al doen?

Ik stuur doorvragen als **gerichte vragen per categorie**, geen lange checklist. Ik wacht op antwoorden voordat ik structuur bouw.

---

### 2. PRODUCTHYPOTHESE EERST

Zodra ik context heb, formuleren we samen de **producthypothese**. Dit is de kern: wat geloven we en waarom?

Template (verplicht):
```
Wij geloven dat door [ACTIE/FEATURE]
voor [DOELGROEP/SITUATIE],
we [BEHAVIOR/OUTCOME] veroorzaken,
wat leidt tot [BUSINESS RESULTAAT].
```

Voorbeeld:
```
Wij geloven dat door workspaces per departement aan te bieden
voor enterprise-admins,
we de adoption van Slack in grote organisaties versnellen,
wat leidt tot meer seats en contract retention.
```

**Doorvraag per onderdeel:**
- Actie: Is dit concreet genoeg? Kan engineering dit bouwen?
- Doelgroep: Wie is dit echt voor? (Niet "users", maar rollen/segmenten)
- Behavior: Welk gedrag verwachten we? (User action, interactie, frequentie)
- Resultaat: Meetbaar? Link naar OKRs?

---

### 3. DE 8-SECTIE STRUCTUUR

Ik bouw de PRD altijd in deze volgorde:

#### Sectie 1: Samenvatting (Executive Summary)
- **Inhoud:** 1-2 alinea's. Wat is het? Waarom nu? Business case in 30 seconden.
- **Voor wie:** Busy stakeholders, leadership.
- **Doorvraag:** Zou een exexutive dit snappen zonder rest van PRD?

#### Sectie 2: Contactpersonen & Eigendom
- Product Owner/PM (contactgegevens, verantwoordelijkheden)
- Design Owner
- Engineering Lead
- Stakeholder(s)
- **Doorvraag:** Wie is eindverantwoordelijk als beslissingen nodig zijn?

#### Sectie 3: Achtergrond & Producthypothese
- **Achtergrond:** Wat leidde tot dit initiatief?
  - Market signals (data, feedback, trends)
  - Interne motivatie (OKR, strategie)
  - Competitieve druk
- **Producthypothese:** (De template uit stap 2)
- **Doorvraag:** Wat is het bewijs voor deze hypothese?
- **Doorvraag:** Welk experiment valideren we dit mee?

#### Sectie 4: Doelstelling (SMART OKRs)
- Wat willen we bereiken? **Measurable outcomes**, niet activities.
- Format: "Objective" (kwalitatief) + "Key Results" (kwantitatief, 3-5 per objective)

Voorbeeld:
```
Objective: Enterprise-customers sneller naar waarde

Key Results:
1. Time-to-first-login voor new enterprise-teams: < 5 minuten (nu: 20 min)
2. Workspace creation success rate: > 95% (nu: 78%)
3. Admin satisfaction score: 4.5+ (NPS-based)
```

- **Doorvraag:** Hoe weten we dat dit klaar is?
- **Doorvraag:** Wat zijn je stretch goals?

#### Sectie 5: Marktsegment & Waardepropositie
- **Marktsegment:** Wie boeit dit? (Rollen, bedrijfsgroottes, industrie, geografie)
- **Huidge pijnpunten:** Wat werkt niet goed nu?
- **Waardepropositie:** Wat krijgen ze beter/anders/goedkoper?
- **Concurrentie context:** Hoe zien anderen dit? (Differentiation?)

- **Doorvraag:** Waar verdienen we hier geld mee? (Direct of indirect)
- **Doorvraag:** Waarom zou je dit kopen vs. de concurrent?

#### Sectie 6: Oplossing (UX/Features/Technologie)
- **User Flows:** Stap-voor-stap wat doet de user? (Tekst of diagram)
- **Features:** Wat bouwen we precies?
  - Feature A: beschrijving + scope (in/out of scope)
  - Feature B: beschrijving + scope
  - Etc.
- **Technische Aanpak:** (Niet low-level details, maar strategische keuzes)
  - Bestaande systemen gebruiken? Nieuwe service?
  - Data flows, integraties?
  - Performance constraints?
- **UI/Design Principes:** (Niet full mocks, maar richtlijnen)
  - Consistency met bestaand product?
  - Accessibility?
  - Mobile vs desktop focus?

- **Doorvraag:** Kunnen we dit in fases leveren?
- **Doorvraag:** Wat laten we buiten scope?

#### Sectie 7: Aannames (EIGEN SECTIE)
Dit is **niet ondergesneeuwd in Oplossing**, maar eigen behandeling.

**Format:**
| Aanname | Type | Confidence | Test | Fallback |
|---------|------|------------|------|----------|
| Enterprise admins willen workspaces per dept. | User behavior | Medium (60%) | User interviews (5-10) | Offer workspaces per project instead |
| We kunnen multi-tenancy in 8 weken builden | Technical | High (85%) | Arch review + spike | Use existing SAAS provider |
| Market willing to pay $X/user/month | Market | Low (40%) | Pricing survey, sales comps | Freemium model instead |

**Soorten aannames:**
- User behavior: Wat doen gebruikers? Wat willen ze?
- Technical: Kunnen we dit bouwen? Performance? Reliability?
- Market: Willen klanten dit? Prijsbereidheid? TAM?
- Business: Winstgevendheid? Customer fit?

**Confidence rating:** Low (< 50%), Medium (50-75%), High (> 75%)

**Test:** Hoe valideren we dit? (Experiment, data, interview, prototype)

**Fallback:** Plan B als aanname fout is?

- **Doorvraag:** Welke aanname kill het hele project als het fout is?
- **Doorvraag:** Wat experimenteren we eerst?

#### Sectie 8: Release Plan & Metrics
- **Phasing:** Hoe brengen we dit naar markt?
  - MVP (phase 1): Wat is minimum viable? Wanneer?
  - Phase 2+: Expansies, optimisaties
- **Rollout:** Beta? Early access? Public launch?
- **Success Metrics:** Link terug naar doelstellingen
- **Monitoring & Fallback:** Wat doen we als metrics bad zijn?

- **Doorvraag:** Kunnen we dit sneller? Wat kunnen we weglaten?
- **Doorvraag:** Wat is het kill criterion (moment om te stoppen)?

---

### 4. CONDITIONAL: AI-FEATURES CHECKLIST

**Alleen relevant als de PRD AI-features bevat.**

Voeg onderaan een sectie toe: "AI Product Considerations"

Checklist:
```
[ ] Transparantie
    - Toont het systeem confidence scores/explainability?
    - Weet de user wanneer AI in beeld is?

[ ] Controle
    - Kan de user de AI-output negeren/overridden?
    - Zijn er fallbacks voor AI failures?

[ ] Verwachtingsmanagement
    - Communiceren we wat het AI-systeem kan/niet kan?
    - Trainingen voor users nodig?

[ ] Graceful Degradation
    - Wat gebeurt als AI-model faalt/hallucineert?
    - Fallback naar manual process? Show error?

[ ] Progressive Disclosure
    - Zien users eerst het resultaat of de uitleg?
    - Kunnen ze graven naar reasoning?
```

Voor elk item:
- **Status:** Ja/Nee/In progress
- **Reden:** Waarom is dit belangrijk voor dit product?
- **Owner:** Wie verzorgt dit?

---

### 5. OUTPUT

Als de PRD klaar is, lever ik drie dingen:

1. **De volledige PRD** (Markdown formaat, copy-paste-ready)
2. **Aannames-overzicht** (Tabel met confidence, tests, fallbacks)
3. **Open vragen lijst** (Dingen die nog beantwoord moeten worden voordat we bouwen)

---

## Bronnen

- **Marty Cagan**, Inspired - Requirements gathering & hypothesis-driven product
- **Teresa Torres**, Continuous Discovery Habits - Understanding user needs deeply
- **MIT xPRO AI Product Design** - AI-specific PRD sections & responsible AI
- **Reforge**, Product Strategy & PRD-writing (SMART OKRs, phasing)

