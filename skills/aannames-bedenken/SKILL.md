---
name: aannames-bedenken
description: "Identificeer de riskante aannames onder je idee of feature. Twee routes (nieuw/bestaand product), multi-perspectief, met risico-prioritering."
triggers:
  - aannames
  - assumptions
  - risico
  - aanname identificeren
  - hypotheses
  - hypothese
  - validatie voorbereiden
  - risicoanalyse
---

# Aannames Bedenken

## Metadata

**Doel:** Maak expliciet welke aannames je product- of feature-idee steunt. Niet om ze allemaal gelijk te valideren, maar om te weten welke het meest gevaarlijk zijn als ze fout zijn.

**Aanpak:** Twee routes afhankelijk van context (nieuw product vs. feature in bestaand product). Multi-perspectief (PM, Designer, Engineer). Integratie van Product Faculty's Leverage Discovery hypothesen. Risico-prioritering: welke aanname raakt je meest als die fout is?

**Output:** Prioriteised list van 10-15 aannames, top 3 met risico-klassificatie, confidence ratings per aanname (1-5), aanbevolen experiment-type per top-3.

---

## Instructies

### Fase 0: Context ophalen

**Stap 1 — Check wat er al is**
Scan uploads, gedeelde mappen en workspace op relevante bestanden (eerdere assumptions-analyses, validatie-experiments, research-notes). Lees ze door.

**Stap 2 — Slimme vragen stellen**
- **Wel context gevonden →** Bevestig kort wat je ziet ("Ik zie [X], klopt dat?"). Stel alleen vragen over wat je nog mist.
- **Geen context →** Stel onderstaande vragen.

---

1. **Het idee**: Wat is precies het product-idee of de feature? (Beschrijf in 1-2 zinnen)
2. **De context**: Is dit een *volledig nieuw product* of een *feature in een bestaand product*?
3. **De bron**: Waarom denk je dat dit het juiste antwoord is? (Klantfeedback? Markttrend? Je eigen frustratie?)
4. **Doelgroep**: Voor wie is dit? (Vul zo concreet mogelijk in)
5. **Urgentie**: Welke aannames zijn cruciaal om volgende week al te valideren, en welke kunnen nog even wachten?

---

## Framework: Twee Routes

### Route A: Nieuw Product (6 categorieën)

Als je een **volledig nieuw product** bouwt, zijn dit de kritieke aannames:

#### 1. **VALUE**: Hebben mensen dit probleem echt?
- "Onze doelgroep ervaart dit als een pijnpunt met hoge prioriteit"
- "Dit probleem kost hun significant tijd/geld/moeilijkheid per maand"
- "Ze hebben al geprobeerd dit op te lossen (met workarounds of tools)"
- "Ze zouden actief geld/inspanning willen investeren om dit op te lossen"

**Rode vlag:** "Ze zeiden dat het interessant leek" is geen aanname dat er waarde is.

#### 2. **USABILITY**: Kunnen mensen ons product werkelijk gebruiken?
- "De gebruikersinterface is intuïtief voor onze doelgroep"
- "De learning curve past bij hun beschikbare tijd/geduld"
- "Ze hebben de juiste apparaten/vaardigheden/context om dit te gebruiken"
- "Onboarding duurt niet langer dan X minuten"

**Rode vlag:** "We bouwen voor tech-savvy users" is in veel markten een dodesteek.

#### 3. **FEASIBILITY**: Kunnen wij het technisch bouwen?
- "Met huidiger team en skill-set is dit haalbaar in X maanden"
- "We hebben geen blockers op 3rd-party integraties/APIs"
- "De kosten voor hosting/infra passen binnen budget"
- "Deze tech-stack schaal mee als we groeien"

**Rode vlag:** "We gaan een AI-model trainen" is geen aanname, dat is engineering-werk. Wel: "We kunnen dit model in goede kwaliteit runnen op gebruiker's apparaat" kan een aanname zijn.

#### 4. **VIABILITY**: Is dit financieel gezond?
- "We kunnen dit tegen X prijs verkopen"
- "Onze target Unit Economics (ratio bv. CAC:LTV) zijn positief op 24 maanden"
- "Concurrenten prijzen dit ook tegen X, dus dat gat bestaan"
- "De opslag die we nemen is verdedigbaar vs. waarde"

**Rode vlag:** "We verkopen tegen $9/maand maar CAC is $500" is een aanname die direct waarschijnlijk fout is.

#### 5. **GO-TO-MARKET**: Kunnen we klanten bereiken?
- "Er is een bestaand channel/platform waar onze doelgroep verzameld zit"
- "Onze boodschap resonates met messaging op die plek"
- "We hebben toegang tot of budget voor die channel"
- "Concurrenten gebruiken dezelfde channel, dus het werkt"

**Rode vlag:** "We zullen viral gaan" is geen Go-to-Market aanname, dat is hoop. "We kunnen betaalde acquisition tot X CAC runnen op Product Hunt" is concreet.

#### 6. **STRATEGY**: Fit dit in wat we willen zijn?
- "Dit product strengthens ons brand/positioning"
- "Dit sluit aan op langetermijn roadmap/vision"
- "Dit brengt ons niet in directe conflict met bestaande inkomstenbronnen"
- "Dit helpt ons defensible competitive advantage bouwen"

**Rode vlag:** "Dit volgt de markt" is het tegenovergestelde van strategie.

---

### Route B: Bestaand Product (4 categorieën)

Als je een **feature in een bestaand product** toevoegt:

#### 1. **VALUE**: Zal deze feature het kernprobleem van doelgroep oplossen?
- "De doelgroep erleeft het huiidigen workflow als pijnlijk in onderdeel X"
- "Ze hebben aangegeven dat ze bereid zijn dit als eerste te verbeteren"
- "Deze feature lost het probleem op (niet: voegt mogelijkheid toe)"
- "Ze zouden dit maanden eerder willen hebben dan feature Y"

**Rode vlag:** "Product team vindt dit cool" is irrelevant. "3 van onze 5 best customers vroegen hier expliciet om" is relevant.

#### 2. **USABILITY**: Past dit bij het bestaand product en user behavior?
- "Onze gebruikers zullen dit feature vinden (discovery)"
- "De UI/UX past in het bestaand design system"
- "De workflow onderbreekt niet het bestaand happypath"
- "Adoption rate zal boven X% liggen (t.o.v. baseline features)"

**Rode vlag:** "Het past technisch in de codebase" betekent niet dat het usable is.

#### 3. **FEASIBILITY**: Is dit haalbaarheid in ons development cycle?
- "Dit past in X sprints zonder huiidig roadmap te blokkeren"
- "We hebben geen upstream-dependency issues"
- "Geen onverwachte technical debt risk"

**Rode vlag:** "We zullen het refactoren" bij feature-adds = scope creep.

#### 4. **VIABILITY**: Helpt dit onze economie?
- "Dit verhoogt retention/engagement met Y% (baseline: Z%)"
- "Dit reduceert support tickets (impact: aantal per maand)"
- "Dit opens nieuw segment (IAC growth) of verhoogt ARPU"
- "Dit voorkomt customer churn naar competitor (defensief value)"

**Rode vlag:** "Dit is nice-to-have" is geen viability-aanname.

---

## Discovery Hypothesen: Een Extra Lens

Buiten deze categorieën, raadpleeg altijd Product Faculty's **4 Core Hypothesen** uit Leverage Discovery:

### H1: DOELGROEP — Wie dienen we werkelijk?
- "Ons huiidigen ICP (Ideal Customer Profile) is X"
- "Dit feature attracts/retains vooral [segment], niet [ander segment]"
- "We begrijpen de jobs/pains van deze groep goed genoeg om dit te bouwen"

**Onderzoeksvraag:** Zit dit feature in de top 3 pijnpunten voor dit segment?

### H2: ALTERNATIEVEN — Wat gebruiken ze vandaag?
- "Ze gebruiken huiidigen alternatieven: [A], [B], [C]"
- "Onze feature is duidelijk beter dan [B] in onderdeel X"
- "We weten waarom ze niet zelf deze feature in [C] hebben gebouwd"

**Onderzoeksvraag:** Hoe ziet het huiidigen workflow eruit en waarom is onze feature beter?

### H3: VOORDEEL — Wat kunnen wij dat concurrenten niet?
- "Concurrents features vergelijkbaar, maar wij hebben [defensible voordeel]"
- "Dit voordeel is moeilijk te kopieren (network, data, positioning)"
- "Dit voordeel rechtvaardigt onze prijs/positioning"

**Onderzoeksvraag:** Wat kunnen wij hier uniek doen dat competitors niet makkelijk kunnen copyen?

### H4: TREND — Wat maakt dit nu mogelijk?
- "Marktshift [technologie / regelgeving / behavior] maakt dit relevant nu"
- "Dit moment voorbij, dit feature wordt irrelevant over 18 maanden"
- "Onze timing is strategic, niet lukraak"

**Onderzoeksvraag:** Waarom lukt dit NU en niet vorig jaar? Wat verandert?

---

## Stap 1: Lijst de Kandidaat-Aannames

Werk beide routes parallel (of kies Route A/B afhankelijk van context). Brainstorm per categorie:

**Template voor brainstormen:**
```
ROUTE A / ROUTE B: [Categorienaam]

Onze aannames zijn:
1. [Aanname 1 — begin altijd met "We geloven dat..."]
2. [Aanname 2]
3. [Aanname 3]
...
```

**Tip:** Elke aanname moet:
- Falsifieerbaar zijn (niet: "klanten zullen het willen", wel: "minstens 40% van doelgroep zal dit maanden eerder willen hebben dan alternatieven")
- Observable zijn (niet: "dit is innovatief", wel: "de feature biedt 3x sneller workflow dan huiidigen alternatief X")
- Gemeten kunnen worden (getal, % of ja/nee observatie)

---

## Stap 2: Multi-Perspectief — PM, Designer, Engineer

Dit is **cruciaal**. Elke rol heeft ander blinde plekken.

### PM-Perspectief
- Focusseert op VALUE en VIABILITY
- Risk: overdrijft wat klanten willen; onderschat execution risk
- Vragen: "Hebben we direct met klanten gesproken? Hebben ze actief om dit gevraagd?"

### Designer-Perspectief
- Focusseert op USABILITY en VALUE (hoe voelt het?)
- Risk: optimaliseert elegantie boven simplicity; onderschat doelgroep werkelijkheid
- Vragen: "Wie moet dit echt gebruiken? Wat is hun huiidigen context? Hoe snel moeten ze dit leren?"

### Engineer-Perspectief
- Focusseert op FEASIBILITY en scalability
- Risk: ziet alleen technical blockers; onderschat user-behavior impact
- Vragen: "Wat kan fout gaan? Welke dependencies missen we? Wat breekt als 10x meer users dit gebruiken?"

**Praktijk:** Leid elk perspectief apart 15 minuten, dan merge:
1. "PM, wat zijn jouw top-3 riskante aannames?"
2. "Designer, hoe ziet een user dit werkelijk gebruiken? Wat kan misgaan?"
3. "Engineer, waar zie jij technical risk?"
4. Merge tot gedeelde top-3 lijst.

---

## Stap 3: Confidence Rating per Aanname

Score elke aanname 1-5:

- **5**: "We hebben dit gevalideerd in 10+ klantgesprekken, alle zeiden ja, en zelfs betaald al"
- **4**: "Klanten hebben dit directe gevraagd, en concurrenten bieden het, dus markt bestaat"
- **3**: "Dit klinkt logisch, maar we hebben het niet direct getest; wel past het in bekende patronen"
- **2**: "Dit is een intelligent gok, maar we hebben weinig data; veel kan hier fout gaan"
- **1**: "Dit is puur speculatie; we hebben geen data of expert consensus"

**Belangrijk:** Lage confidence = hoge prioriteit voor validatie. Niet het tegenovergestelde!

---

## Stap 4: Risico-Klassificatie

Niet alle aannames zijn even belangrijk. Klassificeer per aanname:

### TIG — **T**ight **I**ntegration with **G**rowth

Deze aanname bepaalt of het product überhaupt schaalbaar is. Fout = volledig mislukt.

*Voorbeelden:*
- "Er is marktevraag voor dit probleem" (TIGE)
- "We kunnen economisch klanten bereiken" (TIGE)
- "Unit economics worden positief op 24 maanden" (TIGE)

### TOY — **T**echno **O**pportunity **Y**ield

Deze aanname bepaalt of we het technisch kunnen bouwen op schaal.

*Voorbeelden:*
- "We kunnen dit op gebruikers-apparaat runnen onder 2s latency" (TOY)
- "De API's die we nodig hebben zijn beschikbaar" (TOY)

### MUST — Must-haves voor product-market fit

Deze aannames bepalen of het product bruikbaar en begeerd is.

*Voorbeelden:*
- "Doelgroep vindt deze UI intuïtief" (MUST)
- "Setup duurt <5 minuten" (MUST)

**Rangschikking voor validatie:**
1. TIGE — validate eerst (stop-loss)
2. MUST — validate tweede (product betreft)
3. TOY — validate derde (execution betreft)

---

## Stap 5: Top-3 Aannames met Experiment-Type

Selecteer je top-3 meest risicante/laag-confidence aannames. Voor elk:

1. **Aanname** (statement)
2. **Huiidigen confidence** (1-5)
3. **Waarom dit risicant** (als dit fout is, wat gaat er mis?)
4. **Aanbevolen experiment-type** (zie overzicht hieronder)

### Experiment-Type Overzicht

**Route A (Nieuw Product)**

- **VALUE-aannames valideer met:** Customer interviews (klachten 10+ targets), pretotype (landing page, explainer video), fake door (pre-order/waitlist)
- **USABILITY-aannames valideer met:** Prototype usability test (5-8 users), concierge MVP (jij doet het handmatig voor hen)
- **FEASIBILITY-aannames valideer met:** Technical spike, proof-of-concept
- **VIABILITY-aannames valideer met:** Pricing experiment (fake pricing page), cohort analysis (simulation)
- **GTM-aannames valideer met:** Channel test (pilot paid ads), fake door via channel (zie je opscaling)

**Route B (Bestaand Product)**

- **VALUE-aannames valideer met:** A/B test feature (percentage users zien het), cohort analysis (engage rate verschil)
- **USABILITY-aannames valideer met:** Prototype in staging (intern + 5-10 power users), heatmap/session recording
- **FEASIBILITY-aannames valideer met:** Technical spike, load test
- **VIABILITY-aannames valideer met:** Cohort analysis (retention/engagement verschil), revenue impact simulation

---

## Output Checklist

Lever het volgende op:

1. **Volledige aannames-lijst** — minimaal 10-15 items, per route/categorie
2. **Confidence-ratings** — 1-5 per aanname
3. **Risk-klassificatie** — TIGE / MUST / TOY per aanname
4. **Top-3 prioriteit** — gerangschikt op risico + lage confidence
5. **Experiment-aanbevelingen** — per top-3 aanname, type + korte beschrijving
6. **Merge-rapport** — hoe PM, Designer, Engineer het eens zijn (en waar ze het *nog* niet eens zijn)

---

## Veel Voorkomende Fouten

- **Te veel aannames tegelijk willen valideren** — focus op top-3, niet alle 15
- **Confidence overschatten omdat je "voelde dat het klopt"** — gevoel is niet data
- **Geen onderscheid tussen TIGE/MUST/TOY** — niet alle aannames zijn even kritiek
- **VALUE-aanname confunderen met feature-feedback** — "feature klinkt cool" ≠ "probleem is groot"
- **De Designer/Engineer niet echt vragen** — monoloog van PM is bias
- **Aanname is te breed** ("doelgroep zal het willen") — specifiek maken ("minstens 40% van X zal dit kiezen boven Y")
- **Geen back-up experiment gedefinieerd** — "wat doen we als experiment faalt?"

---

## Bronnen

- Product Faculty — *Leverage Discovery* (hypothesen H1-H4, prioritering TIGE/MUST/TOY)
- Teresa Torres — *Continuous Discovery Habits* (aanname-driven discovery)
- Marty Cagan — *Inspired* (risky assumptions)
- Lean Startup — aanname-testing discipline
