---
name: experiment-ontwerp
description: "Ontwerp een experiment om je aanname zo snel en makkelijk mogelijk te valideren. Twee routes: nieuw product of bestaand product."
triggers:
  - experiment
  - validatie
  - test
  - a/b test
  - ab test
  - prototype
  - pretotype
  - mvp
  - hypothese testen
  - experiment design
---

# Experiment Ontwerp

## Metadata

**Doel:** Voor een gegeven aanname, design het *snelste en goedkoopste* experiment dat betrouwbare antwoorden geeft.

**Aanpak:** Twee routes (nieuw product: pretotyping; bestaand product: A/B, prototype). YODA-principe (Alberto Savoia): alleen data vertrouwen die je zelf verzameld hebt van echt marktgedrag. Geen opiniepeilingen.

**Output:** 1 experiment per aanname met: XYZ hypothesis, succes-drempel, timeline, kosten, implementation-stappen.

---

## Instructies

Je ontwerpt **één experiment per aanname**. Begin altijd met vragen.

### Fase 0: Context ophalen

**Stap 1 — Check wat er al is**
Scan uploads, gedeelde mappen en workspace op relevante bestanden (eerdere outputs, research, data). Lees ze door.

**Stap 2 — Slimme vragen stellen**
- **Wel context gevonden →** Bevestig kort wat je ziet ("Ik zie [X], klopt dat?"). Stel alleen vragen over wat je nog mist.
- **Geen context →** Stel onderstaande vragen.

1. **De aanname**: Wat exact willen we valideren? (Zorg dat het falsifieerbaar is)
2. **Huiidigen confidence**: Op schaal 1-5, hoe zeker zijn we nu al?
3. **De context**: Nieuw product of feature in bestaand product?
4. **De succesdrempel**: Wat telt als "aanname bevestigd"? (getal!)
5. **De constraints**: Hoeveel tijd / geld kunnen we hieraan besteden? Wanneer hebben we antwoord nodig?

---

## YODA-Principe: Alleen Vertrouwen Wat Je Meet

Dit is de fundament van elk goed experiment.

**YODA = Your Own Data Analysis**

Dit betekent:
- Geen opiniepeilingen ("Zou je dit betalen?")
- Geen hypothetische vragen ("Zou je dit gebruiken?")
- Geen sociale-wenselijke-antwoorden accepteren ("Ja, interessant!")
- **Alleen:** Wat mensen echt doen (klikken, kopen, gebruiken, verzoeken)

**Rode vlaggen — NIET doen:**
- "We sturen een enquête" ← Meningen, niet gedrag
- "We organiseren focusgroep" ← Groepsdenken en sociale wenselijkheid
- "We vragen of ze zouden betalen" ← Niemand zegt "nee" in een gesprek
- "We tellen hoeveel mensen op de ad klikten" ← Click-through ≠ intent

**YODA-vriendelijk:**
- "Hoeveel van die klikkers gaan echt door met signup?" ← Gedrag
- "Hoeveel betaalde werkelijk?" ← Geld spreekt
- "Hoeveel giorni gebruik ze het echt? (retention)" ← Langetermijn gedrag

---

## Framework: XYZ Hypothesis Format

Elk experiment werkt rond een XYZ hypothesis (Alberto Savoia):

```
We geloven dat [X doelgroep]
zal [Y gedrag vertonen / X conversie bereiken]
wanneer we [Z verandering maken]
```

**Voorbeelden:**

❌ **Slecht:** "Programmeurs zullen onze tool willen gebruiken"
→ Te vaag, niet testbaar, geen X/Y/Z

✅ **Goed:** "Junior Python developers zullen zich aanmelden voor de beta
wanneer ze een 2-min setup-video zien i.p.v. documentatie"
→ X = junior Python devs, Y = signup, Z = video i.p.v. docs

❌ **Slecht:** "Deze feature helpt users hun workflow sneller af te ronden"
→ "Sneller" is niet gemeten

✅ **Goed:** "Users die de export-feature gebruiken zullen 60% minder tijd
aan manual data-entry spenderen (vs. vandaag avg 4 uur/week)"
→ Testbaar, meetbaar, duidelijk wat "succes" is

---

## Route A: Nieuw Product — Pretotyping Experiments

Voor **volledig nieuwe producten** waar je nog geen codebase hebt.

Doel: Valideer VALUE en GTM-aannames met minimale build-effort.

### Experiment 1: Landing Page (VALUE)

**Wat:** Single-page website met value propositie + call-to-action (signup/waitlist).

**Leert:** "Zullen mensen dit interessant genoeg vinden om hun email in te voeren?"

**XYZ:** "Doelgroep Y zal hun email geven wanneer ze onze value propositie lezen."

**Succes-drempel:** "Minstens 10% conversion rate" (normen: tech/saas 1-5%, depending niche)

**Timeline:** 1-2 uur (Webflow, Framer, single HTML)

**Kosten:** $0-50

**Implementation:**
1. Hero section: probleem + jouw unique angle
2. 3-4 evidence bullets (wat maakt jouw anders vs. alternatives)
3. Email signup form (Convertkit, Mailchimp)
4. Paid ads test (Google Ads, Facebook): $50-100 budget, track conversions

**Succes-metrieken:**
- Click-through rate (hoe veel bezoekers zien de ad?)
- Conversion rate (hoe veel vult email in?)
- Cost per signup (ad spend / signups)

**Voorzichtig:** Hoge landing-page conversion kan fake zijn (je vrienden klikken).
→ Test met koude traffic (paid ads op relevant audience)
→ Minimaal 50 conversies voordat je concludeert

---

### Experiment 2: Explainer Video (VALUE + USABILITY)

**Wat:** 1-2 min animatie of screencast: probleem → jouw oplossing.

**Leert:** "Begrijpen mensen meteen wat dit doet? Is het intuïtief?"

**XYZ:** "Doelgroep Y zal video kijken tot het einde en kan uitleggen wat we doen."

**Succes-drempel:** "Minstens 70% watch-through rate; 80% kunnen het samenvatten"

**Timeline:** 2-5 uur (Loom, Figma prototype + voiceover, of bv. Runway)

**Kosten:** $0-50 (je eigengeluid + screencast) tot $200-500 (professionele animator)

**Implementation:**
1. Script: 90 seconden, focus op PROBLEM → SOLUTION → OUTCOME (niet features)
2. Storyboard: 3-4 key scenes
3. Film/animate en post
4. A/B test: video på landing page vs. zonder video

**Succes-metrieken:**
- Watch-through rate (hoe veel kijken tot einde?)
- Post-watch conversion vs. no-video (zegt video impact?)
- Inkomende feedback (wat snapten ze? Wat niet?)

---

### Experiment 3: Fake Door (VALUE + VIABILITY)

**Wat:** User denkt het product af te sluiten, maar in plaats daarvan landing ze op "thanks for interest, pre-order now" page.

**Leert:** "Zouden ze echt betalen voor dit? Hoe hoog kan de prijs zijn?"

**XYZ:** "Doelgroep Y zal [X] euro betalen voor pre-order wanneer ze begrijpen wat het doet."

**Succes-drempel:** "Minstens 5-10% van kwalificeerde traffic converts to pre-order intent"

**Timeline:** 2-3 uur (link + simple landing page)

**Kosten:** $0-50

**Implementation:**
1. Laad pseudo-product/demo (kan fake zijn, hoeft niet te werken)
2. After ~2 minuten of at CTA: "Helaas, dit is nog niet live. Wil je voorkant-toegang?"
3. Toon pricing options ($5/month? $29/month? VIP $99?)
4. Track: hoeveel zeggen ja? Bij welke prijs-tier?

**Succes-metrieken:**
- Pre-order intents (emails + prijs-keuze)
- Prijs elasticity (veel meer nee bij $99 vs. $9?)
- Frictie: hoeveel brekken op "payment method" stap?

**Voorzichtig:** Dit is ethisch grijs (je presenteert het als echt). Transparantie: "Dit is een early-access test" is oké, "complete scam" niet.

---

### Experiment 4: Concierge MVP (VALUE + USABILITY)

**Wat:** Jij doet het handmatig voor 5-10 early adopters. Zij denken dat het geautomatiseerd is.

**Leert:** "Werkt de workflow? Snappen ze het? Willen ze het echt?"

**XYZ:** "Doelgroep Y zal [X] keer per week het product gebruiken en 80% retention behouden."

**Succes-drempel:** "Minstens 5 actieve users; minstens 3 daily active; langetermijn engagement boven 50%"

**Timeline:** 1-2 uur setup + 2-4 weken runtime

**Kosten:** Je tijd (~10 uur/week)

**Implementation:**
1. Recruit 5-10 power users (via LinkedIn, communities, direct outreach)
2. Geef hen toegang tot "product" (maar jij automatiseert het achter scenes)
3. Run dit 2-4 weken; track: DAU, feature usage, churn, NPS
4. Interview na 1-2 weken: "Wat werkt? Wat niet? Zouden je betalen?"

**Succes-metrieken:**
- DAU (daily active users)
- Feature adoption (welke doen ze echt?)
- Time-in-product (hoe lang zetten ze eraan?)
- Churn (stoppen ze na dag 1?)
- NPS of "would you recommend"

**Gold-standard:** Concierge MVP leert je meer dan alles anders, omdat je real usage ziet.

---

### Experiment 5: Pre-Order (VALUE + VIABILITY)

**Wat:** Launch limited pre-order (Gumroad, Stripe) op basis van landing page + video.

**Leert:** "Zullen ze werkelijk betalen voordat het product af is?"

**XYZ:** "Doelgroep Y zal betalen voor pre-order van ons product."

**Succes-drempel:** "Minstens 20-30 pre-orders" (afhankelijk niche)

**Timeline:** 1-2 weken (setup) + 2-4 weken (kampagne)

**Kosten:** $100-500 (ads)

**Implementation:**
1. Landing page + explainer video (zie hierboven)
2. Gumroad product setup (pricing, email sequence)
3. Announce: Twitter, communities, warm outreach
4. Run ads: $100-200 budget
5. Track conversions, gather feedback van buyers

**Succes-metrieken:**
- Pre-orders acquired
- Cost per pre-order
- Feedback van buyers (waarom kochten ze?)
- Refund rate (remorse?)

---

## Route B: Bestaand Product — A/B, Prototype, Behavioral Experiments

Voor **features in bestaand product** waar je al traffic hebt.

Doel: Valideer USABILITY, FEASIBILITY, VIABILITY met real users.

### Experiment 1: A/B Test Feature (VALUE + VIABILITY)

**Wat:** Rol feature uit naar X% van users; meet engagment/retention vs. control.

**Leert:** "Gebruiken ze dit? Helpt het engagement/retention?"

**XYZ:** "Users die feature X gebruiken hebben Y% hoger engagement dan control."

**Succes-drempel:** "Minstens Y% uplift in primary metric (engagement/retention/conversion)" 
(stat sig. met voldoende sample)

**Timeline:** 1-2 weken setup + 2-4 weken runtime (hangt af van traffic)

**Kosten:** Dev time (je team)

**Implementation:**
1. Feature rollout: 10% users zien feature (cohort assignment)
2. Primary metric: wat meet je? (DAU? Feature adoption? Retention week 1-4?)
3. Secondary metrics: confounders? (Did we break something else?)
4. Collect: interaction data, event logging
5. Analyze: 2-4 weken later (moet statistical significant zijn)

**Succes-metrieken:**
- Feature adoption (% van test-cohort die feature gebruiken)
- Primary KPI (engagement, retention, revenue impact)
- Unintended side-effects (buggen, support load)
- Statistical significance (p < 0.05 minimaal)

**Voorzichtig:** "Feature adoption" ≠ "feature is goed"
- Zelfs slecht feature wordt soms gebruikt (curiosity)
- Focus op: retention, repeat usage, user feedback

---

### Experiment 2: Prototype in Staging (USABILITY)

**Wat:** Feature-prototype in staging environment; test met 5-10 power users + internal team.

**Leert:** "Is de UI intuïtief? Snappen ze het direct? Waar zit friction?"

**XYZ:** "Power users kunnen feature zonder instructie gebruiken en slagen voor [X taak]."

**Succes-drempel:** "Minstens 8/10 taak-success rate zonder docs"

**Timeline:** 3-5 uur (prototype) + 2-3 uur (user testing)

**Kosten:** Dev time + user compensation ($0-50 per user)

**Implementation:**
1. Build rapid prototype (Figma interactive? Code?) 
2. Recruit 5-10 power users of internal team members
3. Session: "Here's the new feature, can you [do X]?" — **don't explain it**
4. Observe: waar stokken ze? Waar zijn ze verward? Waar irritatie?
5. Iterate prototype op basis van feedback

**Succes-metrieken:**
- Task success rate (kunnen ze [X] af?)
- Time-to-completion (hoeveel seconden/minuten?)
- Error count (hoeveel verkeerde stappen?)
- Confusion points (opmerking: "ik snapte niet dat X")

---

### Experiment 3: Cohort Analysis (VIABILITY + VALUE)

**Wat:** Analyze existing data: users die feature al usage hebben (bv. indirect via API) vs. control.

**Leert:** "Correlates feature X met betere retention/revenue/engagement?"

**XYZ:** "Users die feature X gebruiken hebben Y% hoger [KPI] dan non-users."

**Succes-drempel:** "Statistisch significant uplift in KPI voor feature-users vs. control"

**Timeline:** 2-4 uur (data pull + analysis)

**Kosten:** $0

**Implementation:**
1. Identify: users die feature X hebt gebruikt (of proxy: interacted with [element])
2. Define comparison group: matched control (same cohort, signupdate, etc.)
3. Compare: KPI over 4/12 weken (retention, revenue, engagement)
4. Control: confounders (power users naturally more engaged)

**Succes-metrieken:**
- KPI difference (feature vs. control)
- Statistical significance (p < 0.05)
- Effect size (is verschil big enough to matter?)

**Voorzichtig:** "Correlation ≠ causation"
- Users die feature gebruiken zijn al meer engaged
- Pas cohort matching toe om bias te reduceren

---

### Experiment 4: Heatmap / Session Recording (USABILITY)

**Wat:** Install Hotjar / Fullstory / similar; record sessions van users die feature testen.

**Leert:** "Hoe gebruiken ze het werkelijk? Waar klikken ze verkeerd?"

**XYZ:** "Sessions tonen dat users [expected behavior] doen."

**Succes-drempel:** "Minstens 80% van sessions tonen expected user flow"

**Timeline:** 1 uur setup + 1-2 weken runtime

**Kosten:** $0-100/maand (free tier beschikbaar)

**Implementation:**
1. Install Hotjar / Fullstory
2. Flag cohort: "only record feature-beta users"
3. Watch 20-30 sessions: Where do they click? Where do they go wrong?
4. Note patterns: "X% klikt verkeerd op button Y"

**Succes-metrieken:**
- Click heatmap (waar vallen kliks?)
- Flow completion (volgen ze expected path?)
- Rage clicks (frustratie-indicators)
- Session duration (spent they time exploring?)

---

### Experiment 5: Wizard of Oz (VALUE + USABILITY)

**Wat:** User denkt features geautomatiseerd, maar je doet het semi-handmatig.

**Leert:** "Werkt de workflow? Waarom gebruiken of niet?"

**XYZ:** "Users zullen [X] keer per week feature gebruiken in Wizard of Oz setup."

**Succes-drempel:** "Minstens 70% DAU; minstens 50% week-2 retention"

**Timeline:** 2-3 uur backend + 2-4 weken runtime

**Kosten:** Je tijd (~5-10 uur/week)

**Implementation:**
1. Identify: 10-20 beta users
2. Build backend: User triggers action → manual fulfillment (via admin panel) → auto-response
3. Users think it's magic, you're doing it manually
4. Track: usage, feedback, churn
5. After 2-4 weken: "Thanks for beta! It was semi-automated, here's what we learned"

**Succes-metrieken:**
- DAU / feature adoption
- Time-to-first-use
- Repeat usage
- Qualitative feedback ("Why did you stop?")

---

## Stap 1: Definier Succes-Drempel (MANDATORY)

Voor elk experiment:

```
Dit experiment slaagt als [METRIC] > [NUMBER]
```

**Voorbeelden:**
- ❌ Slecht: "We zien goede engagement"
- ✅ Goed: "Landing page conversion > 5%"
- ✅ Goed: "A/B test shows >10% uplift in DAU (p<0.05)"
- ✅ Goed: "Prototype test: >80% task success rate"

**Waarom:** Anders kun je resultaten interpreteren hoe je wilt (bias). Vooraf bepaald = onvermijdbaar.

---

## Stap 2: Definieer Timeline & Budget

```
Timeline: [X uur setup] + [Y weken runtime] = [totaal tijdframe]

Budget: [dev-uren kosten] + [ad spend / tools] = [totaal geld]
```

**Richtlijnen:**

| Experiment | Timeline | Budget |
|---|---|---|
| Landing page | 1-2h | $0-50 |
| Video | 2-5h | $0-500 |
| Fake door | 2h | $0 |
| Concierge MVP | 1h setup + 2-4 weken | ~$0 |
| Pre-order | 2h setup + 2-4 weken | $100-500 |
| A/B test | 3-5h + 2-4 weken | Dev time |
| Prototype | 3-5h | $0-50 |
| Cohort | 2-4h | $0 |
| Heatmap | 1h + 1-2 weken | $0-100 |
| Wizard of Oz | 2-3h + 2-4 weken | Dev time |

---

## Stap 3: Data Sampling & Statistical Rigor

Voor alle experiments:

- **Minimum sample size:** 30 data points (regel van groot nummers)
- **Statistical significance:** p < 0.05 (95% confidentie dat result niet random is)
- **Running the numbers:** Als je 1% baseline conversion hebt en 10% test sees it, need ~100+ samples per cohort om significance te reach

**Tip:** Voor early-stage experiments (Concierge, Prototype, Fake Door), samples kunnen klein zijn.
Maar voor A/B tests op live product: computational rigor required.

---

## Output Checklist

Lever per experiment op:

1. **XYZ Hypothesis** — statement van wat je test
2. **Succes-drempel** — getal/metric
3. **Timeline** — setup + runtime
4. **Budget** — kosten
5. **Implementation plan** — stap-voor-stap
6. **Success metrics** — wat meet je, hoe?
7. **Interpretatie-kader** — "als we zien X, concluderen we Y"

---

## Veel Voorkomende Fouten

- **Opiniepeilingen als experiments doen** — "Zou je betalen?" is geen experiment
- **Geen vorafbepaalde succes-drempel** — cherry-picking results post-hoc
- **Statistisch insignificante resultaten trekken** — n=5 users = onbetrouwbaar
- **Fake-door-ethiek** — transparant zijn dat het een test is
- **A/B test rollout naar 50% in plaats van 5%** — risico's exposure
- **Experiment te lang laten lopen** — "we'll keep this forever" = spaghetti
- **Geen qualitative feedback** — nummers vertellen alleen half het verhaal

---

## Bronnen

- Alberto Savoia — *The Right It* (YODA, pretotyping, XYZ hypothesis)
- Eric Ries — *The Lean Startup* (validated learning, build-measure-learn)
- Ronny Kohavi, Diane Tang, Ya Xu — *Trustworthy Online Controlled Experiments* (A/B testing rigor)
- Product Faculty — Leverage Discovery (experiment taxonomy)
