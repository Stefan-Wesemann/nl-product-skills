# 🇳🇱 NL Product Skills

Eigenlijk liep ik er steeds tegenaan. Ik vroeg AI om hulp bij productwerk en kreeg antwoorden die... oké waren. Generiek. Een beetje alsof je een stagiair vraagt om een concurrentieanalyse en je krijgt een samenvatting van de Wikipedia-pagina terug. Niet fout, maar ook niet bruikbaar.

Dus heb ik frameworks die ik jarenlang heb gebruikt (FORCES, Blue Ocean, The Mom Test) vastgelegd op een manier die AI begrijpt. Nederlandstalig, met Nederlandse context, geen vertalingen van Engelstalige templates. Het resultaat: een AI-assistent die doorvraagt in plaats van een generiek lijstje teruggeeft.

## Over mij

Stefan Wesemann. 10+ jaar productervaring bij onder andere Coolblue, Essent en Postcodeloterij. PSPO III gecertificeerd, MIT "Designing and Building AI Products", Product Faculty "AI Product Strategy". Ik gebruik AI dagelijks in mijn werk en deel wat ik leer.

[LinkedIn](https://linkedin.com/in/stefanwesemann) · [Afkijken (Substack)](https://afkijken.substack.com)

## Wat dit anders maakt

De meeste AI-skills geven je een snel antwoord. Je stelt een vraag, je krijgt een lijstje. Klaar.

Deze skills doen dat niet. Ze stellen eerst vragen. Over jouw situatie, jouw klant, jouw markt. Pas als er genoeg context is, komt het resultaat. Het duurt langer. Het resultaat is beter.

Een voorbeeld. Je vraagt de klantinterview skill om een interviewscript. In plaats van een standaardlijstje krijg je eerst vragen: wie is je doelgroep, in welke fase zit je, wat heb je al gehoord in eerdere gesprekken? Op basis daarvan krijg je een script met doorvraagtechnieken op basis van The Mom Test en FORCES. Zodat je de juiste vragen stelt in plaats van de vragen waarvan je hoopt dat het antwoord ja is.

Dat is het verschil. Proces over inhoud. De inhoud wordt beter omdat het proces beter is.

## Waar begin je?

Niet zeker welke skill je nodig hebt? Dit helpt.

**Je hebt een idee en wilt weten of het wat is.** Start met `aannames-bedenken`. Kijk welke aannames er onder je idee zitten. Ga dan naar `experiment-ontwerp` om de riskantste aanname te testen.

**Je weet niet precies voor wie je bouwt.** Begin bij `doelgroepkeuze-primair`. Scoor je segmenten op pijn, betalingsbereidheid en winbaarheid. Gebruik dan `klantinterview` om te checken of je gelijk hebt.

**Je moet je strategie op papier krijgen.** `product-strategie` geeft je het volledige canvas. Scherper op positionering? `positionering`. Op verdedigbaarheid? `concurrentie-analyse`.

**Je gaat een klantgesprek voeren.** `klantinterview`. Zodat je de juiste vragen stelt in plaats van de vragen die je wilt horen.

**Je moet een feature specificeren voor je team.** `prd-schrijven`. Acht secties, met producthypothese en aannames. Geen vage beschrijving maar een scherp document.

**Je lanceert iets.** `go-to-market` voor het plan. `waardepropositie` als je nog scherper wilt formuleren wat je belooft.

**Je wilt weten wat er mis kan gaan.** `pre-mortem`. Bedenk voor de lancering wat mislukt en waarom. Tigers, Paper Tigers en Elephants. Zodat je weet wat je echt moet fixen en wat je kunt laten liggen.

## Skills

### Strategie

| Skill | Wat het doet |
|---|---|
| `product-strategie` | Product Strategy Canvas (9 secties), Seven Powers, Moat Statement |
| `waardepropositie` | JTBD + FORCES Framework (6 krachten), Leverage Statement |
| `positionering` | Blue Ocean (ERRC Grid, Six Paths), Counter Positioning |
| `north-star-metric` | North Star Metric, sub-metrics, KPI-boom |
| `concurrentie-analyse` | 3 concurrenten diep, moat-analyse, relatieve positie |
| `prijsstrategie` | Modelkeuze, Van Westendorp, AI-kostenmodel |
| `product-visie` | Korte, begrijpbare productvisie. Intern gericht |

### Discovery

| Skill | Wat het doet |
|---|---|
| `klantinterview` | The Mom Test + FORCES als doorvraag-lens |
| `aannames-bedenken` | Twee paden (nieuw/bestaand), multi-perspectief, Leverage hypotheses |
| `experiment-ontwerp` | Pretotyping & A/B tests, YODA principle, success thresholds |
| `doelgroepkeuze-primair` | 4 criteria, smallest viable audience, gedragssegmentatie |

### Executie

| Skill | Wat het doet |
|---|---|
| `prd-schrijven` | 8-sectie PRD, producthypothese, aannames, AI-checklist |
| `stakeholder-map` | Mapping + prioritering, Power × Interest grid |
| `pre-mortem` | Tigers / Paper Tigers / Elephants, risico-triage |
| `go-to-market` | FORCES per levenscyclusfase, StoryBrand messaging, STEPPS |

### Analyse

| Skill | Wat het doet |
|---|---|
| `swot-analyse` | Gerichte vragen, cross-referentie matrix, Seven Powers lens |

## Hoe werkt het

Elke skill is een `SKILL.md` bestand. Dat is een document met instructies dat je AI-assistent automatisch oppikt en volgt wanneer het relevant is.

Het verschil met een gewone prompt: een skill vraagt door. Je krijgt geen standaardantwoord maar een gesprek. De skill stelt gerichte vragen over jouw situatie, jouw klant, jouw markt. Pas als het genoeg context heeft, komt het resultaat. Dat is waarom het beter werkt dan "schrijf mij een productstrategie" in ChatGPT typen.

Je vraagt om een productstrategie, de `product-strategie` skill wordt geladen. Je wilt een klantinterview voorbereiden, de `klantinterview` skill wordt geactiveerd. Skills staan los van elkaar. Geen afhankelijkheden. Je kunt ze individueel gebruiken.

## Installatie

### Claude Code

```bash
claude plugin marketplace add SedanWeerman/nl-product-skills
claude plugin install nl-product-skills
```

### Claude Cowork / Claude.ai

Upload individuele `SKILL.md` bestanden als custom skills via de instellingen.

### Cursor / Copilot / andere AI-assistenten

Kopieer de `skills/` map naar je project of global skills directory. De bestanden volgen de Agent Skills open standaard en werken cross-platform.

## Frameworks en bronnen

Deze skills bouwen voort op:

- **FORCES Framework** (Product Faculty) voor gedragsverandering
- **Seven Powers** (Hamilton Helmer) voor verdedigbare voordelen
- **Blue Ocean Strategy** (Kim & Mauborgne) voor positionering
- **The Mom Test** (Rob Fitzpatrick) voor klantinterviews zonder bias
- **JTBD** (Clayton Christensen) voor waardepropositie vanuit klantperspectief
- **StoryBrand** (Donald Miller) voor messaging
- **Contagious STEPPS** (Jonah Berger) voor viraliteit
- **AI Product Design** (MIT xPRO) voor UX-principes bij AI-producten

## Licentie

Apache 2.0. Vrij te gebruiken, ook commercieel.

## Bijdragen

Suggesties, verbeteringen en nieuwe skills zijn welkom. Open een issue of stuur een pull request. Houd de taal Nederlands en de kwaliteit hoog.
