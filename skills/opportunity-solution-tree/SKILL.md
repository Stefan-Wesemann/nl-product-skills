---
name: opportunity-solution-tree
description: "Bouw een Opportunity Solution Tree: van gewenst outcome naar ontdekte kansen, oplossingen en experimenten. Het kernframework voor continuous discovery."
triggers:
  - opportunity solution tree
  - ost
  - teresa torres
  - continuous discovery
  - discovery boom
  - oplossingen vinden
  - kansen identificeren
  - van outcome naar experiment
  - discovery structuur
---

# Opportunity Solution Tree

## Metadata

**Doel:** Structureer je discovery-werk in een boom: gewenst outcome bovenaan → ontdekte klantproblemen (opportunities) → mogelijke oplossingen → experimenten om te valideren. De OST voorkomt dat je direct van idee naar bouwen springt.

**Aanpak:** Top-down opbouwen vanuit één helder outcome. Per laag verdiepen met doorvragen en klantinzichten. Geen oplossingen bedenken zonder eerst de kansen te begrijpen.

**Output:** Visuele boomstructuur (tekst of diagram) met outcome, 3-5 kansen, 2-3 oplossingen per kans, en 1-2 experimenten per oplossing. Plus: prioritering welke tak je eerst valideert.

---

## Instructies

### Hoe de OST werkt — en hoe het zich verhoudt tot andere tools

De Opportunity Solution Tree is de ontdekking-structuur die verbindt WAT je wilt bereiken (outcome) met HOE je dat gaat ontdekken (experimenten). Het is geen meetinstrument (dat is de North Star Metric), geen aannames-lijst (dat is aannames-bedenken), en geen strategisch plan (dat is product-strategie).

De OST beantwoordt: **"Gegeven ons gewenste outcome, welke klantproblemen bestaan er, welke oplossingen zijn denkbaar, en hoe testen we die?"**

```
        [Gewenst Outcome]
        /       |        \
  [Kans 1]  [Kans 2]  [Kans 3]
   /    \      |         /   \
[Opl A] [Opl B] [Opl C] [Opl D] [Opl E]
  |       |       |       |       |
[Exp 1] [Exp 2] [Exp 3] [Exp 4] [Exp 5]
```

**Wanneer gebruik je de OST?**
- Je weet WAT je wilt verbeteren (outcome) maar niet HOE
- Je hebt te veel ideeën en geen structuur om te kiezen
- Je team springt steeds naar oplossingen zonder het probleem te begrijpen
- Je wilt discovery-werk zichtbaar en bespreekbaar maken

**Wanneer NIET?**
- Je weet al precies wat je moet bouwen (ga naar prd-schrijven)
- Je hebt nog geen outcome gedefinieerd (ga naar north-star-metric)
- Je wilt aannames valideren die je al hebt (ga naar experiment-ontwerp)

---

### Fase 0: Context ophalen

**Stap 1 — Check wat er al is**
Scan uploads, gedeelde mappen en workspace op relevante bestanden (eerdere outputs, research, data). Lees ze door.

**Stap 2 — Slimme vragen stellen**
- **Wel context gevonden →** Bevestig kort wat je ziet ("Ik zie [X], klopt dat?"). Stel alleen vragen over wat je nog mist.
- **Geen context →** Stel onderstaande vragen.

1. **Het outcome**: Wat is het gewenste resultaat dat je wilt bereiken? (Liefst meetbaar, gekoppeld aan je North Star of team-OKR)
2. **Outcome-scherpte**: Is dit outcome echt meetbaar en eenduidig? Kan je team het in één zin uitleggen? Als het outcome vaag is, ga eerst terug naar north-star-metric of okrs-formuleren.
3. **De context**: Is dit een nieuw productgebied of een bestaand onderdeel dat je wilt verbeteren?
4. **Bestaande kennis**: Heb je al klantinterviews gedaan? Data-inzichten? Support tickets? Hoeveel directe klantinteractie heb je gehad in de afgelopen 4 weken?
5. **Het team**: Wie werkt hier aan? PM, Design, Engineering? Doe je dit alleen of samen?
6. **Bestaande ideeën**: Zijn er al oplossingen waar het team verliefd op is? (Dit is belangrijk om te weten — de OST helpt juist om niet te snel naar oplossingen te springen.)

Ga pas verder als je het outcome scherp hebt. Een vage outcome levert een vage boom.

---

## Laag 1: Het Gewenste Outcome

Het outcome is de top van je boom. Dit is NIET een feature of oplossing. Het is het resultaat dat je wilt zien.

**Goede outcomes:**
- "Verhoog het percentage gebruikers dat binnen 7 dagen terugkeert van 25% naar 40%"
- "Verlaag de gemiddelde tijd tot eerste waarde van 12 naar 4 minuten"
- "Verhoog de NPS van enterprise-klanten van 32 naar 50"

**Slechte outcomes:**
- "Bouw een dashboard" (dat is een oplossing)
- "Verbeter de gebruikerservaring" (te vaag om te meten)
- "Meer omzet" (te breed, niet klantgericht)

**Doorvragen:**
- "Hoe weet je dat dit het juiste outcome is? Waar komt het vandaan?"
- "Hoe meet je dit vandaag? Wat is de huidige waarde?"
- "Waarom is dit outcome nu prioriteit en niet iets anders?"
- "Als dit outcome verbetert, wat verandert er dan voor de klant? En voor het bedrijf?"

**Rode vlag:** Als je het outcome niet in één zin kunt uitleggen, is het niet scherp genoeg.

---

## Laag 2: Kansen (Opportunities)

Kansen zijn **klantproblemen, behoeften of verlangens** die je hebt ontdekt. Ze komen uit interviews, data, support tickets — niet uit je eigen hoofd.

**Belangrijk:** Kansen zijn geformuleerd vanuit de klant, niet vanuit jouw product.

**Goed:**
- "Gebruikers raken gedemotiveerd als ze na aanmelding niet weten wat de eerste stap is"
- "Teamleads willen zien wat hun team heeft bereikt, maar moeten nu handmatig rapportages maken"
- "Klanten vergelijken ons met concurrent X maar snappen niet waarin we anders zijn"

**Fout:**
- "We moeten onboarding verbeteren" (dat is een oplossing, geen kans)
- "De conversie is laag" (dat is een metric, geen klantprobleem)

### Hoe je kansen ontdekt

**Uit klantinterviews (primair):**
- Gebruik je klantinterview-skill voor gestructureerde gesprekken
- Let op: wat zeggen ze dat frustrerend is? Waar verliezen ze tijd? Wat probeerden ze al?
- Eén interview levert vaak 3-5 kansen op

**Uit data:**
- Waar vallen gebruikers af in je funnel?
- Welke features worden gestart maar niet afgemaakt?
- Waar komen support tickets het meest over?

**Uit support en feedback:**
- Welke klachten komen steeds terug?
- Welke feature requests verbergen een dieper probleem?

### Structureer je kansen

Groepeer verwante kansen. Je wilt 3-5 kansen op het eerste niveau, elk met eventueel sub-kansen.

```
[Outcome: Verhoog retentie van 25% naar 40%]
├── Kans 1: Nieuwe gebruikers weten niet wat ze eerst moeten doen
│   ├── Sub: Ze begrijpen de interface niet
│   └── Sub: Ze zien de waarde pas na 3 sessies
├── Kans 2: Gebruikers die stoppen zeggen dat het "te veel tijd kost"
│   ├── Sub: De dagelijkse workflow heeft te veel stappen
│   └── Sub: Ze moeten steeds dezelfde informatie opnieuw invoeren
└── Kans 3: Teamleads zien geen waarde voor het team als geheel
    └── Sub: Individueel nuttig, maar geen team-voordeel zichtbaar
```

**Doorvragen per kans:**
- "Hoeveel klanten noemden dit? Is het een patroon of een eenling?"
- "Hoe groot is de impact als we dit oplossen? Op retentie? Op tevredenheid?"
- "Is dit een probleem voor al onze gebruikers of voor een specifiek segment?"

---

## Laag 3: Oplossingen

Per kans bedenk je 2-3 mogelijke oplossingen. Dit is het moment om creatief te zijn — maar altijd gekoppeld aan een specifieke kans.

**Regels:**
- Elke oplossing hoort bij precies één kans
- Bedenk minimaal 2 oplossingen per kans (voorkom dat je verliefd wordt op je eerste idee)
- Oplossingen variëren in grootte: van klein experiment tot grote feature
- Betrek Design en Engineering bij het bedenken

**Voorbeeld:**

```
Kans: Nieuwe gebruikers weten niet wat ze eerst moeten doen

├── Oplossing A: Interactieve onboarding-wizard (3 stappen)
├── Oplossing B: Persoonlijke welkomstmail met één specifieke eerste actie
└── Oplossing C: Lege-staat-scherm met voorbeelddata die je kunt verkennen
```

**Doorvragen per oplossing:**
- "Lost dit de kans echt op, of is het een pleister?"
- "Hoe complex is dit om te bouwen? Wat is de kleinste versie?"
- "Hebben concurrenten dit al geprobeerd? Wat werkte wel/niet?"
- "Wat zou de klant hiervan vinden als je het voorlegt?"

**Veelgemaakte fout:** Oplossingen bedenken zonder kansen. Als je merkt dat je een oplossing hebt die niet bij een kans past, vraag je af: "Welk klantprobleem lost dit op?" Als je dat niet kunt beantwoorden, schrap de oplossing.

---

## Laag 4: Experimenten

Per oplossing definieer je 1-2 experimenten om te testen of de oplossing werkt — VOORDAT je hem volledig bouwt.

**Types experimenten (van klein naar groot):**

| Type | Wat | Wanneer | Duur |
|---|---|---|---|
| **Interview** | Leg de oplossing voor aan 5 klanten, vraag reactie | Vroege fase | 1 week |
| **Prototype-test** | Clickable prototype, observeer gedrag | Oplossing visueel te maken | 1-2 weken |
| **Concierge** | Jij voert de oplossing handmatig uit voor de klant | Complexe oplossing, weinig dev-tijd | 1-2 weken |
| **Wizard of Oz** | Front-end bestaat, backend is handmatig | Testen of klanten het gebruiken | 2-3 weken |
| **Fake door** | Knop/pagina die er is maar nog niets doet, meet interesse | Demand testen | Dagen |
| **A/B-test** | Twee varianten live, meet verschil | Bestaand product, genoeg traffic | 2-4 weken |

**Per experiment definieer je:**
1. **Wat test je?** (de aanname achter de oplossing)
2. **Hoe meet je succes?** (concrete metric + drempelwaarde)
3. **Hoeveel tijd/resources kost het?**
4. **Wat doe je met het resultaat?** (als positief → bouwen / als negatief → volgende oplossing)

**Voorbeeld:**

```
Oplossing: Interactieve onboarding-wizard

Experiment 1: Prototype-test
- Aanname: "Gebruikers die een wizard doorlopen, begrijpen sneller wat de eerste stap is"
- Metric: Tijd tot eerste kernactie < 4 minuten (nu: 12 minuten)
- Resources: 1 week design, 5 testgebruikers
- Bij succes: Bouwen in volgende sprint
- Bij falen: Test oplossing B (welkomstmail)
```

---

## Prioritering: Welke Tak Eerst?

Je kunt niet alles tegelijk valideren. Prioriteer op basis van:

1. **Impact op outcome**: welke kans heeft de meeste invloed op je gewenste resultaat?
2. **Bewijs**: voor welke kans heb je het meeste bewijs uit interviews/data?
3. **Snelheid van leren**: welk experiment levert het snelst inzicht op?

**Praktijk:** Kies één tak (kans → oplossing → experiment) om deze week mee te starten. Niet drie tegelijk.

**Doorvragen:**
- "Als je maar één kans mocht aanpakken dit kwartaal — welke zou het meeste verschil maken?"
- "Voor welke kans heb je het meeste bewijs? En voor welke het minste?" (minste bewijs = misschien eerst valideren)
- "Welk experiment kun je morgen al starten?"

---

## De OST Levend Houden

De boom is geen eenmalig document. Zo houd je hem actueel:

- **Na elk klantinterview:** Voeg nieuwe kansen toe, verplaats of verwijder kansen die niet kloppen
- **Na elk experiment:** Markeer welke oplossingen gevalideerd/ontkracht zijn
- **Wekelijks met je team:** Loop de boom door — zijn we nog op de juiste tak?
- **Per kwartaal:** Heroverweeg het outcome. Is het nog relevant?

**Tip:** Hang de boom fysiek op (whiteboard) of gebruik een tool als Miro/FigJam. Een boom die niemand ziet, wordt niet gebruikt.

---

## Output

Lever het volgende op:

1. **Gewenst outcome** — scherp, meetbaar, in één zin
2. **Opportunity-boom** — 3-5 kansen, elk met 2-3 oplossingen, elk met 1-2 experimenten
3. **Prioritering** — welke tak ga je eerst valideren en waarom
4. **Eerste experiment** — concreet gedefinieerd (aanname, metric, resources, tijdlijn)
5. **Open vragen** — wat weet je nog niet en hoe ga je dat ontdekken

---

## Veel Voorkomende Fouten

- **Oplossingen als kansen formuleren** — "we moeten de onboarding verbeteren" is geen kans. "Gebruikers haken af omdat ze niet weten wat ze moeten doen" is een kans
- **Kansen bedenken in plaats van ontdekken** — de boom vul je met inzichten uit interviews en data, niet met aannames uit je eigen hoofd
- **Verliefd worden op één oplossing** — daarom minimaal 2 per kans. Je eerste idee is zelden het beste
- **Te veel takken tegelijk aanpakken** — focus op één tak, valideer, leer, dan volgende
- **De boom één keer maken en vergeten** — het is een levend document, niet een eenmalige exercise
- **Outcome te vaag houden** — "gebruikerservaring verbeteren" stuurt niets. Maak het meetbaar
- **Experimenten overslaan** — direct bouwen zonder te testen is de duurste manier om erachter te komen dat je fout zat

---

## Bronnen

- Teresa Torres — *Continuous Discovery Habits* (2021) — het standaardwerk over de OST
- Marty Cagan — *Inspired* en *Empowered* — product discovery principes
- Product Faculty — Leverage Discovery — hypothese-driven discovery
- Jeff Patton — *User Story Mapping* — verwant framework voor het structureren van gebruikersbehoeften
