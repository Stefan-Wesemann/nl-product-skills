---
name: outcome-roadmap
description: "Transformeer een featurelijst naar een outcome-gerichte roadmap. Kies tussen Now/Next/Later of kwartaalindeling op basis van je situatie."
triggers:
  - roadmap
  - outcome roadmap
  - product roadmap
  - now next later
  - kwartaalplanning
  - roadmap maken
  - productplanning
  - roadmap schrijven
  - feature roadmap omzetten
---

# Outcome Roadmap

## Metadata

**Doel:** Maak een roadmap die communiceert WELKE resultaten je nastreeft — niet welke features je bouwt. Een outcome-roadmap geeft stakeholders richting zonder je te committen aan specifieke oplossingen die kunnen veranderen.

**Twee formats:**
- **Now / Next / Later** → wanneer je flexibel wilt blijven en niet aan kwartalen gebonden bent
- **Kwartaalindeling** → wanneer stakeholders of het bedrijf kwartaalplanning verwacht

**Aanpak:** Begin bij de bestaande featurelijst of roadmap. Herformuleer features als outcomes. Groepeer en prioriteer. Kies het format dat past bij je organisatie.

**Output:** Outcome-roadmap in gekozen format, met per outcome de rationale en mogelijke oplossingsrichtingen.

---

## Instructies

### Fase 0: Context ophalen

**Stap 1 — Check wat er al is**
Scan uploads, gedeelde mappen en workspace op relevante bestanden (eerdere roadmaps, feature-backlogs, strategische documenten, OKRs). Lees ze door.

**Stap 2 — Slimme vragen stellen**
- **Wel context gevonden →** Bevestig kort wat je ziet ("Ik zie [X], klopt dat?"). Stel alleen vragen over wat je nog mist.
- **Geen context →** Stel onderstaande vragen.

---

1. **Huidige roadmap**: Heb je al een roadmap? Zo ja, is het een featurelijst of al outcome-gericht?
2. **Publiek**: Wie leest deze roadmap? (Engineering, stakeholders, C-level, klanten?)
3. **Strategische context**: Wat zijn de bedrijfsdoelen of OKRs dit kwartaal/jaar?
4. **Format-voorkeur**: Wil je Now/Next/Later of kwartaalindeling?
5. **Tijdshorizon**: Hoever vooruit plan je? (3 maanden, 6 maanden, jaar?)
6. **Input**: Heb je een backlog, feature requests, of strategische thema's als input?

---

## Features vs. Outcomes

Dit is het kernonderscheid. Een feature-roadmap zegt WAT je bouwt. Een outcome-roadmap zegt WAAROM.

| Feature-roadmap | Outcome-roadmap |
|---|---|
| "Bouw notificatiesysteem" | "Gebruikers missen geen belangrijke updates meer" |
| "Voeg SSO toe" | "Enterprise-klanten kunnen veilig en snel inloggen" |
| "Redesign dashboard" | "Gebruikers vinden in 10 seconden wat ze zoeken" |
| "Integratie met Slack" | "Teams ontvangen inzichten in hun bestaande workflow" |

**Het verschil:** Een feature verandert niet meer als je hem hebt afgesproken. Een outcome laat ruimte voor de beste oplossing — misschien is de integratie met Slack niet de beste manier, maar een dagelijkse email-samenvatting wel.

### Hoe je een feature herformuleert als outcome

**Stap 1:** Neem de feature
**Stap 2:** Vraag "Waarom willen we dit?" (het antwoord = het echte doel)
**Stap 3:** Vraag "Hoe weten we dat het gelukt is?" (het antwoord = de metric)
**Stap 4:** Formuleer als: "[Doelgroep] [bereikt resultaat], gemeten door [metric]"

**Voorbeeld:**
```
Feature: "Bouw een dashboard met real-time metrics"

Waarom? → PM's willen snel zien hoe het product presteert
Metric? → Tijd om antwoord op een datavraag te vinden
Outcome: "PM's vinden antwoord op hun datavraag binnen 30 seconden
          (nu: 5+ minuten in spreadsheets)"
```

---

## Format 1: Now / Next / Later

**Wanneer gebruiken:** Startups, teams met korte cycli, of wanneer je niet aan kwartalen gebonden wilt zijn. Geeft flexibiliteit om te verschuiven.

### Structuur

**Now (nu bezig, dit moment)**
- Items waar je team actief aan werkt
- Hoog detail: outcome + gekozen oplossingsrichting
- Tijdshorizon: deze sprint / komende 2-4 weken
- Maximum: 2-3 items (meer = geen focus)

**Next (daarna, in de pijplijn)**
- Items die je hebt gevalideerd en klaarstaan om op te pakken
- Middel detail: outcome + mogelijke oplossingsrichtingen
- Tijdshorizon: komende 1-3 maanden
- Maximum: 3-5 items

**Later (toekomst, op de radar)**
- Items die je wilt verkennen maar nog niet gevalideerd hebt
- Laag detail: outcome + open vragen
- Tijdshorizon: 3-6 maanden+
- Maximum: 5-8 items

**Voorbeeld:**

```
NOW
├── Nieuwe gebruikers ervaren kernwaarde in eerste sessie
│   Metric: Time-to-value < 5 min (nu: 12 min)
│   Richting: Onboarding wizard + voorbeelddata
│
└── Enterprise-klanten beheren teamtoegang zelf
    Metric: 0 support tickets over access management
    Richting: Admin-panel met RBAC

NEXT
├── Teams delen inzichten zonder extra stappen
│   Metric: % teams dat wekelijks deelt > 40%
│   Richtingen: Slack-integratie OF email-digest OF in-app delen
│
└── Power users automatiseren repetitieve taken
    Metric: Uren bespaard per gebruiker per week > 2
    Open: Nog valideren welke taken het meest repetitief zijn

LATER
├── Klanten in reguleerde sectoren voldoen aan compliance-eisen
│   Open: Welke sectoren? Welke eisen precies?
│
└── Internationaal: product bruikbaar voor niet-NL markt
    Open: Welke markt eerst? Wat moet er lokaliseren?
```

---

## Format 2: Kwartaalindeling

**Wanneer gebruiken:** Organisaties met kwartaalplanning, OKR-cycli, of stakeholders die een tijdlijn verwachten.

### Structuur

Per kwartaal:
- **Thema**: Overkoepelend thema dat de outcomes verbindt
- **2-3 outcomes**: Wat willen we bereiken dit kwartaal?
- **Per outcome**: Metric + mogelijke oplossingsrichtingen
- **Afhankelijkheden**: Wat moet er eerst? Waar hangen we van af?

**Voorbeeld:**

```
Q2 2026 — Thema: "Van aanmelding naar dagelijks gebruik"

Outcome 1: Nieuwe gebruikers vinden binnen 5 min hun weg
├── Metric: Time-to-value van 12 naar 5 minuten
├── Mogelijke richtingen: wizard, voorbeelddata, persoonlijke onboarding
└── Afhankelijk van: persona-onderzoek (Q1)

Outcome 2: Bestaande gebruikers komen vaker terug
├── Metric: WAU/MAU ratio van 0.25 naar 0.40
├── Mogelijke richtingen: notificaties, weekrapport, team-features
└── Afhankelijk van: analytics-implementatie

---

Q3 2026 — Thema: "Van individueel naar team"

Outcome 1: Teams werken samen in het product
├── Metric: % accounts met 3+ actieve gebruikers > 30%
├── Richtingen: gedeelde workspaces, team-dashboard, commentaar
└── Afhankelijk van: Q2 retentie-verbetering

Outcome 2: Teamleads zien waarde voor hun team
├── Metric: NPS teamleads > 45
├── Open: Interviews nodig om te begrijpen wat teamleads verwachten
```

---

## Het Roadmap-Gesprek met Stakeholders

Een roadmap is een communicatiemiddel. Zo presenteer je hem:

**Wat je WEL zegt:**
- "Dit zijn de resultaten die we nastreven en waarom"
- "Dit is hoe we meten of we op de goede weg zijn"
- "Dit is wat we nu weten en wat we nog moeten uitzoeken"

**Wat je NIET zegt:**
- "Dit is precies wat we gaan bouwen" (dat verandert)
- "Dit is wanneer het af is" (dat weet je niet)
- "Dit is een belofte" (het is een plan op basis van huidige kennis)

**Doorvragen die je kunt verwachten:**
- "Wanneer is feature X klaar?" → "We werken aan outcome Y. De specifieke oplossing bepalen we op basis van wat we leren"
- "Waarom staat mijn verzoek er niet op?" → "Hoe draagt het bij aan deze outcomes? Als het dat doet, past het erin"
- "Kan dit niet sneller?" → "Wat zouden we dan niet doen? Hier zijn de trade-offs"

---

## Output

Lever het volgende op:

1. **Outcome-roadmap** — in gekozen format (Now/Next/Later of kwartaal)
2. **Per outcome**: rationale (waarom dit), metric (hoe meten), mogelijke richtingen
3. **Herformulering** — als de input een featurelijst was: tabel met feature → outcome vertaling
4. **Afhankelijkheden** — wat moet er eerst of hangt van iets anders af
5. **Open vragen** — wat moet je nog valideren voordat je aan een outcome begint

---

## Veel Voorkomende Fouten

- **Features vermommen als outcomes** — "Bouw X" is geen outcome, ook niet als je er "zodat..." achter plakt
- **Te veel items in Now** — meer dan 3 items in Now = geen focus. Het hele punt is kiezen
- **Later als dump** — Later is niet "alles wat we ooit willen". Het zijn items die je serieus overweegt maar nog niet gevalideerd hebt
- **Geen metrics** — een outcome zonder metric is een wens. Hoe weet je of het gelukt is?
- **De roadmap als contract behandelen** — het is een plan op basis van huidige kennis. Nieuwe inzichten veranderen de roadmap
- **Nooit updaten** — de roadmap is een levend document. Review minimaal maandelijks
- **Stakeholders verrassen** — als je de roadmap verandert zonder communicatie, verlies je vertrouwen

---

## Zie ook

- **Product-visie** — De roadmap vertaalt de visie naar concrete stappen. Geen visie = geen richting voor je roadmap.
- **Product-strategie** — De roadmap is de executie van je strategie. Zorg dat je strategische keuzes helder zijn voordat je prioriteert.
- **OKRs Formuleren** — Outcomes op je roadmap zouden moeten aansluiten bij je team-OKRs.
- **North Star Metric** — Je roadmap-outcomes moeten bijdragen aan je North Star. Als dat niet zo is, vraag je af waarom ze erop staan.

---

## Bronnen

- Janna Bastow — *The Now/Next/Later Roadmap* (ProdPad)
- Bruce McCarthy — *Product Roadmaps Relaunched* (2017)
- Marty Cagan — *Empowered* — outcome-based teams
- Teresa Torres — *Continuous Discovery Habits* — outcomes koppelen aan discovery
