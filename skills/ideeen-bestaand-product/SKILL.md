---
name: ideeen-bestaand-product
description: "Multi-perspectief ideatie voor bestaande producten. Genereer oplossingsrichtingen vanuit PM, Designer en Engineer-lens voor een specifiek probleem of kans."
triggers:
  - ideeën bedenken
  - brainstorm
  - ideatie
  - oplossingen bedenken
  - hoe lossen we dit op
  - feature ideeën
  - verbeterideeën
  - creatieve oplossingen
  - brainstorm sessie
---

# Ideeën Bestaand Product

## Metadata

**Doel:** Genereer meerdere oplossingsrichtingen voor een concreet probleem of kans in je bestaande product. Niet één idee, maar een brede set vanuit verschillende perspectieven — zodat je het beste kunt kiezen.

**Aanpak:** Multi-perspectief (PM, Designer, Engineer). Van divergent (zoveel mogelijk ideeën) naar convergent (de beste selecteren). Altijd gekoppeld aan een concreet probleem of kans, niet "brainstormen om te brainstormen".

**Output:** 8-12 ideeën vanuit 3 perspectieven, gescoord op impact en haalbaarheid, met top 3 om verder te verkennen.

---

## Instructies

### Fase 0: Context ophalen

**Stap 1 — Check wat er al is**
Scan uploads, gedeelde mappen en workspace op relevante bestanden (vorige brainstorm-sessies, user research, data over het probleem, eerdere ideatie-documenten). Lees ze door.

**Stap 2 — Slimme vragen stellen**
- **Wel context gevonden →** Bevestig kort wat je ziet ("Ik zie user research over dit probleem, klopt dat?"). Stel alleen vragen over wat je nog mist.
- **Geen context →** Stel onderstaande vragen.

---

1. **Het probleem of de kans**: Wat willen we oplossen of verbeteren? (Formuleer als klantprobleem, niet als feature)
2. **Bewijs**: Hoe weten we dat dit een probleem is? (Data, interviews, support tickets, eigen ervaring)
3. **Doelgroep**: Voor welke persona of welk segment?
4. **Constraints**: Zijn er beperkingen? (Technisch, budget, tijdlijn, juridisch)
5. **Eerdere pogingen**: Hebben we al eerder iets geprobeerd om dit op te lossen? Wat werkte niet?
6. **Gewenst resultaat**: Hoe ziet succes eruit? Welke metric willen we bewegen?

**Belangrijk:** Zonder een helder probleem wordt brainstormen een willekeurige ideeën-generator. Zorg dat het probleem scherp is voordat je begint.

---

## Stap 1: Probleem Scherp Stellen

Formuleer het probleem als:

```
[Persona] ervaart [probleem] wanneer [situatie],
waardoor [consequentie]. Dit raakt [metric] met [impact].
```

**Voorbeeld:**
```
Teamleads ervaren dat ze geen zicht hebben op teamvoortgang
wanneer ze hun wekelijkse update moeten schrijven, waardoor
ze 45 minuten besteden aan handmatig informatie verzamelen.
Dit raakt de adoptie-metric: teamleads die het product niet
waardevol vinden churnen 3x sneller.
```

---

## Stap 2: Divergent — Ideeën Genereren vanuit 3 Perspectieven

### PM-Perspectief (waarde en strategie)

Denk vanuit: "Wat levert de meeste waarde voor de klant en het bedrijf?"

**Stimulusvragen:**
- "Wat als we het probleem elimineren in plaats van verbeteren?"
- "Hoe lost de concurrent dit op? Wat doen ze anders?"
- "Wat als we niets bouwen maar het proces veranderen?"
- "Wat zou de 10x oplossing zijn — niet 10% beter maar 10x beter?"
- "Welke oplossing creëert de meeste lock-in of switching costs?"

### Designer-Perspectief (ervaring en bruikbaarheid)

Denk vanuit: "Hoe ervaart de gebruiker dit en hoe kan het moeitelozer?"

**Stimulusvragen:**
- "Wat als dit nul interactie van de gebruiker zou vragen?"
- "Hoe zou dit eruitzien als het voor iemand was die het product voor het eerst gebruikt?"
- "Welke stappen kan je weglaten zonder waarde te verliezen?"
- "Wat als de oplossing al bestond in een tool die ze al gebruiken?"
- "Hoe zou Apple/Notion/Slack dit oplossen?"

### Engineer-Perspectief (haalbaarheid en mogelijkheden)

Denk vanuit: "Wat is technisch mogelijk dat we nog niet overwogen hebben?"

**Stimulusvragen:**
- "Welke data hebben we al die we niet benutten?"
- "Wat kunnen we automatiseren dat nu handmatig gaat?"
- "Wat als we een bestaande API of dienst integreren?"
- "Wat is de kleinste technische verandering met de grootste impact?"
- "Wat wordt mogelijk door AI/ML dat vorig jaar nog niet kon?"

---

## Stap 3: Ideeën Documenteren

Per idee noteer je:

| Element | Invullen |
|---|---|
| **Naam** | Korte, herkenbare naam |
| **Beschrijving** | 1-2 zinnen: wat is het en hoe werkt het |
| **Perspectief** | PM, Designer of Engineer |
| **Aanname** | Wat moet waar zijn voor dit idee om te werken |
| **Kleinste versie** | Wat is de MVP van dit idee? |

**Voorbeeld:**
```
Naam: Auto-weekoverzicht
Beschrijving: Het product genereert automatisch een weekoverzicht
              op basis van teamactiviteit en stuurt het maandag
              naar de teamlead
Perspectief: Engineer (automatisering + bestaande data)
Aanname: Teamleads willen een samenvatting ontvangen, niet zelf
         samenstellen
Kleinste versie: Email met bullet-points van activiteit, geen
                 bewerkfunctie
```

---

## Stap 4: Convergent — Ideeën Selecteren

Nu je 8-12 ideeën hebt, selecteer de top 3 om verder te verkennen.

**Scorematrix (snel en pragmatisch):**

| Idee | Impact op metric (1-5) | Haalbaarheid (1-5) | Past bij strategie (1-5) | Totaal |
|---|---|---|---|---|
| Auto-weekoverzicht | 4 | 4 | 5 | 13 |
| Dashboard redesign | 3 | 2 | 4 | 9 |
| Slack-integratie | 5 | 3 | 4 | 12 |

**Doorvragen bij selectie:**
- "Welk idee testen we het snelst?" (snelste learning loop)
- "Welk idee heeft de meeste impact als het werkt?"
- "Welk idee is het riskantst? Moeten we dat juist eerst testen?"

---

## Stap 5: Van Idee naar Experiment

Koppel de top 3 ideeën aan een validatie-aanpak (verwijs naar experiment-ontwerp of opportunity-solution-tree):

Per idee:
- **Wat is de aanname?** (Wat moet waar zijn?)
- **Hoe testen we dat?** (Interview, prototype, fake door, A/B-test)
- **Wanneer weten we genoeg?** (Welke metric, welke drempel)

---

## Facilitatietips voor Teambrainstorm

Als je dit met je team doet:

1. **Probleem presenteren** (5 min): Context, data, persona
2. **Individuele brainstorm** (10 min): Iedereen schrijft alleen, geen discussie
3. **Delen zonder oordeel** (10 min): Iedereen presenteert, anderen luisteren
4. **Bouwen op elkaars ideeën** (10 min): "Ja, en..." in plaats van "Ja, maar..."
5. **Dot-voting** (5 min): Iedereen krijgt 3 stippen, stem op favorieten
6. **Top 3 bespreken** (15 min): Verdieping, kleinste versie, volgende stap

**Regels:**
- Kwantiteit boven kwaliteit in de divergente fase
- Geen kritiek tijdens het genereren
- Wilde ideeën zijn welkom — ze inspireren realistische varianten
- Bouw voort op anderen ("wat als we dat combineren met...")

---

## Output

Lever het volgende op:

1. **Probleemstelling** — helder geformuleerd met bewijs en metric
2. **8-12 ideeën** — met naam, beschrijving, perspectief, aanname en kleinste versie
3. **Scorematrix** — impact, haalbaarheid, strategische fit
4. **Top 3** — met rationale waarom deze verder verkend worden
5. **Volgende stap per idee** — hoe valideer je elk idee

---

## Veel Voorkomende Fouten

- **Brainstormen zonder probleem** — zonder helder probleem genereer je willekeurige features
- **Direct naar de eerste beste oplossing springen** — daarom minimaal 8 ideeën. Je eerste idee is zelden het beste
- **Alleen vanuit PM-perspectief denken** — Designers zien gebruikersfrustaties die PM's missen, Engineers zien mogelijkheden die anderen niet kennen
- **Ideeën te snel afkappen** — "dat kan technisch niet" is vaak "dat is technisch lastig". Laat Engineers de haalbaarheid beoordelen
- **Geen aannames benoemen** — elk idee is een hypothese. Als je de aanname niet kent, kun je het idee niet valideren
- **Van brainstorm naar bouwen zonder validatie** — een goed idee is nog steeds een aanname tot je het hebt getest

---

## Bronnen

- Jake Knapp — *Sprint* (2016) — gestructureerde ideatie in design sprints
- IDEO — Design Thinking methodologie
- Teresa Torres — *Continuous Discovery Habits* — ideeën koppelen aan opportunities
- Product Faculty — multi-perspectief discovery
