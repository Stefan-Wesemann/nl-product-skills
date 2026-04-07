---
name: wsjf-prioritering
description: "Prioriteer features, epics of initiatieven met WSJF (Weighted Shortest Job First). Scoor op business value, tijdkritiek, risicoreductie en job size. Levert een gerangschikte backlog op."
triggers:
  - wsjf
  - prioritering
  - prioriteren
  - weighted shortest job first
  - backlog prioriteren
  - feature prioritering
  - wat pakken we eerst
  - rangschikking
  - prioriteit bepalen
  - impact vs effort
---

# WSJF-Prioritering

## Metadata

**Doel:** Prioriteer je backlog objectief door de Cost of Delay af te zetten tegen de Job Size. WSJF voorkomt dat je team werkt aan wat het luidst schreeuwt in plaats van wat het meeste oplevert.

**Formule:** WSJF = Cost of Delay ÷ Job Size

Waarbij Cost of Delay = Business Value + Time Criticality + Risk Reduction / Opportunity Enablement

**Aanpak:** Score elk item op 4 dimensies (1-10), bereken WSJF, rangschik. Doe dit als team — niet alleen als PM. De discussie is minstens zo waardevol als de score.

**Output:** Gerangschikte lijst met scores, rationale per item, en aanbevolen volgorde.

---

## Instructies

### Fase 0: Context ophalen

**Stap 1 — Check wat er al is**
Scan uploads, gedeelde mappen en workspace op relevante bestanden (backlog-spreadsheets, vorige WSJF-scores, prioriterings-documenten, roadmaps). Lees ze door.

**Stap 2 — Slimme vragen stellen**
- **Wel context gevonden →** Bevestig kort wat je ziet ("Ik zie een backlog met 25 items, klopt dat?"). Stel alleen vragen over wat je nog mist.
- **Geen context →** Stel onderstaande vragen.

---

1. **Wat prioriteren we?** Features, epics, initiatieven, bugs? Zijn ze vergelijkbaar in scope?
2. **Hoeveel items?** Hoeveel staan er op de lijst? (Ideaal: 8-15. Meer dan 20 = eerst groeperen)
3. **Wie scoort?** Doe je dit alleen of met je team? (Aanbevolen: PM + Tech Lead + Designer minimaal)
4. **Strategische context**: Wat is de huidige productstrategie of het kwartaaldoel? Dit stuurt de scores
5. **Bestaande data**: Heb je al klantfeedback, usage data of urgentie-informatie per item?
6. **Constraints**: Zijn er items die sowieso eerst moeten (compliance, contractueel) ongeacht de score?

---

## De WSJF-Formule Uitgelegd

```
                  Business Value + Time Criticality + Risk Reduction
WSJF Score  =  ─────────────────────────────────────────────────────
                                    Job Size
```

Hogere WSJF = eerder oppakken. De logica: je wilt de items doen die het MEESTE opleveren (hoge Cost of Delay) en het SNELST klaar zijn (kleine Job Size).

---

## Stap 1: De Items Op een Rij

Zet alle te prioriteren items op een lijst. Per item heb je nodig:
- **Naam/titel**: Kort en herkenbaar
- **Beschrijving**: 1-2 zinnen over wat het is en voor wie
- **Eventuele context**: Klantfeedback, data, strategische relevantie

**Tip:** Als items te groot zijn om te vergelijken (een epic vs. een bugfix), splits ze of groepeer ze op vergelijkbaar niveau.

---

## Stap 2: Scoren op 4 Dimensies

Score elk item op een schaal van 1-10 per dimensie. Gebruik **relatieve scoring**: het hoogste item op een dimensie krijgt een 8-10, het laagste een 1-3. De rest valt ertussenin.

### Dimensie 1: Business Value (BV)

**Vraag:** Hoeveel waarde levert dit op voor gebruikers en het bedrijf?

| Score | Betekenis |
|---|---|
| 9-10 | Direct meetbare impact op kernmetric (retentie, conversie, omzet) |
| 7-8 | Significant voor een belangrijk segment, meetbaar maar indirect |
| 4-6 | Waardevol maar niet urgent, verbetert ervaring zonder kernmetric te raken |
| 1-3 | Nice-to-have, minimale meetbare impact |

**Doorvragen:**
- "Hoeveel gebruikers/klanten worden hierdoor geraakt?"
- "Wat is de verwachte impact op onze kernmetric?"
- "Hebben klanten hier actief om gevraagd of is dit ons idee?"

---

### Dimensie 2: Time Criticality (TC)

**Vraag:** Hoeveel erger wordt het als we dit uitstellen?

| Score | Betekenis |
|---|---|
| 9-10 | Harde deadline (contractueel, compliance, seizoensgebonden) |
| 7-8 | Concurrenten lanceren iets vergelijkbaars, first-mover voordeel verdwijnt |
| 4-6 | Wordt langzaam belangrijker, maar geen directe consequentie van uitstel |
| 1-3 | Geen tijdsdruk, kan over 6 maanden nog net zo goed |

**Doorvragen:**
- "Wat gebeurt er concreet als we dit 3 maanden uitstellen?"
- "Is er een externe deadline of marktmoment?"
- "Wordt het technisch moeilijker of duurder als we wachten?"

---

### Dimensie 3: Risk Reduction / Opportunity Enablement (RR/OE)

**Vraag:** Hoeveel risico neemt dit weg, of hoeveel maakt het mogelijk voor andere initiatieven?

| Score | Betekenis |
|---|---|
| 9-10 | Blokkeert andere hoog-waarde items, of neemt een kritiek risico weg |
| 7-8 | Maakt 2-3 andere items makkelijker of goedkoper |
| 4-6 | Enige synergie met andere items, of reduceert een middelgroot risico |
| 1-3 | Staat op zichzelf, geen afhankelijkheden of risicoreductie |

**Doorvragen:**
- "Welke andere items worden mogelijk of makkelijker als we dit eerst doen?"
- "Welk risico nemen we weg? Technisch, markt, compliance?"
- "Wat is de consequentie als dit risico realiteit wordt?"

---

### Dimensie 4: Job Size (JS)

**Vraag:** Hoe groot is de inspanning om dit te bouwen en te lanceren?

| Score | Betekenis |
|---|---|
| 1-3 | Klein: dagen tot 1 sprint. Helder, weinig onzekerheid |
| 4-6 | Middel: 2-4 sprints. Enige complexiteit en afhankelijkheden |
| 7-8 | Groot: 1-2 maanden. Significante technische uitdaging |
| 9-10 | Zeer groot: kwartaal+. Veel onzekerheid, meerdere teams nodig |

**Let op:** Job Size gaat in de NOEMER van de formule. Een lage Job Size (klein item) verhoogt de WSJF-score. Dat is de kern: kleine items die veel opleveren, ga je eerst doen.

**Doorvragen:**
- "Wat is de kleinste versie die we kunnen bouwen die nog waarde levert?"
- "Hoeveel onzekerheid zit erin? Weten we hoe we dit moeten bouwen?"
- "Zijn er afhankelijkheden van andere teams of systemen?"

---

## Stap 3: Berekenen en Rangschikken

Bereken per item:

```
Cost of Delay = BV + TC + RR/OE
WSJF = Cost of Delay ÷ Job Size
```

**Voorbeeld:**

| Item | BV | TC | RR/OE | CoD | JS | WSJF | Rang |
|---|---|---|---|---|---|---|---|
| Onboarding wizard | 9 | 7 | 6 | 22 | 4 | **5.5** | 1 |
| API v2 refactor | 5 | 3 | 9 | 17 | 8 | **2.1** | 4 |
| Notificatie-systeem | 7 | 5 | 4 | 16 | 3 | **5.3** | 2 |
| Enterprise SSO | 8 | 8 | 5 | 21 | 7 | **3.0** | 3 |
| Dark mode | 4 | 1 | 1 | 6 | 5 | **1.2** | 5 |

**Sorteer van hoog naar laag op WSJF-score.** Dat is je aanbevolen volgorde.

---

## Stap 4: Sanity Check

De score is een hulpmiddel, geen dictator. Check na het berekenen:

**Kloppen de top 3?**
- "Als ik deze volgorde aan de CEO zou presenteren, is dat verdedigbaar?"
- "Missen we context die de scores zouden veranderen?"
- "Zijn er items met een lage score die toch eerst moeten?" (compliance, critical bugs)

**Zijn de scores eerlijk?**
- "Heeft iemand zijn favoriete feature een 10 gegeven zonder onderbouwing?"
- "Hebben we Job Size realistisch ingeschat, of optimistisch?"
- "Zijn de Business Value scores gebaseerd op data of op onderbuik?"

**Outliers begrijpen:**
- Items met zeer hoge WSJF: klopt de Job Size echt? Is het niet te optimistisch?
- Items met zeer lage WSJF: moeten deze überhaupt op de backlog staan?

---

## Stap 5: Constraints Meenemen

Na de WSJF-rangschikking, pas aan voor realiteit:

- **Hard-blockers**: Items die contractueel of wettelijk verplicht zijn → altijd bovenaan, ongeacht score
- **Afhankelijkheden**: Item B kan niet zonder Item A → A moet eerst, ook als B hoger scoort
- **Teamcapaciteit**: Als je 2 teams hebt, kun je parallelle tracks plannen op basis van WSJF per track
- **Quick wins**: Items met WSJF > 4 en Job Size < 3 zijn quick wins — overweeg ze tussendoor te doen

---

## Het Scoringsgesprek

Doe dit als team, niet alleen. Zo faciliteer je het:

1. **Presenteer elk item** (PM): 1 minuut context per item
2. **Stille scoring** (iedereen): Ieder scoort individueel op alle 4 dimensies
3. **Vergelijk scores**: Waar zitten de grootste verschillen?
4. **Bespreek de uitschiters** (15 min): Waar scoort iemand een 3 en een ander een 9? Dat gesprek is goud
5. **Convergeer**: Pas scores aan na discussie, bereken WSJF
6. **Sanity check**: Klopt het totaalplaatje?

**Tip:** De discussie over WAAROM iemand anders scoort is waardevoller dan de score zelf. Het dwingt het team om aannames te benoemen.

---

## Output

Lever het volgende op:

1. **WSJF-scoretabel** — alle items met scores op 4 dimensies + berekende WSJF
2. **Gerangschikte lijst** — van hoog naar laag
3. **Rationale top 3** — waarom deze bovenaan staan, in 2-3 zinnen per item
4. **Constraints en aanpassingen** — welke items zijn verschoven door hard-blockers of afhankelijkheden
5. **Quick wins** — items met hoge WSJF en kleine Job Size die tussendoor kunnen
6. **Aanbevolen volgende stap** — wat pak je deze sprint/dit kwartaal op

---

## Veel Voorkomende Fouten

- **Absoluut scoren in plaats van relatief** — als alles een 8 krijgt, prioriteer je niets. Gebruik de volle range 1-10
- **Job Size onderschatten** — optimisme-bias zit overal. Vraag Engineering om een realistische schatting
- **Business Value baseren op onderbuik** — onderbouw met data. Hoeveel klanten vragen erom? Wat laat de data zien?
- **WSJF als dogma gebruiken** — het is een hulpmiddel voor gesprek, niet een orakel. Override als de context erom vraagt
- **Te veel items tegelijk scoren** — boven de 15 items wordt het chaotisch. Groepeer eerst
- **Alleen als PM scoren** — zonder Engineering mis je realistische Job Size, zonder Design mis je gebruikersinzicht
- **Time Criticality altijd hoog scoren** — niet alles is urgent. Als alles urgent is, is niets urgent
- **Afhankelijkheden negeren** — een hoge WSJF-score helpt niet als het item geblokkeerd is door iets anders

---

## Bronnen

- Don Reinertsen — *The Principles of Product Development Flow* (2009) — het origineel over Cost of Delay en WSJF
- SAFe Framework — WSJF-toepassing in Scaled Agile
- Joshua Arnold — Cost of Delay Blog (Black Swan Farming)
- Product Faculty — prioriteringsdiscussie als ontdekking
