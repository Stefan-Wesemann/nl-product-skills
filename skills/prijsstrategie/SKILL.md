---
name: prijsstrategie
description: Bepaal je prijsstrategie met modelkeuze, waarde-analyse en validatie. Van Van Westendorp tot AI-kostenmodel.
tags:
  - prijsstrategie
  - pricing
  - pricing-strategy
  - tarieven
  - prijsmodel
triggers:
  - prijsstrategie
  - pricing
  - pricing strategy
  - prijsmodel
  - prijs
  - tarieven
---

# Prijsstrategie

## Metadata

**Triggers:** prijsstrategie, pricing, pricing strategy, prijsmodel, prijs, tarieven

**Doel:** Bepaal je prijsstrategie — niet alleen "welke prijs?" maar "hoe praat je over prijs met klanten?" Selecteer 2-3 relevante pricing-modellen, analyseer waardepropositie, bereken kostenmodel (als relevant), en valideer met klanten.

**Output:**
1. Gekozen pricing-model(s) met rationale
2. Prijsarchitectuur (tiers, features, pricing points)
3. Waarde-analyse (waarom deze prijs?)
4. Kostenmodel (indien AI-relevante product)
5. Validatieplan

---

## Instructies

### Fase 0: Context ophalen

**Stap 1 — Check wat er al is**
Scan uploads, gedeelde mappen en workspace op relevante bestanden (eerdere outputs, research, data). Lees ze door.

**Stap 2 — Slimme vragen stellen**
- **Wel context gevonden →** Bevestig kort wat je ziet ("Ik zie [X], klopt dat?"). Stel alleen vragen over wat je nog mist.
- **Geen context →** Stel onderstaande vragen.

---

### Fase 1: Doorvragen over Business Model & Doelgroep

Voordat ik pricing-modellen voorstel, moet ik begrijpen waar je bent.

1. **Wat is je product?** (SaaS, marketplace, AI-tool, consulting, mixed?)
2. **Wie is je primaire doelgroep?** (Enterprise, SMB, startups, consumers?)
3. **Hoe verdien je nu geld?** (Of hoe dacht je dit te doen?)
4. **Wat is je huidge pijnpunt met pricing?** (Onzekerheid, competition, positioning?)
5. **Hoe betalen klanten vandaag?** (Per user? Per transaction? Per month?)
6. **Wat is je business constraint?** (Need to hit revenue target? Stay competitive? Build moat?)

**Doorvraag:** Wat is je grootste uncertainty over pricing? (Klanten onwillig? Pricing power? Concurrentie?)

---

### Fase 2: Pricing-Model Selectie

Er zijn ~7 beproefde modellen. Ik kies 2-3 MEEST RELEVANT voor jouw situatie — niet alle 7.

#### Model 1: Freemium (Free tier + Paid tier)
**Wie:** Slack, Figma, Notion, Airtable
- Gratis tier met beperkte features
- Paid tier when you hit specific limit (users, seats, storage)

**Voordeel:** Lage acquisition friction, viral potential
**Nadeel:** Lage conversion (2-5%), moet overtuigen om upgrade
**Best for:** B2B SaaS, lage switching costs, viral use cases

**Doorvraag:** Kunnen klanten waarde krijgen in gratis tier? Hoe triggeren we upgrade?

#### Model 2: Per-Seat Subscription (per user/month)
**Wie:** HubSpot, Asana, Monday.com
- Prijs per team member per maand
- Standaard SaaS model

**Voordeel:** Predictable revenue, clear expansion path
**Nadeel:** Friction bij additionele seats, CAC hoog
**Best for:** Team collaboration tools, professional software

**Doorvraag:** Wie is de user vs. de payer? Match je pricing aan die roles?

#### Model 3: Usage-Based (Pay what you use)
**Wie:** AWS, Twilio, Stripe, OpenAI
- Prijs per API call, per GB, per token
- Elastic: meer gebruik = meer betaling

**Voordeel:** Aligned incentives (they only pay when they get value)
**Nadeel:** Unpredictable revenue, customer anxiety (bill shock)
**Best for:** Infrastructure, APIs, variable usage patterns

**Doorvraag:** Is je product high-variance usage (some months 100 calls, some 10K)? Of steady?

#### Model 4: Tier-Based (Good/Better/Best)
**Wie:** Mailchimp, Zapier, Salesforce
- Discrete tiers (Starter $10, Growth $50, Enterprise $500)
- Each tier = feature package + usage limit

**Voordeel:** Clarity, easy to understand, three options = middle usually wins
**Nadeel:** Awkward gaps (what if customer needs "Starter features + Growth usage"?)
**Best for:** When you have clear market segments

**Doorvraag:** Can you segment your market into 3 clear use cases?

#### Model 5: Value-Based (Prijs = value delivered)
**Wie:** Consulting, high-touch SaaS, premium tools
- Prijs determined by: customer ROI, risk savings, productivity gain
- Voorbeeld: "We save you $100K/year → we charge $30K"

**Voordeel:** Unlimited upside, aligned with customer success
**Nadeel:** Complex sales, need ROI models, hard to scale
**Best for:** Enterprise, high-touch, clear ROI

**Doorvraag:** Can you quantify customer value? (Cost savings? Revenue increase? Risk reduction?)

#### Model 6: Pricing-as-Revenue-Share
**Wie:** Shopify (takes % of sales), Upwork (takes commission)
- You take X% of what customer makes/transacts

**Voordeel:** Perfectly aligned (you win when they win), low friction
**Nadeel:** You own customer success (not scaling), need to build trust
**Best for:** Marketplaces, transaction networks, creator platforms

**Doorvraag:** Are you enabling customer revenue? Can you take a % cut?

#### Model 7: Hybrid (Combination)
**Wie:** Slack (seats + usage), Figma (teams + overage), AWS (base + usage)
- Multiple pricing dimensions combined
- Voorbeeld: "$10/user/month + $0.01 per API call over 10K/month"

**Voordeel:** Flexibility, captures more value, aligns with multiple use cases
**Nadeel:** Complex, confusing, hard to explain
**Best for:** Products with high variance in value per customer

**Doorvraag:** Are there multiple value dimensions? (Team size AND usage? Data AND processing?)

---

**Selectie:** Welke 2-3 models resonate? Met je business model matching?

Ik kies samen met jou. Dan duiken we dieper in die 2-3.

---

### Fase 3: Waarde-Analyse (Hoe veel is het waard?)

Nu bepalen we: op welk prijsniveau maken klanten een keuze?

#### 3.1: Van Westendorp Price Sensitivity Meter (eenvoudig)

Dit is een simpel vragenlijstje aan potentiële klanten:

1. "Bij welke prijs vind je dit product **te goedkoop**?" (Onder deze prijs: "Dit kan niet goed zijn")
2. "Bij welke prijs vind je dit product **minder interessant, maar nog acceptabel**?"
3. "Bij welke prijs wordt dit product **echt duur**?"
4. "Bij welke prijs vind je dit product **veel te duur**?"

**Voorbeeld antwoorden (SaaS tool):**
- Too cheap: $5/month
- Acceptable: $25/month
- Expensive: $75/month
- Too expensive: $150/month

**Analyse:**
- "Optimale prijs" = waar meeste klanten zeggen "acceptabel"
- "Price indifference point" = waar "minder interessant" en "echt duur" elkaar kruisen
- Je wilt in de zone zitten: acceptabel voor meeste, niet te goedkoop

**Output:** 3-5 prijspunten waar je customer feedback hebt.

**Doorvraag:** Welke prijs voelt JUIST? Niet te goedkoop, niet te duur?

#### 3.2: Competitive Pricing Analysis

Hoe prijzen concurrenten zich?

| Competitor | Pricing model | Price point | Per unit |
|---|---|---|---|
| Slack | Per user | $8-$12.50 | Per user/month |
| Microsoft Teams | Per user | $4-$6 (bundled with Office) | Per user/month |
| Discord | Freemium | $9.99 | Nitro subscription |

**Inzichten:**
- Zijn ze duurder/goedkoper? Waarom?
- Welk segment betaalt hoeveel?
- Welk pricing model domineren zij?

**Voorzichtig:** Kopieer niet blind. Pricing is strategy, niet race naar beneden.

**Doorvraag:** Waar positioneer je jezelf vs. hun? Premium? Discount? Niche?

#### 3.3: Customer Willingness to Pay (Direct)

Vraag potentiële klanten rechtstreeks:

- "Zou je dit kopen voor $X/month?"
- "Hoeveel zou je maximaal betalen?"
- "Hoe veel ROI verwacht je? → Wat kunnen we daar vragen?"

**Voorbeeld:**
- "Deze tool bespaart je 5 uur/week → bij $50/uur = $250/week value → we vragen $50/month (20% of value)"

**Doorvraag:** Hebben je potentiële klanten een budget voor dit? Hoeveel?

---

### Fase 4: CONDITIONAL: AI-Kostenmodel

**Dit is ALLEEN relevant als je product AI-powered is.**

Voeg een sectie toe: "AI Cost Structure"

#### AI Kosten Typering

| Kostentype | Voorbeeld | Impact op pricing |
|---|---|---|
| **Per-inference cost** | $0.001 per API call (OpenAI) | Direct pass-through → Usage-based pricing |
| **Model training** | $1000-10K per finetune | Sunk cost, amortize over customers |
| **Data processing** | $0.50 per 1M tokens | Per-usage or per-tier |
| **GPU/compute** | $0.50-2.00 per hour | Depends on on-prem vs. cloud |
| **Human review** | $20-50 per review (RLHF) | QA cost, factor into margin |

#### The 3-5x Rule

**Heuristic:** Your pricing should be 3-5x your marginal cost.

**Voorbeeld:**

```
If OpenAI API = $0.001 per call
And you expect 1M calls/month for customer = $1000/month cost
Then: 3-5x markup = $3000-5000/month customer pricing
```

**Voorzichtig:** Dit is baseline. Jij mag hoger gaan als je value > cost.

#### Kostenmodel Template

```
Product: AI Writing Assistant

Scenario: Mid-market customer (50 users)

COST SIDE (per month):
- OpenAI API calls (est 100K calls @ $0.001): $100
- GPT-4 upsell (est 50K @ $0.03): $1500
- Data processing (est 2GB @ $0.50/GB): $1
- Infrastructure (AWS, CDN): $300
- Human QA (5 hours @ $50/hr): $250
─────────────────────────────
Total Cost: $2,151/month

PRICING (3-5x rule):
- 3x: $6,453/month
- 5x: $10,755/month
- Reality check: That's $129-215/user/month. Is that defensible?

ADJUSTED PRICING:
- We charge $99/user/month = $4,950/month
- Margin: 230% ($4950 - $2151 = $2799 profit)
- Acceptable? Yes, covers support + R&D
```

**Doorvraag:**
- What is your actual per-unit cost?
- How many units per customer?
- What's your target margin? (50%? 80%? 95%?)
- Can customers absorb this price given their usage?

---

### Fase 5: Prijsarchitectuur Bouwen

Nu: hoe structureer je de tiers/features/limits?

#### Optie A: Freemium Tier-Based

```
Free Tier
├─ Features: 5 documents, 1 user, basic templates
├─ Limit trigger: "Upgrade when you hit 5 documents"
└─ Conversion hook: Need collab? Pay.

Pro Tier ($29/month)
├─ Features: Unlimited docs, 5 users, integrations
├─ Price psychology: Annual discount available ($29×10 = $290/yr)
└─ Target customer: Freelance, small teams

Team Tier ($99/month)
├─ Features: Unlimited, 20 users, API access, SSO
├─ Target: Growing teams
└─ Typical customer: 10-15 users (expansion opportunity)

Enterprise
├─ Custom pricing
├─ Negotiation: Volume discount? Long-term? Features?
└─ Target: 100+ users, need SLA
```

#### The "Magic Middle" (Goldilocks Effect)

Behavioral economics: When you offer 3 options, most people pick the middle.

```
Cheap Tier: $9/month (not attractive, "too cheap")
MIDDLE Tier: $29/month (feels right, MOST PICK THIS)
Premium Tier: $99/month (for power users)
```

Strategy: Price the middle tier where you want most customers to land.

#### Feature Packaging (What goes in each tier?)

**Principle:** Each tier unlock different motivations.

| | Free | Pro | Enterprise |
|---|---|---|---|
| **Use case** | Explore | Productive use | Org-wide |
| **Key feature** | All can access | Collaboration | Admin controls |
| **Unlocks** | Core job | Team work | Compliance |

**Avoid:** Feature fragments (where high-tier is JUST lower tier + 1 feature). Make jumps meaningful.

**Doorvraag:** At each tier, why would customer UPGRADE? What changes?

---

### Fase 6: Hoe Praat je Over Prijs?

Pricing is communication. How you present affects perception.

#### Principe 1: Annual Bias (2 maanden korting)
```
Monthly: $29/month ($348/year)
Annual: $290/year (save $58 = 2 maanden free)
```
→ Emphasize "save 2 months" not "discount 17%"

#### Principe 2: Anchoring Effect
```
Competitor prijs: $50/month
Jij: $29/month
Frame: "Premium features at SMB pricing"
NOT: "Cheaper than Slack"
```

#### Principe 3: Value Framing
```
NOT: "Get API access" (feature)
BUT: "Automate 10+ workflows with our API" (value)
```

#### Principe 4: Social Proof
```
"Join 5,000+ teams using X to save 5 hours/week"
```
→ Create FOMO if tiers are selling well.

**Doorvraag:** How will you communicate YOUR pricing? (Per user? Per value? Per outcome?)

---

### Fase 7: Validatie Plan

Pricing moet je testen. Dit is niet theoretisch.

**Validation steps:**

1. **Van Westendorp interviews** (5-10 potentiële klanten)
   - Ask the 4 questions
   - Identify optimal range
   - Timeline: 1 week

2. **Beta pricing test** (soft launch)
   - Launch with 1 pricing model
   - Monitor: conversion rate, churn rate, customer feedback
   - Timeline: 4-8 weeks

3. **Willingness to pay interviews**
   - Direct conversation with 3-5 customers
   - Ask: "Would you pay $X?" → adjust → test again
   - Timeline: 2 weeks

4. **Competitor pricing monitor**
   - Set up alerts for competitor pricing changes
   - Adjust quarterly if needed
   - Timeline: ongoing

**Success criteria:**
- Conversion rate: Target 10-30% for SaaS
- Churn rate: < 5% monthly for healthy pricing
- CAC payback: < 12 months ideally

---

## Output

Jij levert af:

1. **Pricing Model(s) Selected** (2-3 modellen met rationale)
2. **Pricing Architecture** (tiers, features, price points)
3. **Waarde-analyse** (Van Westendorp ranges, competitive analysis, WTP)
4. **CONDITIONAL: AI Cost Model** (if applicable: cost structure + 3-5x pricing logic)
5. **Communicatieplan** (How you frame pricing to customers)
6. **Validatieplan** (How you test before launch)

---

## Bronnen

- **Eric Almquist et al**, MIT xPRO AI Product Design — AI cost models
- **Robert Cialdini**, Influence — Anchoring effect, social proof in pricing
- **Stripe Pricing Guide** — Usage-based pricing best practices
- **Reforge**, Pricing Strategy — Willingness to pay, tier architecture
- **Product Faculty**, Pricing Frameworks
- **Van Westendorp PSM** — https://en.wikipedia.org/wiki/Van_Westendorp_Price_Sensitivity_Meter
