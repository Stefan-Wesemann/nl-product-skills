---
name: pre-mortem
description: Bedenk voor lancering wat mis kan gaan. Categoriseer risico's als Tigers, Paper Tigers of Elephants en triage ze.
tags:
  - risico
  - risicoanalyse
  - pre-mortem
  - lancering
  - launch risk
  - failure planning
triggers:
  - pre-mortem
  - premortem
  - risico
  - risicoanalyse
  - lancering risico
  - what could go wrong
  - wat kan misgaan
  - failure risk
---

# Pre-Mortem

## Metadata

**Activatietrigger:** Je staat op het punt iets te lanceren (feature, product, markt) en wil proactief denkdenkend naar "wat kan misgaan?" VOOR het gebeurt.

**Doel:** Systematisch risico's identificeren → categoriseren (Tigers, Paper Tigers, Elephants) → triage op impact → preventie + fallback planning.

**Input:** PRD, launch plan, roadmap, of je eigen beschrijving van wat je gaat doen.

**Output:** Risico-overzicht met categorisering + impact-prioriteit + acties + fallback-plannen.

**Nota:** Pre-mortem is educatief. Je faciliteert dit samen met je team, je leert hoe je team denkt over risico.

---

## Instructies

### Fase 1: Wat Gaat Lanceren?

Eerst: duidelijkheid over WHAT.

**Doorvragen:**
1. Wat lanceren we? (Feature, product, markt, pricing-verandering, rebranding?)
2. Wie zijn users/betrokken?
3. Wat is het go/no-go moment?
4. Wanneer? (Datum, window, deadline)
5. Wie moet dit afstemmen? (Team voor pre-mortem sessie)

**Voorbeeld:**
- We lanceren "Workspace Templates" (feature) voor enterprise customers
- Launch-datum: 15 april
- Go/no-go: 1 april
- Team: Product, Engineering, Design, Customer Success

---

### Fase 2: Pre-Mortem Sessie (Team Exercise)

Dit is een **groepsoefening**, geen checklist die ik alleen invul.

**Setup (30 min):**

Zeg tegen het team:

> "We're on launch day (15 april) en het gaat helemaal fout. Wat is er gebeurd? Jullie vertellen: hoe zijn we hier gekomen?"

**Procedure:**
1. **Silent ideation** (10 min): Iedereen schrijft individueel op wat kon misgaan
   - Geen discussie, alles is geldig
   - Bedenk meerdere failure scenarios

2. **Voordragen zonder debate** (15 min): Iedereen leest, anderen schrijven mee
   - Geen "maar dat kan niet" → focus op "what could"

3. **Cluster & groeperen** (5 min): Welke risico's horen bij elkaar?

**Output van sessie:** Ungestructureerde lijst van mogelijke failures

---

### Fase 3: Categorisering — Tigers, Paper Tigers, Elephants

Dit is waar structuur binnenkomt. Ik categoriseer de risico's:

**TIGERS** (Echte risico's, waarschijnlijk + impactvol)
- Real problems die echt kunnen gebeuren
- Waarschijnlijkheid: Hoog (60%+)
- Impact: Hoog (launch stopt, revenue dip, customer churn)
- Voorbeeld: "Engineering kan performance niet opschalen → slow rollout"

**PAPER TIGERS** (Klinkt eng, maar niet echt)
- Overestimated risks
- Waarschijnlijkheid: Laag (< 30%)
- Impact: Laag-Middel (een paar customers angry, media notice, snelle fix mogelijk)
- Voorbeeld: "Media gaat kritiek hebben op UI design" (mogel, maar klein impact)

**ELEPHANTS** (Onuitgesproken, niemand durft erover)
- Risico's waar niemand over praat omdat het gevoelig is
- Waarschijnlijkheid: Onbekend
- Impact: Potentieel hoog (maar taboe)
- Voorbeeld:
  - "De klant die 30% van revenue is wil dit niet"
  - "VP Sales zal dit underminen vanuit angst voor cannibalization"
  - "Engineering team buigt onder pressure en kwaliteit daalt"

**Criteria per categorie:**

| Categorie | Waarschijnlijkheid | Impact | Urgentie | Actie |
|---|---|---|---|---|
| Tiger | Hoog (60%+) | Hoog | IMMEDIATE | Mitigate / fallback |
| Paper Tiger | Laag (< 30%) | Laag-Mid | Later | Monitor / accept |
| Elephant | Unknown | Potentieel hoog | IMMEDIATE | Surface / talk about |

---

### Fase 4: Risicochecklist (Context-Dependent)

Je bent niet blind. Ik help je **gerichte vragen** stellen per context.

**ALGEMENE CHECKLIST** (Geldt voor alles):

- **User adoption:** Hebben users dit nodig? Of is het de-lighting?
- **Performance:** Breekt het bestaande product? Load times ok?
- **Data/Privacy:** Passen we GDPR/compliance? Nieuwe data?
- **Dependencies:** Hangen we af van extern systeem/team/third-party API?
- **Timing:** Botst dit met ander werk? Customer-seizoen?
- **Communication:** Hebben we stakeholders aligned? Sales team trained?

**CONDITIONAL: AI-PRODUCT CHECKLIST** (Als feature AI bevat):

- **Hallucinations:** Kan het model "dingen verzinnen"? Hoe groot is de impact?
- **Bias:** Is output unfair voor bepaalde user-groepen?
- **Model drift:** Werkt model beter/slechter over tijd?
- **Data quality:** Is training data goed? Stale?
- **Transparency:** Weten users dat dit AI is? Snappen ze wanneer het werkt?
- **Fallbacks:** Wat doen we als AI fails? Manual override nodig?
- **Cost:** Model-inference kosten schaalbaar? Surprise bill risk?

---

### Fase 5: Impact × Effort Matrix (Prioritization)

Nu je Tigers/Paper Tigers/Elephants hebt, prioriteer je mitigatie.

```
HIGH           
IMPACT    │ MITIGATE        │ PLAN (later)
          │ (Do now)        │
          │ ╔═══════════════╗ │
          │ ║ Tiger risks   ║ │
          │ ║ Elephant      ║ │
          │ ╚═══════════════╝ │
─────────┼─────────────────┼────────→ EFFORT
          │ MONITOR         │ ACCEPT
          │ (accept risk)   │ (ignore)
          │                 │
          │ Paper Tigers    │
          │                 │
LOW       │                 │
```

**Bepaal per Tiger/Elephant:**
- Effort om te mitigeren? (Engineering hours, QA, training, deadline)
- Effort om fallback in place te zetten? (Go/no-go plan, rollback)
- Is het haalbaar VOOR launch?

**Triage-logica:**

| Risico | Impact | Effort to mitigate | Actie |
|---|---|---|---|
| Performance at 100k users | Hoog | Hoog (2 wk engineering) | Plan spike; mitigate if time allows; fallback: staged rollout |
| Sales team niet ready | Hoog | Laag (1 dag training) | FIX NOW |
| VP disagreement (Elephant) | Onbekend | Laag (1 meeting) | DISCUSS immediately |

---

### Fase 6: Mitigatie + Fallback Strategie

Per Tiger/Elephant: wat doen we?

**MITIGATE = Remove the Risk**
- Engineer a better solution
- Validate assumption early (pilot test)
- Add quality gates (test, monitoring)
- Train team (sales, support)

Voorbeeld: "Performance risk" → Målet load testing, monitor in beta

**FALLBACK = Plan B if Risk Happens**
- Rollback / staged rollout (launch only for segment)
- Manual override (support can help if AI breaks)
- Kill decision (this feature won't launch; we pivot)
- Communication plan (we tell customers why)

**Vul in per Tiger:**

| Tiger | Mitigation | Owner | Timeline | Fallback Plan | Go/No-Go moment |
|---|---|---|---|---|---|
| Performance at scale | Load test, optimize DB queries | Sarah (Eng) | Done by 30-mar | Staged rollout for 10% first | 1 Apr |
| Sales team adoption | 2-day training, battle cards | Jaap (Sales) | Week before launch | Hotline to support from Jaap | 3 Apr |
| VP doesn't want this (Elephant) | 1-on-1 with CEO, show customer demand | Me (PM) | This week | Delay launch 2 weeks OR feature flag off | By EOW |

---

### Fase 7: Team Alignment & Facilitatie

Je voert pre-mortem niet in je hoofd uit.

**Zo faciliteert je een pre-mortem met je team:**

1. **Kick-off** (5 min)
   - Zeg: "We lanch op [datum]. Stel je voor: het gaat helemaal mis. Wat gebeurde?"
   - Tone: "This is NOT blame, this is preventing disaster. All ideas valid."

2. **Silent ideation** (10 min)
   - Iedereen: whiteboard / doc / post-its
   - "Write everything you're worried about"

3. **Voordragen** (15 min)
   - Per persoon: wat schreef je?
   - Anderen: "Ik ook" → groeperen

4. **Q&A (niet debate)** (10 min)
   - Vragen voor clarification, niet "nee dat kan niet"
   - Elephant-surfacing: "Iets wat je niet durfde te zeggen?"

5. **Categoriseer samen** (15 min)
   - Tigers: "Dit kost ons de launch"
   - Paper Tigers: "Klinkt eng, maar klein kans"
   - Elephants: "Lastig, maar moet erover praten"

6. **Decide ownership** (10 min)
   - Per Tiger: wie neemt eigenaarschap?
   - Fallback: wie voert plan B uit als nodig?

7. **Action items** (5 min)
   - Volgende stap per Tiger
   - Moment voor check-in (weekly? bi-weekly?)

**Tips voor facilitatie:**
- Jij bent nota bene van outcomes, niet decision-maker
- Toon dat je risico's serieus neemt (en solutions)
- Surfacing van Elephants = team vertrouwt je
- Doe dit 2-3 weken VOOR launch, niet day-of

---

### Fase 8: FORCES Framework als Extra Risico-Lens

Je kunt ook FORCES gebruiken om weerstandsrisico's te dienen.

Vraag jezelf: wat zijn de **adoption risks** van je stakeholders?

| Stakeholder | Motivatie | Enablement | Momentum | Wrijving | Angst | Inertia |
|---|---|---|---|---|---|---|
| Customer | "Willen templates" | "Kunnen ze gebruiken?" | "Zien concurrenten doen?" | "Moet workflow veranderen" | "Wat als we kwijtraken?" | "Doen het oud-stijl" |

Per rij: wat kan de risk zijn?
- Low enablement? → Training fallback
- High inertia? → Phased rollout, incentives
- High friction? → Simplify UX first

---

## Output

Je levert af:

1. **Pre-mortem sessieverslag** (Wat kwam eruit van groepsoefening?)
2. **Categorisering** (Tigers / Paper Tigers / Elephants)
3. **Impact-prioriteit matrix** (Wat is critical?)
4. **Mitigatie + Fallback plan** (Per Tiger: wat doen we? Plan B?)
5. **Team ownership** (Wie verantwoordelijk?)
6. **Check-in cadence** (Hoe monitoren we?)

---

## Bronnen

- **Gary Klein** — Pre-Mortem technique (HBR, orig. "Performing a Project Premortem")
- **Product Faculty** — Risk Management & FORCES Framework
- **Andy Grove** — High Output Management (decision trees, contingency planning)
- **Taleb, Nassim Nicholas** — Antifragile (tail risks, black swans)

