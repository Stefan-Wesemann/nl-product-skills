---
name: testscenarios
description: "Genereer testscenario's voor een feature of user story: happy paths, edge cases, foutafhandeling en grensgevallen. Voorkom dat je pas na lancering ontdekt wat er misgaat."
triggers:
  - testscenarios
  - test scenarios
  - testgevallen
  - test cases
  - edge cases
  - happy path
  - foutscenarios
  - acceptance testing
  - wat kan misgaan
  - testen
---

# Testscenario's

## Metadata

**Doel:** Genereer een complete set testscenario's voor een feature of user story vóórdat je gaat bouwen. Happy paths, edge cases, foutafhandeling en grensgevallen — zodat je niet pas na lancering ontdekt wat er misgaat.

**Aanpak:** Begin bij de happy path, breid uit naar edge cases, fouten en grensgevallen. Denk vanuit de gebruiker, niet vanuit de code. Werk samen met Engineering en QA.

**Output:** Gestructureerde lijst van testscenario's per categorie, met verwacht gedrag en prioriteit.

---

## Instructies

### Fase 0: Context ophalen

**Stap 1 — Check wat er al is**
Scan uploads, gedeelde mappen en workspace op relevante bestanden (eerdere outputs, research, data). Lees ze door.

**Stap 2 — Slimme vragen stellen**
- **Wel context gevonden →** Bevestig kort wat je ziet ("Ik zie [X], klopt dat?"). Stel alleen vragen over wat je nog mist.
- **Geen context →** Stel onderstaande vragen.

1. **De feature**: Wat is de feature of user story waar we scenario's voor schrijven?
2. **Acceptance criteria**: Zijn er al acceptance criteria gedefinieerd? Zo ja, welke?
3. **Gebruikerscontext**: Wie gebruikt dit? In welke situatie? Op welk apparaat?
4. **Afhankelijkheden**: Hangt deze feature af van externe systemen, APIs of andere features?
5. **Bekende risico's**: Zijn er al scenario's waarvan je weet dat ze lastig worden?

---

## De Vier Categorieën

### 1. Happy Path (het ideale scenario)

De gebruiker doet alles "goed" — de standaard flow zonder afwijkingen.

**Vragen om happy paths te vinden:**
- "Wat is de meest voorkomende manier waarop een gebruiker dit zal gebruiken?"
- "Als alles perfect gaat, wat is dan het pad van begin tot eind?"
- "Wat is het verwachte resultaat als de gebruiker de flow voltooit?"

**Format per scenario:**

```
Scenario: [Beschrijving]
Gegeven: [Uitgangssituatie]
Wanneer: [Actie van de gebruiker]
Dan: [Verwacht resultaat]
Prioriteit: Must-test
```

**Voorbeeld:**
```
Scenario: Gebruiker maakt succesvol een nieuw rapport
Gegeven: Gebruiker is ingelogd en heeft minimaal 1 databron gekoppeld
Wanneer: Gebruiker klikt "Nieuw rapport", selecteert template,
         vult titel in en klikt "Opslaan"
Dan: Rapport wordt opgeslagen, gebruiker ziet bevestiging,
     rapport verschijnt in overzichtslijst
Prioriteit: Must-test
```

---

### 2. Edge Cases (uitzonderingen en grensgevallen)

Situaties die niet standaard zijn maar wel voorkomen. Hier zitten de meeste bugs.

**Vragen om edge cases te vinden:**
- "Wat als de gebruiker dit in een onverwachte volgorde doet?"
- "Wat als er heel weinig of heel veel data is?"
- "Wat als de gebruiker halverwege stopt en later terugkomt?"
- "Wat als twee gebruikers hetzelfde tegelijk doen?"
- "Wat als de input onverwacht lang, kort, of in een ander format is?"

**Typische edge cases:**

| Categorie | Voorbeelden |
|---|---|
| **Lege staat** | Geen data, geen items, eerste gebruik |
| **Volumes** | 0 items, 1 item, 1.000+ items |
| **Gelijktijdigheid** | Twee gebruikers bewerken hetzelfde tegelijk |
| **Onderbreking** | Gebruiker sluit browser halverwege, verliest verbinding |
| **Permissies** | Gebruiker zonder rechten probeert actie |
| **Invoer** | Extreem lange tekst, speciale tekens, lege velden, emoji's |
| **Tijd** | Tijdzones, zomer-/wintertijd, middernacht, schrikkeljaar |
| **Apparaat** | Mobiel, tablet, klein scherm, traag netwerk |

**Voorbeeld:**
```
Scenario: Gebruiker maakt rapport zonder databron
Gegeven: Gebruiker is ingelogd maar heeft geen databron gekoppeld
Wanneer: Gebruiker klikt "Nieuw rapport"
Dan: Gebruiker ziet melding "Koppel eerst een databron" met link
     naar instellingen. Geen lege of kapotte rapportage.
Prioriteit: Hoog
```

---

### 3. Foutafhandeling (als het misgaat)

Wat gebeurt er als er technische problemen zijn of de gebruiker iets fout doet?

**Vragen om foutscenario's te vinden:**
- "Wat als de server niet reageert?"
- "Wat als de API van een derde partij down is?"
- "Wat als de gebruiker ongeldige data invoert?"
- "Wat als de betaling mislukt?"
- "Wat als de sessie verloopt tijdens een actie?"

**Typische foutscenario's:**

| Categorie | Scenario | Verwacht gedrag |
|---|---|---|
| **Netwerk** | Verbinding valt weg | Duidelijke foutmelding, geen dataverlies |
| **Server** | API timeout | Retry + melding, geen eindeloos laden |
| **Validatie** | Ongeldig emailadres | Inline foutmelding bij het veld |
| **Autorisatie** | Verlopen sessie | Redirect naar login, werk bewaard |
| **Extern systeem** | Derde-partij API down | Graceful degradation, melding |
| **Data** | Corrupt of missende data | Fallback-weergave, geen crash |

**Voorbeeld:**
```
Scenario: Opslaan mislukt door serverfout
Gegeven: Gebruiker heeft rapport ingevuld en klikt "Opslaan"
Wanneer: Server geeft een 500-fout
Dan: Gebruiker ziet foutmelding "Opslaan mislukt, probeer opnieuw",
     ingevulde data blijft behouden, retry-knop beschikbaar
Prioriteit: Hoog
```

---

### 4. Grensgevallen (de randen van je feature)

Waar eindigt je feature en begint de rest van het systeem?

**Vragen:**
- "Wat als de gebruiker iets doet dat nét buiten de scope valt?"
- "Wat als ze een onverwachte combinatie van features gebruiken?"
- "Wat als ze vanuit een andere plek in het product bij deze feature terechtkomen?"
- "Wat als ze teruggaan na een actie? (browser back-knop)"

---

## Prioritering

Niet alle scenario's zijn even belangrijk. Prioriteer:

| Prioriteit | Criterium | Actie |
|---|---|---|
| **Must-test** | Happy path + scenario's die dataverlies of crash veroorzaken | Altijd testen vóór release |
| **Should-test** | Veelvoorkomende edge cases en foutscenario's | Testen als er tijd is |
| **Could-test** | Zeldzame grensgevallen | Testen in regressie, niet bij elke release |

---

## Testscenario's Schrijven met het Team

Doe dit samen met Engineering en QA:

1. **PM presenteert de feature** (5 min): Wat, voor wie, waarom
2. **Stille brainstorm** (10 min): Iedereen schrijft scenario's per categorie
3. **Delen en groeperen** (10 min): Overlap verwijderen, gaps vinden
4. **Prioriteren** (5 min): Must/Should/Could per scenario
5. **Eigenaarschap** (5 min): Wie schrijft de geautomatiseerde tests?

**Tip:** Engineers en QA denken in edge cases die PM's missen. Designers denken in gebruikersfouten die engineers missen. De combinatie is het sterkst.

---

## Output

Lever het volgende op:

1. **Happy path scenario's** — de standaard flows, volledig uitgeschreven
2. **Edge cases** — per categorie (volumes, permissies, invoer, timing, etc.)
3. **Foutscenario's** — per type (netwerk, server, validatie, extern systeem)
4. **Grensgevallen** — waar de feature raakt aan de rest van het systeem
5. **Prioritering** — must/should/could per scenario
6. **Open vragen** — scenario's die je niet kunt beoordelen zonder meer context

---

## Veel Voorkomende Fouten

- **Alleen happy path testen** — 80% van de bugs zit in de andere 20% van de flows
- **Scenario's schrijven na het bouwen** — dan test je wat je hebt gebouwd, niet wat je had moeten bouwen
- **Te technisch formuleren** — schrijf scenario's vanuit de gebruiker, niet vanuit de database
- **Foutafhandeling vergeten** — "wat als het misgaat" is de helft van gebruikerservaring
- **Lege staat negeren** — de eerste keer dat een gebruiker iets ziet is vaak leeg. Hoe ziet dat eruit?
- **Geen prioritering** — 50 scenario's zonder prioriteit = niemand test ze allemaal
- **Scenario's alleen door PM laten schrijven** — Engineering kent de technische edge cases, QA kent de testpatronen

---

## Bronnen

- Lisa Crispin & Janet Gregory — *Agile Testing* (2009)
- Gojko Adzic — *Specification by Example* (2011)
- Elisabeth Hendrickson — *Explore It!* (2013) — exploratory testing
- Michael Bolton — *Rapid Software Testing* — heuristieken voor edge cases
