---
name: personas
description: "Ontwikkel onderbouwde persona's uit onderzoeksdata. Geen fictieve profielen maar patronen uit echte interviews, data en observatie."
triggers:
  - persona
  - personas
  - user persona
  - gebruikersprofiel
  - doelgroepprofiel
  - wie is onze gebruiker
  - klantprofiel
  - persona ontwikkelen
  - persona's maken
---

# Persona's

## Metadata

**Doel:** Maak persona's die je team helpt om ontwerpbeslissingen te nemen vanuit het perspectief van de gebruiker. Geen fictieve profielfoto's met willekeurige namen, maar gestructureerde patronen uit echt onderzoek.

**Verschil met Ideal Customer Profile (ICP):**
- **ICP** = wie is onze ideale *klant* op bedrijfs-/koperniveau → gericht op acquisitie en sales ("dit type bedrijf met deze kenmerken koopt het snelst")
- **Persona** = wie is de *gebruiker* als mens → gericht op productontwerp ("zo denkt en werkt deze persoon, zo ontwerpen we voor hen")
- Bij B2B heb je vaak beide: ICP bepaalt op WIE je richt, persona's bepalen HOE je bouwt
- Bij B2C is er meer overlap en kun je vaak met persona's volstaan

**Aanpak:** Patronen destilleren uit klantinterviews, support data en gedragsinzichten. Persona's zijn hypotheses — je valideert en itereert ze.

**Output:** 2-3 persona's met JTBD, gedragspatronen, frustraties en context. Plus: primaire persona-keuze met rationale.

---

## Instructies

### Fase 0: Context ophalen

**Stap 1 — Check wat er al is**
Scan uploads, gedeelde mappen en workspace op relevante bestanden (eerdere outputs, research, data). Lees ze door.

**Stap 2 — Slimme vragen stellen**
- **Wel context gevonden →** Bevestig kort wat je ziet ("Ik zie [X], klopt dat?"). Stel alleen vragen over wat je nog mist.
- **Geen context →** Stel onderstaande vragen.

1. **Beschikbare data**: Heb je klantinterviews gedaan? Hoeveel? Met wie?
2. **Andere bronnen**: Heb je support tickets, NPS-data, analytics, of feedback die we kunnen gebruiken?
3. **Bestaande persona's**: Zijn er al persona's? Zo ja, wat klopt er niet meer aan?
4. **Product**: Wat is het product en wie gebruikt het nu?
5. **Doel**: Waarvoor ga je de persona's gebruiken? Productontwerp, onboarding, marketing, of iets anders?
6. **Scope**: Gaat het om alle gebruikers of een specifiek deel? (bijv. alleen nieuwe gebruikers, of alleen admin-rollen)

**Belangrijk:** Persona's zonder onderzoeksdata zijn fictie. Als er geen interviews of data zijn, begin dan bij de klantinterview-skill en kom hier terug.

---

## Wat een Goede Persona WEL en NIET Is

### Een goede persona:
- Is gebaseerd op patronen uit meerdere interviews (niet één persoon)
- Beschrijft gedrag en motivatie, niet alleen demografie
- Helpt je team om "nee" te zeggen tegen features die niet voor deze persona zijn
- Verandert mee als je meer leert

### Een slechte persona:
- Is verzonnen op basis van aannames ("vast wel zo")
- Focust op leeftijd, hobby's en een stockfoto
- Is zo breed dat iedereen erin past
- Hangt in een la en wordt nooit gebruikt

---

## Stap 1: Patronen Herkennen uit Onderzoek

Loop je beschikbare data door en zoek naar **clusters van vergelijkbaar gedrag**.

**Groepeer op:**
- **Gedrag**: Hoe gebruiken ze het product? Dagelijks, wekelijks, ad hoc?
- **Motivatie**: Waarom gebruiken ze het? Wat is hun Job to Be Done?
- **Frustratie**: Waar lopen ze tegenaan? Wat kost ze tijd/moeite?
- **Context**: In welke situatie gebruiken ze het? Alleen, in teamverband, onder tijdsdruk?
- **Expertise**: Hoe ervaren zijn ze met dit type tool/proces?

**Voorbeeld van patronen:**
```
Patroon A: Gebruikt het product dagelijks, kent alle features,
           frustratie zit in gebrek aan geavanceerde opties
           → Power user

Patroon B: Gebruikt het product 1x per week, alleen de basisfuncties,
           frustratie zit in dat het "te ingewikkeld" voelt
           → Casual user

Patroon C: Gebruikt het product niet zelf, maar moet resultaten
           beoordelen die anderen ermee maken
           → Beslisser/stakeholder
```

**Doorvragen:**
- "Welke gedragspatronen zag je steeds terugkomen in interviews?"
- "Waren er mensen die het product heel anders gebruikten dan verwacht?"
- "Welke groep had de meeste frustratie? Welke de meeste tevredenheid?"

---

## Stap 2: Persona-Profiel Opbouwen

Per geïdentificeerd patroon bouw je een persona op. Gebruik deze structuur:

### Identiteit

- **Naam**: Een herkenbare naam die het team gaat gebruiken (geen stockfoto-naam, maar iets dat het patroon typeert)
- **Rol/functie**: Wat doen ze voor werk?
- **Context**: In welk type organisatie, team, situatie zitten ze?
- **Ervaring**: Hoe ervaren zijn ze in hun vakgebied en met dit type tooling?

### Jobs to Be Done

Dit is de kern. Niet wat ze WILLEN, maar wat ze proberen GEDAAN te krijgen.

**Formuleer als:**
- **Primaire JTBD**: "Wanneer [situatie], wil ik [motivatie], zodat ik [gewenst resultaat]"
- **Gerelateerde jobs**: Welke andere taken hangen hiermee samen?
- **Emotionele job**: Hoe willen ze zich voelen? (Competent, in controle, ontlast)
- **Sociale job**: Hoe willen ze gezien worden? (Door team, door leidinggevende)

**Voorbeeld:**
```
Primaire JTBD: "Wanneer ik een sprintplanning voorbereid, wil ik
snel zien welke items het meeste impact hebben, zodat ik het team
kan focussen op wat er echt toe doet."

Emotionele job: "Ik wil me voorbereid en competent voelen in het
planning-overleg, niet verrast worden door vragen die ik niet
kan beantwoorden."

Sociale job: "Ik wil dat mijn team vertrouwen heeft in mijn
prioriteringsbeslissingen."
```

### Gedrag en Gewoonten

- **Frequentie**: Hoe vaak hebben ze met dit probleem/product te maken?
- **Workflow**: Hoe ziet hun huidige werkwijze eruit, stap voor stap?
- **Tools**: Welke tools gebruiken ze nu? Wat werkt, wat niet?
- **Beslisgedrag**: Hoe kiezen ze nieuwe tools? Zelf, in teamverband, via manager?

### Frustraties en Pijnpunten

- **Primaire frustratie**: Het grootste pijnpunt gerelateerd aan het probleem
- **Secundaire frustraties**: Wat maakt het erger?
- **Workarounds**: Wat hebben ze zelf bedacht om het probleem te omzeilen?
- **Consequenties**: Wat kost het ze als het probleem niet opgelost wordt? (tijd, geld, stress)

### Behoeften en Verwachtingen

- **Must-haves**: Zonder dit overwegen ze je product niet
- **Nice-to-haves**: Dit maakt het verschil maar is niet dealbreaker
- **Dealbreakers**: Hierdoor haken ze direct af

### Citaten

Pak 2-3 letterlijke citaten uit interviews die deze persona typeren. Echte woorden zijn krachtiger dan samenvatting.

```
"Ik besteed elke maandag 2 uur aan het bijwerken van mijn
spreadsheet. Dat is werk dat niemand ziet maar dat wel moet gebeuren."

"Als ik een nieuwe tool voorstel aan mijn team, moet het binnen
5 minuten duidelijk zijn wat het doet. Anders haken ze af."
```

---

## Stap 3: Primaire Persona Kiezen

Je hebt 2-3 persona's. Kies er één als primaire persona — de persona voor wie je in eerste instantie ontwerpt.

**Criteria:**
- Grootste overlap met je doelgroep/ICP
- Meeste pijn (burning pain)
- Best bereikbaar (kanalen, netwerk)
- Meeste groeipotentieel (als je deze groep wint, opent dat andere segmenten)

**Doorvragen:**
- "Als je product maar voor één van deze persona's perfect zou werken — wie kies je?"
- "Welke persona zou het snelst betalen?"
- "Welke persona zou het product het vaakst aanraden?"

**Voorbeeld:**
```
Primaire persona: "Lisa de Hands-on PM"
Rationale: Grootste pijn (besteedt 4+ uur/week aan handmatig werk),
betaalt uit eigen toolbudget, zit in actieve PM-communities.
Als we haar winnen, wordt ze onze ambassadeur.

Secundaire persona: "Mark de Stakeholder"
Reden: Moet de output begrijpen, maar is niet de dagelijkse gebruiker.
We ontwerpen niet primair voor hem, maar houden zijn behoeften
in de gaten (output moet stakeholder-ready zijn).
```

---

## Stap 4: Persona Valideren

Een persona is een hypothese. Valideer hem:

1. **Toets bij het team**: Herkennen Design, Engineering en Sales deze persona?
2. **Toets bij klanten**: Laat de persona zien aan 2-3 klanten. Herkennen ze zichzelf?
3. **Toets tegen data**: Kloppen de gedragspatronen met wat je in analytics ziet?
4. **Herzie na 5 nieuwe interviews**: Past de persona nog of moet je bijstellen?

**Rode vlaggen dat je persona niet klopt:**
- Niemand in je team kan een echte klant noemen die op de persona lijkt
- De persona beschrijft een gemiddelde in plaats van een patroon
- Je kunt niet uitleggen waarin persona A verschilt van persona B

---

## Output

Lever het volgende op:

1. **2-3 persona-profielen** — elk met identiteit, JTBD, gedrag, frustraties, behoeften en citaten
2. **Primaire persona-keuze** — met rationale waarom deze persoon voorrang krijgt
3. **Onderscheidende kenmerken** — hoe verschillen de persona's van elkaar in gedrag en motivatie
4. **Validatie-plan** — hoe ga je checken of deze persona's kloppen
5. **Relatie met ICP** — als relevant: hoe verhoudt de persona zich tot het bedrijfsprofiel dat je target

---

## Veel Voorkomende Fouten

- **Persona's maken zonder onderzoek** — een verzonnen persona is erger dan geen persona, want het voelt alsof je klanten begrijpt terwijl dat niet zo is
- **Focussen op demografie** — leeftijd, woonplaats en hobby's zeggen niets over productgedrag. Focus op motivatie, frustratie en context
- **Te veel persona's** — 5+ persona's = je ontwerpt voor niemand. Houd het bij 2-3
- **Geen primaire persona kiezen** — als je voor iedereen ontwerpt, ontwerp je voor niemand
- **Persona's maken en dan vergeten** — ze moeten terugkomen in elke design review, elke user story, elke prioriteringsbeslissing
- **Persona met persona verwarren** — het gaat niet om een fictief karakter maar om een gedragspatroon
- **ICP en persona door elkaar gebruiken** — ICP = wie koopt, persona = wie gebruikt. Bij B2B zijn dat vaak verschillende mensen

---

## Bronnen

- Alan Cooper — *About Face* — het standaardwerk over persona's
- Teresa Torres — *Continuous Discovery Habits* — persona's in continuous discovery
- Kim Goodwin — *Designing for the Digital Age* — persona-methoden
- Product Faculty — FORCES Framework — begrijpen waarom persona's wel/niet veranderen
- Indi Young — *Mental Models* — gedragspatronen als basis voor persona's
