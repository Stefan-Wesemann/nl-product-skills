# NL Product Skills

[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
[![Skills](https://img.shields.io/badge/skills-35-orange.svg)](#wat-zit-erin)
[![Nederlands](https://img.shields.io/badge/taal-Nederlands-red.svg)](#)

35 Nederlandstalige skills voor product management. 

Een skill is een pakketje instructies dat ingeladen wordt wanneer je het met Claude of een andere AI aanroept. Met een skill maak je van generieke AI assistent, een AI-expert, zonder dat je daar zelf veel moeite voor hoeft te doen. 

Die moeite heb ik al voor je gedaan.

Mijn skills bevatten instructies op basis van wat mij betreft de beste producttheorieën. Denk aan frameworks zoals Jobs to Be Done, WSJF, FORCES, Blue Ocean, Seven Powers, The Mom Test en meer.

Skills werken onafhankelijk. Je hoeft er geen 35 te installeren om er één te gebruiken. Allemaal downloaden en proberen kan natuurlijk wel altijd.

**Tip:** Een skill wordt vele malen beter wanneer je ook relevante documenten toevoegt aan je gesprek. Hoe meer context Claude heeft, hoe gerichter de vragen en hoe beter de output zal zijn. De combinatie van een skill met jouw relevante context en jouw input op de vragen zorgt voor de beste resultaten.


## Aan de slag

### Stap 1. Download een skill van GitHub

Ga naar de [`skills/`](skills/) map in deze repo. Open de map van de skill die je wilt gebruiken, bijvoorbeeld [`klantinterview`](skills/klantinterview/). Klik op `SKILL.md`. Klik rechtsboven op het download-icoon (of op **Raw** en dan opslaan met Ctrl+S / Cmd+S).


<img width="750" height="300" alt="Scherm­afbeelding 2026-04-07 om 22 38 56" src="https://github.com/user-attachments/assets/2d1d8e1f-f2a5-49ba-85e2-b614ae21e071" />



### Stap 2. Upload de skill in Claude

Open Claude desktop en ga naar **Cowork**. Klik op **Customize** in de linkerzijbalk, dan op **Skills**, dan op het **+** icoon. Kies **Upload a skill** en sleep het bestand erin.


<img width="1903" height="335" alt="Scherm­afbeelding 2026-04-01 om 11 03 01" src="https://github.com/user-attachments/assets/684d1f81-5078-4600-9924-39273b554f64" />


Sleep hier je gedownloade skill .md file naartoe en je skill is onderdeel van je Claude:


<img width="400" height="280" alt="Scherm­afbeelding 2026-04-01 om 11 03 25" src="https://github.com/user-attachments/assets/a0bec84b-0479-46dd-8ef2-06b14ae72d3c" />


### Stap 3. Gebruik de skill

Start een nieuw gesprek en typ `/`. De skill verschijnt in de lijst. Klik erop en je bent aan het werk.

<img width="803" height="382" alt="Scherm­afbeelding 2026-04-07 om 22 51 37" src="https://github.com/user-attachments/assets/77c9d542-a116-440d-93a1-3b098d98bd30" />


Wil je het eerst uitproberen met één? Snap ik. 
Hier download je klantinterview op basis van de mom test: [`klantinterview`](skills/klantinterview/SKILL.md). Een skill die je helpt bij écht goede interviewvragen om hiermee je plannetje te valideren.

> LET OP: Je hebt een betaald Claude-account nodig (Pro, Team of Enterprise) om van skills in Claude gebruik te kunnen maken.

<details>
<summary>Via Claude Code</summary>

Als je Claude Code gebruikt, werkt het via het plugin-systeem:

```
/plugin marketplace add Stefan-Wesemann/nl-product-skills
```

Daarna kun je browsen via `/plugin` (ga naar het **Discover** tabblad) of direct installeren:

```
/plugin install nl-product-skills@nl-product-skills
```

> Deze route is nog in ontwikkeling. Werkt het niet? Clone de repo en kopieer de `skills/` map naar je project.

</details>


## Wat zit erin

35 skills, vier categorieën.

### Strategie (10)

`product-strategie` · `waardepropositie` · `positionering` · `north-star-metric` · `concurrentie-analyse` · `prijsstrategie` · `product-visie` · `verdienmodel` · `business-model-canvas` · `lean-canvas`

### Discovery (8)

`klantinterview` · `aannames-bedenken` · `experiment-ontwerp` · `doelgroepkeuze-primair` · `ideaal-klantprofiel` · `personas` · `klantreis` · `opportunity-solution-tree`

### Executie (11)

`prd-schrijven` · `stakeholder-map` · `pre-mortem` · `go-to-market` · `onderhandelen` · `user-stories` · `testscenarios` · `okrs-formuleren` · `wsjf-prioritering` · `outcome-roadmap` · `ideeen-bestaand-product`

### Analyse & groei (6)

`swot-analyse` · `metrics-dashboard` · `marketingideeen` · `retro` · `product-leadership-stances` · `ai-evals`

<details>
<summary>Alle skills met beschrijving</summary>

#### Strategie

| Skill | Wat het doet |
|-------|-------------|
| `product-strategie` | Product Strategy Canvas (9 secties), Seven Powers, Moat Statement |
| `waardepropositie` | Jobs to Be Done + FORCES Framework, Leverage Statement |
| `positionering` | Blue Ocean (ERRC Grid, Six Paths), Counter Positioning |
| `north-star-metric` | North Star Metric bepalen, sub-metrics, KPI-boom |
| `concurrentie-analyse` | Drie concurrenten diep in kaart, moat-analyse, relatieve positie |
| `prijsstrategie` | Modelkeuze, Van Westendorp, AI-kostenmodel |
| `product-visie` | Korte, begrijpelijke productvisie die intern richting geeft |
| `verdienmodel` | Zeven verdienmodellen, evaluatiematrix, validatie-experimenten |
| `business-model-canvas` | Osterwalder's negen bouwblokken, samenhang-checks |
| `lean-canvas` | Ash Maurya's negen blokken, aanname-identificatie |

#### Discovery

| Skill | Wat het doet |
|-------|-------------|
| `klantinterview` | The Mom Test + FORCES als vraagtechniek |
| `aannames-bedenken` | Twee paden (nieuw/bestaand), multi-perspectief, risico-prioritering |
| `experiment-ontwerp` | Pretotyping & A/B testing, YODA principle, success thresholds |
| `doelgroepkeuze-primair` | Vier criteria, smallest viable audience, gedragssegmentatie |
| `ideaal-klantprofiel` | Van beste klanten naar ICP statement, disqualificatie-criteria |
| `personas` | Patronen uit onderzoeksdata, JTBD-gestructureerd |
| `klantreis` | Zeven fasen (bewustwording tot aanbeveling), touchpoints, emoties |
| `opportunity-solution-tree` | Teresa Torres: outcome naar kansen naar oplossingen naar experimenten |

#### Executie

| Skill | Wat het doet |
|-------|-------------|
| `prd-schrijven` | Acht-sectie PRD met product-hypothese en aannames |
| `stakeholder-map` | Power x Interest grid met actiepunten per groep |
| `pre-mortem` | Tigers / Paper Tigers / Elephants risico-triage |
| `go-to-market` | FORCES per levenscyclusfase, StoryBrand messaging |
| `onderhandelen` | Tactical empathy, calibrated questions, Ackerman model (Chris Voss) |
| `user-stories` | 3 C's (Card, Conversation, Confirmation), INVEST check |
| `testscenarios` | Happy path, edge cases, foutafhandeling, Given/When/Then |
| `okrs-formuleren` | Doerr-style OKRs, van bedrijfsdoel naar team key results |
| `wsjf-prioritering` | WSJF-formule, vier scoringsdimensies, team-scoring |
| `outcome-roadmap` | Now/Next/Later + kwartaalformat, features naar outcomes |
| `ideeen-bestaand-product` | Multi-perspectief ideatie (PM/Designer/Engineer), scoring matrix |

#### Analyse & groei

| Skill | Wat het doet |
|-------|-------------|
| `swot-analyse` | Cross-referentie matrix, Seven Powers lens, aanbevelingen |
| `metrics-dashboard` | Metric-piramide (NSM naar input naar operationeel), alert-drempels |
| `marketingideeen` | Vijf concrete ideeën, owned/earned/paid, Nederlandse marktcontext |
| `retro` | Zes formats, auto-selectie op basis van situatie en teamdynamiek |
| `product-leadership-stances` | Diagnose misunderstood vs preferred stances, shift-advies |
| `ai-evals` | AI-kwaliteitsmeting en evaluatieframeworks |

</details>


## Waar beginnen

Kijk, dat hangt natuurlijk af van waar je nu staat en wat je daarbij nodig denkt te hebben.

**Je hebt een nieuw idee en wilt weten of het klopt.**
Begin met `aannames-bedenken` om te zien welke aannames eronder zitten. Daarna `experiment-ontwerp` om de riskantste te testen.

**Je weet niet precies voor wie je bouwt.**
Start met `doelgroepkeuze-primair` om segmenten te scoren op pijn, betalingsbereidheid en winbaarheid. Dan `klantinterview` om het te checken.

**Je zoekt strategische richting.**
`product-strategie` geeft je een compleet canvas. `positionering` scherpt je positie aan. `concurrentie-analyse` laat zien waar de ruimte zit.

**Je gaat in gesprek met klanten.**
`klantinterview` zorgt dat je de goede vragen stelt. Onthullend in plaats van sturend.

**Je moet iets opleveren aan engineering.**
`prd-schrijven` geeft je een structuur met aannames en hypotheses. Geen vage beschrijvingen.

**Je lanceert iets.**
`go-to-market` voor het plan. `waardepropositie` om je belofte scherp te krijgen.

**Je wilt weten wat er mis kan gaan.**
`pre-mortem` onderscheidt echte risico's van overschatte en onuitgesproken.


## Over mij

# Hoi, ik ben Stefan.

Ik doe aan product. Al meer dan tien jaar. Consultancy, trainingen, Coolblue, Postcodeloterij, Essent. Ik kon nooit veel. Met AI kan ik alles.

Ik bouw deze skills omdat ik ze zelf nodig heb. En uiteraard mag iedereen ze gebruiken. 

Ik ben dol op feedback dus voel je vrij mij te berichten.
[LinkedIn](https://linkedin.com/in/stefanwesemann) · [Substack](https://enenai.substack.com)


## Licentie

Apache 2.0. Vrij te gebruiken, ook commercieel.


## Bijdragen

Suggesties, verbeteringen en nieuwe skills zijn welkom. Open een issue of stuur een pull request. Twee eisen: Nederlands en kwalitatief. Zie [CONTRIBUTING.md](CONTRIBUTING.md) voor de details.
