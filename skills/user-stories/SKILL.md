---
name: user-stories
description: "Schrijf user stories volgens de 3 C's (Card, Conversation, Confirmation) en INVEST-criteria. Met acceptance criteria die engineering en QA direct kunnen gebruiken."
triggers:
  - user story
  - user stories
  - gebruikersverhaal
  - story schrijven
  - als gebruiker wil ik
  - backlog item
  - acceptance criteria
  - stories schrijven
---

# User Stories

## Metadata

**Doel:** Schrijf user stories die het team helpt begrijpen VOOR WIE je bouwt, WAT ze willen en WAAROM — zonder de HOE vast te leggen. De story is een gespreksstarter, niet een specificatie.

**Aanpak:** 3 C's (Card, Conversation, Confirmation). INVEST-check per story. Acceptance criteria die concreet en testbaar zijn.

**Output:** Uitgeschreven user stories met acceptance criteria, klaar voor de backlog.

---

## Instructies

### Fase 0: Context ophalen

**Stap 1 — Check wat er al is**
Scan uploads, gedeelde mappen en workspace op relevante bestanden (eerdere user stories, persona-documenten, feature specs). Lees ze door.

**Stap 2 — Slimme vragen stellen**
- **Wel context gevonden →** Bevestig kort wat je ziet ("Ik zie [X], klopt dat?"). Stel alleen vragen over wat je nog mist.
- **Geen context →** Stel onderstaande vragen.

---

1. **Context**: Voor welke feature of epic schrijven we stories?
2. **Persona**: Voor welke persona is dit? (Verwijs naar je persona's als je die hebt)
3. **Doel**: Wat is het gewenste outcome van deze feature?
4. **Scope**: Hoe gedetailleerd moeten de stories zijn? (Epic-level of sprint-ready?)
5. **Team**: Wie gaat deze stories oppakken? Hebben ze context nodig?

---

## De 3 C's

### Card — de korte beschrijving

**Format:**
```
Als [persona/rol]
wil ik [actie/capability]
zodat ik [resultaat/waarde]
```

**Regels:**
- **Als** = een specifieke gebruiker of rol, niet "de gebruiker" of "het systeem"
- **Wil ik** = wat ze willen DOEN, niet hoe het technisch werkt
- **Zodat** = de waarde of het resultaat. Dit is het belangrijkste deel — als je het "zodat" niet kunt invullen, is de story niet waardevol

**Goed:**
```
Als teamlead
wil ik in één overzicht zien wat mijn team deze week heeft bereikt
zodat ik mijn weekrapport in 5 minuten kan schrijven in plaats van 45 minuten
```

**Fout:**
```
Als gebruiker
wil ik een dashboard
zodat ik data kan zien
```
→ Te vaag. Welke gebruiker? Welke data? Welke waarde?

### Conversation — het gesprek

De card is niet de specificatie. De specificatie ontstaat in het gesprek tussen PM, Design en Engineering.

**Vragen voor het gesprek:**
- "Hoe doet de gebruiker dit nu? Wat is het probleem?"
- "Wat is de kleinste versie die nog waarde levert?"
- "Wat zijn de edge cases?" (verwijs naar testscenarios skill)
- "Is er design nodig of is het duidelijk genoeg?"

### Confirmation — de acceptance criteria

Hoe weet je dat de story af is? Dat zijn de acceptance criteria.

---

## Acceptance Criteria Schrijven

**Format: Gegeven / Wanneer / Dan**

```
Gegeven [uitgangssituatie]
Wanneer [actie]
Dan [verwacht resultaat]
```

**Per story: 3-7 acceptance criteria.** Minder = te vaag. Meer = de story is te groot.

**Voorbeeld:**

```
Story: Als teamlead wil ik een weekoverzicht van teamactiviteit
       zodat ik mijn weekrapport snel kan schrijven

Acceptance Criteria:

1. Gegeven dat ik teamlead ben met 3+ teamleden
   Wanneer ik het weekoverzicht open
   Dan zie ik activiteit van alle teamleden van de afgelopen 7 dagen

2. Gegeven dat een teamlid geen activiteit had deze week
   Wanneer ik het weekoverzicht open
   Dan zie ik dat teamlid met "Geen activiteit" in plaats van een lege rij

3. Gegeven dat ik het weekoverzicht bekijk
   Wanneer ik op "Kopieer naar klembord" klik
   Dan wordt het overzicht gekopieerd in een format dat ik in Slack kan plakken

4. Gegeven dat het maandag is
   Wanneer ik inlog
   Dan krijg ik een notificatie dat het weekoverzicht klaarstaat
```

**Tips voor goede acceptance criteria:**
- Testbaar: QA kan er een test van maken
- Specifiek: geen "de gebruiker ziet relevante informatie" maar WAT precies
- Onafhankelijk: elk criterium staat op zichzelf
- Geen implementatiedetails: niet "de API retourneert JSON" maar wat de gebruiker ervaart

---

## INVEST-Check

Elke story moet voldoen aan INVEST:

| Criterium | Vraag | Actie als het faalt |
|---|---|---|
| **I**ndependent | Kan deze story onafhankelijk van andere stories worden gebouwd en opgeleverd? | Splits of combineer stories |
| **N**egotiable | Is er ruimte voor het team om de oplossing te bepalen? | Verwijder implementatiedetails uit de story |
| **V**aluable | Levert het waarde op voor de gebruiker of het bedrijf? | Check het "zodat"-deel. Als je het niet kunt benoemen, schrap de story |
| **E**stimable | Kan het team inschatten hoe groot dit is? | Als niet inschatbaar: splits of doe eerst een spike |
| **S**mall | Past het in één sprint? | Splits in kleinere stories |
| **T**estable | Kun je vaststellen of het af is? | Scherp de acceptance criteria aan |

---

## Stories Splitsen

Als een story te groot is (niet **S**mall), splits hem. Maar niet op technische lagen — splits op waarde.

**Fout splitsen (technische lagen):**
```
Story 1: Bouw de database-tabel voor weekoverzicht
Story 2: Bouw de API voor weekoverzicht
Story 3: Bouw de frontend voor weekoverzicht
```
→ Story 1 en 2 leveren geen waarde aan de gebruiker.

**Goed splitsen (op waarde):**
```
Story 1: Als teamlead wil ik een weekoverzicht van activiteit
         (basis: lijst met items per teamlid)
Story 2: Als teamlead wil ik het weekoverzicht naar Slack kopiëren
         (toevoeging: kopieer-functionaliteit)
Story 3: Als teamlead wil ik een herinnering krijgen op maandag
         (toevoeging: notificatie)
```
→ Elke story levert zelfstandig waarde.

**Andere splitsingstechnieken:**
- **Per persona**: Story voor admin vs. story voor eindgebruiker
- **Per scenario**: Happy path eerst, edge cases later
- **Per data**: Eén databron eerst, meerdere later
- **Per platform**: Web eerst, mobiel later

---

## Output

Lever het volgende op:

1. **User stories** — in Card-format (Als/Wil ik/Zodat)
2. **Acceptance criteria per story** — in Gegeven/Wanneer/Dan format
3. **INVEST-check** — bevestiging dat elke story voldoet
4. **Suggesties voor splits** — als stories te groot zijn
5. **Open vragen** — wat moet nog besproken worden in de Conversation-fase

---

## Veel Voorkomende Fouten

- **"Als gebruiker" schrijven** — wees specifiek: welke persona of rol
- **Het "zodat" weglaten** — zonder waarde is het een taak, geen story
- **Implementatie in de story zetten** — "Als gebruiker wil ik een dropdown met..." is geen story, het is een design-keuze
- **Te grote stories** — als het niet in 1 sprint past, splits het
- **Acceptance criteria als wensenlijst** — houd het bij 3-7 criteria. Meer = de story is te groot
- **Stories in isolatie schrijven** — de story is een gespreksstarter. Schrijf de card, bespreek met het team, verfijn
- **Technisch splitsen** — backend/frontend splits leveren geen waarde per story

---

## Bronnen

- Mike Cohn — *User Stories Applied* (2004) — het standaardwerk
- Jeff Patton — *User Story Mapping* (2014) — stories in context plaatsen
- Ron Jeffries — de 3 C's (Card, Conversation, Confirmation)
- Bill Wake — INVEST-criteria
