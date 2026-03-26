---
name: AI Evaluatiecriteria definiëren
description: Definieer evaluatiecriteria voor AI-output vanuit business-perspectief. Van criteria tot meetplan en monitoring.
triggers:
  - ai evals
  - evaluatie
  - ai kwaliteit
  - ai output
  - evaluatiecriteria
  - ai feature beoordeling
  - ai metrics
  - wanneer is ai goed genoeg
---

# AI Evaluatiecriteria Definiëren

## Metadata

**Gebruik deze skill als je:**
- Een nieuwe AI-feature bouwt en moet bepalen wat "goed genoeg" betekent
- Twijfelt of de kwaliteit van AI-output acceptabel is
- Moet communiceren naar stakeholders WANNEER je AI-feature live kan
- Monitoring wilt opzetten zodat je drift in kwaliteit detecteert
- Cost-quality trade-offs moet maken (betere modellen = hogere kosten)
- Controle en transparantie in AI-features wilt inbouwen

**Dit is UNIEK in product management:** Deze skill is geschreven voor POs/PMs, niet voor ML engineers. Het gaat over business-beslissingen rond AI-kwaliteit, niet over technische implementatie.

---

## Stap 1: Deep Questioning — Wat betekent "Goed" voor JOU?

Dit is het cruciale startpunt. Veel teams tellen metrics zonder eerst te definiëren: goed voor wie? Goed voor welke use case?

**Stel jezelf en je team deze vragen:**

1. **Wat is de impact als het fout gaat?**
   - Als mijn AI aanbeveling hier 10% van de tijd fout is, wat gebeurt er? (Een slechte productaanbeveling vs. een medische diagnose zijn totaal andere impact-niveaus)
   - Wie lijdt eronder? De eindgebruiker? Je support team? Je bedrijfsrepuatie?
   - Kun je dit zelf herstellen, of is het permanent schade?

2. **Voor welk probleem lost deze AI iets op?**
   - Wat deed het team voorheen? (handmatig sorteren, gokken, helemaal niet doen)
   - Hoe slecht was dat probleem? (Wat verliest jouw bedrijf/gebruiker als het niet opgelost wordt)
   - Is "90% accuracy" beter dan "handmatige werk van 8 mensen"? Ja. Is het beter dan "100% accuracy van 1 expert"? Misschien niet.

3. **Wie gebruikt dit en wat zijn HUN verwachtingen?**
   - Verwacht een HR-manager dat je AI CV's 100% juist categoriseert? Nee, ze verwacht dat het 80% juist is zodat zij 20% moet review'en
   - Verwacht een klant dat jouw chatbot 100% accurate is? Of 95%?
   - Wat zeggen je concurrenten? (Expectation anchoring)

4. **Waar zit je kost-beperkng?**
   - Is dit een gratis feature? (lagere kwaliteitsdrempel)
   - Betaalt je klant €100/maand? (hogere drempel)
   - Betaalt je klant €10.000/maand? (zeer hoge drempel)

5. **Kan de gebruiker het overriden of feedback geven?**
   - Als jouw AI-aanbeveling fout is maar de gebruiker kan het met 1 klik corrigeren en het systeem leert ervan: lagere drempel
   - Als jouw AI beslissing NIET kan worden overschreven: zeer hoge drempel

---

## Stap 2: Criteria Definiëren per AI Feature

Elke AI feature in je product heeft andere criteria. Begin met het definiëren van de volgende categorieën:

### 2.1 Accuracy/Relevance Criteria

**Definieer wat JE meet:**

| Criterion | Definitie | Voorbeeld |
|-----------|-----------|----------|
| **Accuracy** | % correct predictions | AI-categorisering: 85% van alle categorisaties juist |
| **Precision** | % positive predictions die juist zijn | Van alle users die AI als "high-value" label, hoeveel zijn het echt? (Hou false positives laag) |
| **Recall** | % van alle echte positives die AI vindt | Van alle echte high-value users, hoeveel vindt je AI? (Hou false negatives laag) |
| **Relevance** | Zijn de top-N resultaten bruikbaar? | Van de top-5 aanbevelingen, hoeveel zou je daadwerkelijk gebruiken? (Precision@5) |
| **Confidence** | Hoe zeker is het model? | Kan het model zeggen "ik ben maar 40% zeker"? |

**Keuze: Wat meet je?**
- Precision is belangrijker als false positives duur zijn (verkeerde targetering = verspilde marketing budget)
- Recall is belangrijker als false negatives een gemiste kans zijn (target missen = verloren klant)
- Voor recommendations: relevance@top-5 is zinvoller dan overall accuracy

### 2.2 User Experience Criteria

Dit gaat NIET over technische accuracy, maar over: voelt het goed aan voor de eindgebruiker?

| Criterion | Definitie | Voorbeeld |
|-----------|-----------|----------|
| **Responsiveness** | Hoe snel antwoordt het? | Chat moet binnen 2sec antwoord geven (niet 10 seconden) |
| **Consistency** | Geeft het dezelfde vraag steeds hetzelfde antwoord? | Je chatbot zegt vandaag X, morgen Y: slecht |
| **Transparency** | Laat het zien WHY het dit doet? | "Ik raad dit product aan OMDAT jij het merk eerder kocht" |
| **Graceful Degradation** | Wat doet het als het niet zeker is? | Bij lage confidence: fallback naar human, niet blokkering |
| **Overridability** | Kan de user het tegenspreeken? | User kan klikken "nee, fout" en het systeem leert ervan |

### 2.3 Business Impact Criteria

Dit zijn de ECHT belangrijke criteria — niet accuracy, maar: wat gebeurt er met je metrics?

| Criterion | Definitie | Voorbeeld |
|-----------|-----------|----------|
| **Adoption** | Gebruiken gebruikers dit feature? | Percentage users die de AI-aanbeveling minst 1x/maand openen |
| **Time Saved** | Hoeveel tijd besparen we? | Human review duurde 5 min/item, met AI 1 min: 80% time saved |
| **Retention** | Blijven users met AI feature langer klant? | Users die AI feature gebruiken hebben 15% hogere retention |
| **Error Cost** | Wat kost 1 fout ons? | 1 verkeerde medische diagnose = risico, schadeclaim, reputatie |
| **Support Load** | Hoeveel support-tickets creëert dit feature? | Als AI het fout doet, raken users gefrustreerd en bellen support |

---

## Stap 3: Measurement Method — HOE Meet Je Dit?

Nu je criteria hebt, hoe meet je ze?

### 3.1 Menselijke Evaluatie (Labeling)

**Wanneer:** Complex decisions, subjective quality, low-volume

**Hoe:**
1. Sample random outputs (100, 500, 1000 — afhankelijk van volume)
2. Laat 2-3 mensen onafhankelijk beoordelen (agreement = validiteit)
3. Bereken agreement (Cohen's kappa of Fleiss' kappa)
4. Bereken accuracy tegen golden standard

**Voorbeeld:** Je chatbot stelt 1000 vragen per dag. Week 1: label 100 random responses met 3 labelers. "Is dit antwoord bruikbaar ja/nee?"

**Kosten:** Hoog (mensenarbeid), maar betrouwbaar

### 3.2 Automatische Evaluatie (Metrics)

**Wanneer:** Veel volume, duidelijke ground truth, snelheid nodig

**Hoe:**
1. Definieer golden standard (wat is het juiste antwoord?)
2. Vergelijk output tegen golden standard
3. Bereken metrics (accuracy, precision, recall, F1)
4. Track over tijd

**Voorbeeld:** Je AI genereert product descriptions. Golden standard = handmatig geschreven descriptions. Vergelijk met BLEU/ROUGE scores (text similarity).

**Kosten:** Laag, maar alleen voor metrics met duidelijke ground truth

### 3.3 Hybrid Evaluatie

**Wanneer:** Veel output, maar niet alles labelen

**Hoe:**
1. Automatische metriek voor alle output
2. Menselijke sampling (random check) voor validatie
3. Gebruikersfeedback (thumbs up/down) als continuous signal

**Voorbeeld:** AI-categorisering voor 100k support tickets/week. 
- Automatisch: categoriseer alle tickets (dag 1)
- Menselijk sample: 200 random tickets per week labelen (dag 2-3)
- User feedback: support agents kunnen "correct/incorrect" klikken live (continu)

**Kosten:** Medium, maar scaleerbaar

---

## Stap 4: Threshold Definiëren — Wanneer is het "Goed Genoeg"?

Dit is waar veel teams falen. Ze denken: "mijn AI moet 95% accurate zijn." Maar 95% van wat? Voor welke use case?

### 4.1 Risk-Based Thresholds

Bepaal je drempel gebaseerd op IMPACT, niet op "standaard" getallen.

| Impact Level | Accuracy Drempel | Voorbeeld |
|--------------|------------------|----------|
| **Low Risk** | 70-80% | Suggestie voor volgende artikel ("je zou dit leuk vinden") |
| **Medium Risk** | 80-90% | Product categorisatie (user kan het zelf corrigeren) |
| **High Risk** | 90-95% | Email filtering (false positive = verloren mail) |
| **Very High Risk** | 95%+ | Medische diagnose, compliance decision, fraud detection |

**Kernprincipe:** Lagere threshold OKÉ als:
- Gebruiker kan het easy overriden
- Je hebt menselijke fallback
- Cost of error is laag
- Batch processing (je kunt achteraf corrigeren)

Hogere threshold NODIG als:
- Gebruiker kan het NIET overriden
- Real-time, geen fallback
- Cost of error is hoog

### 4.2 Precision vs. Recall Trade-off

Je kunt niet beide 100% hebben. Kies wat je meer wilt:

**Hoog Precision (weinig false positives):**
- "Als mijn AI zegt JA, is het 95% juist"
- Gebruiker vertrouwt de aanbeveling
- Voorbeeld: "Goedkeuren voor krediet" — false positive kost veel geld

**Hoog Recall (weinig false negatives):**
- "Van alle echte gevallen vindt mijn AI 95%"
- Je mist niemand
- Voorbeeld: "Detecteer fraud" — false negative kost veel geld

**Voorbeeld trade-off:**
Je AI moet leads identificeren. 
- High precision: "Als AI zegt JA, is het 95% goede lead" → sales converteert 19/20, blij
- High recall: "Van alle echte leads, vind ik 95%" → je mist 5% leads, jammer
- Wat kost meer: 1 verloren lead of 1 slecht lead naar sales? Als sales team groot is: high precision. Als leads schaars zijn: high recall.

### 4.3 Confidentiality Thresholds

Definieer ook: bij welke confidence voer je het uit?

```
IF confidence >= 90% → auto-execute (volledig AI-driven)
IF confidence 70-90% → suggest to human (human in the loop)
IF confidence < 70% → don't show (fallback or escalate)
```

**Voorbeeld:** Jouw support chatbot:
- 90%+ confidence: antwoord direct aan customer
- 70-90% confidence: suggest antwoord aan human agent die het kan aanpassen
- <70% confidence: "I'm not sure, let me connect you to an agent"

---

## Stap 5: Cost-Quality Trade-off — Waar is je Sweet Spot?

Betere modellen = hogere kosten (groter model, meer compute, betere training data, expert labeling).

### 5.1 Signaling Level: Waar Zit de Grens?

Je hoeft dit niet in detail uit te werken, maar: **waar voelt het onverantwoord om laag te gaan?**

```
Model A: 70% accuracy, €100/maand
Model B: 80% accuracy, €200/maand
Model C: 90% accuracy, €500/maand
Model D: 95% accuracy, €2000/maand

Vraag: Voor jouw use case, welk model is "verantwoord"?
```

**Factoren:**
- **Revenue impact:** Hoe veel geld verdien je met dit feature?
- **Brand risk:** Als je een slechte aanbeveling doet, verlies je dan klanten?
- **Support cost:** Hoe veel support tickets creëert lage quality?
- **User expectation:** Wat betaalt de user ervoor?

**Heuristic:** 
- Gratis feature: je kunt het riskant maken (70%+)
- Betaalde feature: middenweg (80-85%)
- Enterprise: moet betrouwbaar zijn (90%+)

---

## Stap 6: UX-Checklist — AI Product Design Principles

Dit zijn de "hygiene factors" — dingen die je MOET hebben, ongeacht je accuracy:

### 6.1 Transparantie
- [ ] Toont het systeem confidence level? ("Ik ben 85% zeker dat...")
- [ ] Laat het zien WHY het dit advies geeft? ("omdat je deze categorie eerder koos")
- [ ] Is duidelijk wat dit is: AI suggestion, niet fact?

### 6.2 Controle
- [ ] Kan de user het overriden/corrigeren?
- [ ] Kan de user zeggen "nee, jij hebt het fout"?
- [ ] Is er een undo/revert optie?

### 6.3 Verwachtingsmanagement
- [ ] Vertelt het systeem wat het WEL kan doen?
- [ ] Vertelt het systeem wat het NIET kan doen?
- [ ] Is duidelijk: "dit is een eerste draft, jij controleert"?

### 6.4 Graceful Degradation
- [ ] Als confidence laag is: fallback naar human, niet blokkering
- [ ] Laat het nooit een fout zien, altijd alternatief ("I'm not sure, here are alternatives...")
- [ ] Heeft het een "escalate to human" optie?

### 6.5 Progressive Disclosure
- [ ] Result eerst: "Here's your answer"
- [ ] Explanation on demand: "why?" button/link
- [ ] Niet overload met waarschijnlijkheden/uncertainty bands

---

## Stap 7: Monitoring Plan — Hoe Track Je Dit Over Tijd?

Quality drifts. Models degrade. Gebruikersgedrag verandert. Dit plan helpt je detecteren WANNEER het misgaat.

### 7.1 Continuous Metrics (Daily/Weekly)

| Metric | Check | Action bij afname |
|--------|-------|-------------------|
| **Confidence distribution** | Is het average confidence nog 80%? | Onderliggend model degraded? Retraining nodig? |
| **User feedback ratio** | Hoeveel % zegt "incorrect"? | > 5% "incorrect"? Escaleer |
| **Latency** | Hoe snel antwoordt het? | > 3sec? Cache/infra probleem? |
| **Support tickets** | Hoeveel tickets over dit feature? | Spike? Use case broke? |
| **Adoption** | Hoeveel % uses dit? | Daling? Users verliezen interesse |

### 7.2 Quarterly Deep Evaluation

Elke 3 maanden: menselijk sample, beoordeel 200-500 random outputs.

| What | Who | Trigger voor Action |
|------|-----|-------------------|
| Re-sample & label | 2 humans (blind) | Accuracy < threshold? Retrain. |
| Analyze failure modes | PM + ML eng | Wat gaat systematisch fout? (e.g., altijd fout voor kleine companies) |
| Cost-quality check | Finance + Product | Is dit nog verantwoord? Kunnen we goedkoper model gebruiken? |

### 7.3 Drift Indicators — Wanneer Retrain?

Jouw model is getraind op data van oktober 2025. Nu is maart 2026. Wat kan verschoven zijn?

**Data drift:** De inputs veranderen
- Voorbeeld: Je AI categoriseert producten. Klanten begonnen nieuwe producttype te uploaden. Model ziet het nooit gezien.

**Label drift:** De "juiste" antwoord verandert
- Voorbeeld: Sentiment analysis. In oktober was "pandemic talk" = neutral. Nu oktober 2026 = irrelevant.

**Prediction drift:** Model output verandert zonder interne reden
- Voorbeeld: Gemiddelde confidence was 85%, nu 72%. Geen code change, geen data change. Model degraded.

**Monitoring voor drift:**
- Track feature distributions wekelijks (input data dezelfde shape?)
- Track prediction distribution (output dezelfde verdeling?)
- Menselijke validation elke 3 maanden
- Retraining trigger: accuracy daalt >5% van baseline

---

## Output: Sjabloon Evaluatieplan

Vul dit in voor je AI feature:

```
# Evaluatieplan: [Feature Naam]

## Vragen (Stap 1)
1. Impact als het fout gaat: [antwoord]
2. Wat losten we op: [antwoord]
3. Wie zijn users & verwachtingen: [antwoord]
4. Kost-beperking: [antwoord]
5. Kan user overriden: [antwoord]

## Criteria (Stap 2)
Accuracy: [e.g., 85% of categorizations correct]
Precision: [e.g., 90% of "high-value" predictions are correct]
Recall: [e.g., find 95% of true high-value users]
Transparency: [e.g., show confidence score]
Time saved: [e.g., reduce review time 80%]

## Measurement (Stap 3)
Method: [human labeling / automatic / hybrid]
Sample size: [e.g., 200 random samples/week]
Frequency: [weekly / monthly / quarterly]

## Thresholds (Stap 4)
Accuracy threshold: [%]
Precision threshold: [%]
Recall threshold: [%]
Confidence cutoff: [% — when to execute auto vs. suggest]

## Cost-Quality (Stap 5)
Model A: [cost, accuracy]
Model B: [cost, accuracy]
Decision: Model [X] is responsible for our use case because [reason]

## UX Checklist (Stap 6)
[x] Shows confidence
[ ] Shows why
[ ] Transparent it's AI
[x] User can override
[ ] Has graceful degradation
etc.

## Monitoring (Stap 7)
Daily: accuracy, confidence distribution, latency
Monthly: user feedback analysis
Quarterly: deep re-label evaluation
Retraining trigger: accuracy < [X]%
```

---

## Bronnen

- **MIT xPRO, Designing AI Products** — AI Product Design Principles (Transparency, Control, Expectation Management, Graceful Degradation, Progressive Disclosure)
- **Product Faculty, C3 Capability Framework** — How products evolve from tools to teammates; evaluation should measure indispensability
- **Product Faculty, C4 Customer Framework** — Retention via dependency; metrics shift from frequency to necessity

---

## Key Insights

1. **"Good" is contextual.** 95% accuracy for your use case might be terrible or excellent. Start with impact questions, not numbers.

2. **Thresholds > Metrics.** Having a metric is useless without knowing when it's "good enough." Define thresholds first.

3. **UX > Accuracy.** An AI feature with 85% accuracy and graceful degradation often outperforms 95% accuracy with no user control.

4. **Cost matters.** Better models cost more. Know your budget and your break-even point.

5. **Monitor continuously.** Launch is not the end. Track whether the model still works, whether users still adopt it, whether it still saves time.
