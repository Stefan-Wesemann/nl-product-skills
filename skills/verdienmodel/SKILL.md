---
name: verdienmodel
description: "Brainstorm 3-5 verdienmodellen met doelgroepfit, risico's en validatie-experimenten. De stap vóór prijsstrategie: eerst HOE je geld verdient, dan pas HOEVEEL."
triggers:
  - verdienmodel
  - hoe verdienen we geld
  - monetisatie
  - business model
  - revenue model
  - hoe geld verdienen
  - inkomstenmodel
  - verdienmodellen
  - monetization
  - revenue streams
  - freemium
  - abonnementsmodel
  - subscription model
  - pricing model
---

# Verdienmodel

## Metadata

**Doel:** Bepaal hoe je product geld gaat verdienen. Niet welke prijs (dat is prijsstrategie), maar welk mechanisme: abonnement, transactiefee, freemium, marketplace-commissie? Genereer 3-5 opties, beoordeel ze op fit met je doelgroep en product, en kies het model dat je als eerste test.

**Relatie met andere skills:**
- **Verdienmodel** (deze skill) = HOE verdien je geld? Welk mechanisme?
- **Prijsstrategie** (aparte skill) = HOEVEEL vraag je? Welke tiers en prijspunten?
- Eerst verdienmodel kiezen, dan prijsstrategie uitwerken

**Aanpak:** Begin bij je doelgroep en producttype, niet bij wat concurrenten doen. Evalueer elk model op fit met je waardepropositie, schaalbaarheid en risico. Sluit af met een validatie-experiment per model.

**Output:** 3-5 verdienmodellen met per model: beschrijving, doelgroepfit, risico's, validatie-aanpak en een aanbeveling welk model je eerst test.

---

## Instructies

### Fase 0: Context ophalen

**Stap 1 — Check wat er al is**
Scan uploads, gedeelde mappen en workspace op relevante bestanden (waardepropositie, persona's, marktonderzoek, concurrent-analyse, eerdere verdienmodel-brainstorms). Lees ze door.

**Stap 2 — Slimme vragen stellen**
- **Wel context gevonden →** Bevestig kort wat je ziet ("Ik zie je waardepropositie en doelgroep, klopt dat?"). Stel alleen vragen over wat je nog mist.
- **Geen context →** Stel onderstaande vragen.

---

1. **Product**: Wat is het product? SaaS, marketplace, API, tool, dienst, platform?
2. **Doelgroep**: Wie betaalt? (B2B, B2C, B2B2C?) Is de gebruiker ook de betaler?
3. **Waardepropositie**: Welk probleem los je op? (Verwijs naar je waardepropositie als je die hebt)
4. **Huidige situatie**: Verdien je al geld? Zo ja, hoe? Zo niet, wat is je hypothese?
5. **Markt**: Hoe verdienen concurrenten of alternatieven geld?
6. **Fase**: Pre-launch, early traction, of groei?
7. **Constraints**: Zijn er beperkingen? (VC-verwachtingen, winstgevendheid-eis, regulering?)

---

## De 7 Verdienmodellen

### 1. Abonnement (Subscription)

**Hoe het werkt:** Klant betaalt een vast bedrag per maand of jaar voor toegang tot het product.

**Voorbeelden:** Spotify, Netflix, Notion, HubSpot, Slack

**Past goed bij:**
- Producten met doorlopende waarde (niet eenmalig gebruik)
- B2B SaaS waar teams dagelijks mee werken
- Producten waar je regelmatig nieuwe waarde toevoegt

**Past slecht bij:**
- Producten die klanten maar af en toe nodig hebben
- Eenmalige transacties (bijv. een rapportage-tool die je 1x/kwartaal gebruikt)

**Varianten:**
- Per gebruiker (Slack, Asana)
- Per team/organisatie (Basecamp)
- Per feature-tier (Mailchimp: free, standard, premium)

**Risico's:**
- Churn: als klanten de waarde niet voelen, zeggen ze op
- "Subscription fatigue" bij B2C — consumenten hebben te veel abonnementen

**Stimulusvragen:**
- "Gebruikt je klant het product dagelijks of wekelijks?"
- "Wat gebeurt er als ze een maand niet betalen — missen ze iets?"
- "Kun je waarde toevoegen die het abonnement rechtvaardigt?"

---

### 2. Transactiefee (Per gebruik)

**Hoe het werkt:** Klant betaalt per actie, per eenheid, of per verbruik.

**Voorbeelden:** Stripe (% per transactie), AWS (per GB/uur), Twilio (per SMS), OpenAI API (per token)

**Past goed bij:**
- Producten met variabel gebruik
- API's en infrastructuur
- Wanneer waarde direct meetbaar is per actie

**Past slecht bij:**
- Producten waar klanten budget-zekerheid willen
- Lage volumes (dan is de fee te laag om rendabel te zijn)

**Risico's:**
- "Bill shock": klant schrikt van onverwacht hoge rekening
- Revenue is onvoorspelbaar — moeilijk te forecasten
- Bij lage marges per transactie heb je veel volume nodig

**Stimulusvragen:**
- "Is er een logische eenheid om te berekenen? (Per document, per API-call, per actie)"
- "Hebben klanten veel variatie in gebruik?"
- "Kun je kosten direct koppelen aan de waarde die de klant ontvangt?"

---

### 3. Freemium

**Hoe het werkt:** Basisversie is gratis, betaalde versie biedt meer features, capaciteit of support.

**Voorbeelden:** Figma, Notion, Dropbox, Canva, Spotify

**Past goed bij:**
- Producten met virale/netwerk-effecten
- Wanneer het product zichzelf verkoopt door gebruik
- Grote markt waar je snel wilt groeien

**Past slecht bij:**
- Complexe enterprise-producten (lange sales cycle)
- Producten waar de gratis versie al genoeg is (geen upgrade-trigger)
- Hoge variabele kosten per gebruiker (elke gratis gebruiker kost je geld)

**De kernvraag:** Wat is de trigger om te upgraden?

**Typische triggers:**
- Meer gebruikers/seats toevoegen
- Opslaglimiet bereikt
- Geavanceerde features nodig (analytics, integraties, SSO)
- Zakelijk gebruik vs. persoonlijk gebruik

**Risico's:**
- Conversie is laag (typisch 2-5% in B2B SaaS)
- Gratis gebruikers kosten geld (hosting, support)
- Als de gratis versie te goed is, upgradet niemand

**Stimulusvragen:**
- "Welke feature is zo waardevol dat mensen ervoor betalen?"
- "Wat is de natuurlijke grens waar gratis niet meer genoeg is?"
- "Hoeveel kost een gratis gebruiker je per maand?"

---

### 4. Marketplace-commissie

**Hoe het werkt:** Je faciliteert transacties tussen twee partijen en neemt een percentage.

**Voorbeelden:** Airbnb (3-15%), Uber (25-30%), Etsy (6.5%), App Store (15-30%)

**Past goed bij:**
- Platformen die vraag en aanbod verbinden
- Wanneer je de transactie faciliteert of garandeert
- Markten met veel transacties

**Past slecht bij:**
- Eenzijdige producten (geen twee partijen)
- Wanneer partijen elkaar ook zonder jou vinden (disintermediatie-risico)

**Het kip-en-ei-probleem:** Je hebt aanbod nodig om vraag te trekken, en vraag om aanbod te trekken. Welke kant subsidieer je eerst?

**Risico's:**
- Disintermediatie: partijen gaan buiten het platform om
- Kip-en-ei bij lancering
- Regulering (in sommige markten)

**Stimulusvragen:**
- "Wie zijn de twee kanten van je markt?"
- "Waarom zou de transactie via jouw platform gaan in plaats van direct?"
- "Welke kant is bereid te betalen? Welke subsidieer je?"

---

### 5. Licentie / Eenmalige betaling

**Hoe het werkt:** Klant koopt het product eenmalig. Optioneel: jaarlijks onderhoud/support-contract.

**Voorbeelden:** Adobe (oude model), enterprise software, WordPress themes, Sketch (was eenmalig)

**Past goed bij:**
- On-premise software
- Producten die "af" zijn (niet doorlopend nieuwe features)
- Klanten die geen abonnement willen

**Past slecht bij:**
- Producten die regelmatig updates nodig hebben
- Wanneer je doorlopende kosten hebt (servers, API's)
- Als je voorspelbare recurring revenue wilt (VC-perspectief)

**Risico's:**
- Geen recurring revenue — elke maand opnieuw klanten werven
- Moeilijk te schalen zonder nieuwe producten
- Support-kosten lopen op zonder doorlopende inkomsten

**Stimulusvragen:**
- "Is je product 'af' of evolueert het continu?"
- "Hebben klanten een hekel aan abonnementen in jouw markt?"
- "Kun je aanvullende diensten verkopen na de initiële verkoop?"

---

### 6. Advertenties / Sponsoring

**Hoe het werkt:** Het product is gratis voor gebruikers. Inkomsten komen van adverteerders die toegang kopen tot je publiek.

**Voorbeelden:** Google, Facebook, nieuwsbrieven (Substack), podcasts, free mobile games

**Past goed bij:**
- Producten met een groot, betrokken publiek
- Content-platformen en media
- Wanneer je doelgroep niet wil betalen

**Past slecht bij:**
- Kleine niches (te weinig bereik voor adverteerders)
- B2B tools (advertenties verstoren de werkervaring)
- Producten waar privacy belangrijk is

**Risico's:**
- Je hebt enorm bereik nodig om significante inkomsten te genereren
- Advertenties verslechteren de gebruikerservaring
- Je bent afhankelijk van adverteerders, niet van je gebruikers

**Stimulusvragen:**
- "Hoeveel actieve gebruikers heb je (nodig)?"
- "Zouden advertenties de ervaring verpesten?"
- "Is er een adverteerder die je publiek waardevol vindt?"

---

### 7. Data / API / White-label

**Hoe het werkt:** Je verkoopt niet het product zelf, maar de data, technologie of het platform aan andere bedrijven die het inbouwen.

**Voorbeelden:** Plaid (financiële data-API), Mapbox (kaarten-API), White-label SaaS

**Past goed bij:**
- Producten met waardevolle data of technologie
- Wanneer andere bedrijven jouw functionaliteit willen inbouwen
- Platform-plays

**Past slecht bij:**
- Producten zonder technologische moat
- Wanneer je eindgebruiker-relatie belangrijk is

**Risico's:**
- Afhankelijkheid van een klein aantal grote klanten
- Klant kan besluiten het zelf te bouwen
- Geen directe relatie met eindgebruiker

**Stimulusvragen:**
- "Is er een bedrijf dat jouw technologie zou willen inbouwen?"
- "Heb je data die voor anderen waardevoller is dan voor jou?"
- "Kun je je product als API aanbieden naast de eigen interface?"

---

## Verdienmodellen Evalueren

Scoor elk relevant model op deze criteria:

| Criterium | Vraag | Score 1-5 |
|---|---|---|
| **Doelgroepfit** | Past dit bij hoe je klant wil betalen? | |
| **Waarde-alignment** | Betaalt de klant meer naarmate ze meer waarde krijgen? | |
| **Schaalbaarheid** | Groeit de omzet mee zonder evenredige kostengroei? | |
| **Voorspelbaarheid** | Kun je de omzet 3-6 maanden vooruit inschatten? | |
| **Eenvoud** | Snapt je klant in 10 seconden hoe ze betalen? | |
| **Defensibility** | Maakt het model het moeilijker om over te stappen? | |

**Totaalscore per model → rangschik van hoog naar laag.**

---

## Combinaties en Hybride Modellen

De meeste succesvolle producten combineren modellen. Denk in lagen:

**Typische combinaties:**
- **Freemium + Abonnement**: gratis basisversie, betaald voor teams/features (Notion, Figma)
- **Abonnement + Transactiefee**: basisbedrag + betaling per extra gebruik (Shopify: abonnement + transactiefee)
- **Marketplace + Abonnement**: gratis listing + betaald voor premium features (LinkedIn, Indeed)

**Vraag:** Kun je twee modellen combineren zodat ze elkaar versterken?

---

## Van Model naar Validatie

Per top-model definieer je een experiment:

| Element | Invullen |
|---|---|
| **Model** | Welk verdienmodel? |
| **Aanname** | Wat moet waar zijn? (bijv. "klanten willen per maand betalen, niet per jaar") |
| **Experiment** | Hoe test je het? |
| **Metric** | Wat meet je? |
| **Drempel** | Wanneer is het gevalideerd? |
| **Tijdlijn** | Hoe lang duurt de test? |

**Voorbeelden van validatie-experimenten:**

- **Fake pricing page**: Maak een pricing-pagina met je voorgestelde model. Meet clicks op "Kies dit plan". Nog niks bouwen.
- **Letter of Intent**: Vraag 5 potentiële klanten: "Zou je €X/maand betalen voor dit?" Krijg een schriftelijk commitment.
- **Concierge-model**: Lever de dienst handmatig en factureer alsof het product al bestaat.
- **Pre-sale**: Verkoop het product voordat het af is. Betalen mensen? Dan heb je validatie.

---

## Rode Vlaggen

Let op deze signalen dat je verdienmodel niet klopt:

- **"We monetiseren later wel"** — als je niet weet hoe je geld verdient, weet je niet voor wie je bouwt
- **"We doen advertenties"** — tenzij je miljoenen gebruikers hebt, is dit zelden genoeg
- **"Net als Spotify/Uber/Netflix"** — hun model werkt bij hun schaal. Jij bent niet bij die schaal
- **"Gratis + premium"** — als je niet kunt uitleggen waarom iemand upgradet, is freemium geen verdienmodel maar een kostenpost
- **"De klant bepaalt zelf"** — pricing moet je sturen, niet overlaten aan de klant
- **Model past niet bij koopgedrag** — B2B-klanten willen facturen en jaarcontracten, consumenten willen maandelijks opzegbaar

---

## Output

Lever het volgende op:

1. **3-5 verdienmodellen** — beschreven met doelgroepfit, risico's en combinatie-mogelijkheden
2. **Evaluatiematrix** — scores per model op de 6 criteria
3. **Aanbevolen model** — welk model test je eerst en waarom
4. **Hybride optie** — welke combinatie zou op termijn het sterkst zijn
5. **Validatie-experiment per model** — hoe test je elk model snel
6. **Volgende stap** — verwijs naar prijsstrategie om het gekozen model uit te werken

---

## Veel Voorkomende Fouten

- **Verdienmodel verwarren met prijsstrategie** — "€29/maand" is een prijs, niet een model. Eerst kiezen: abonnement, transactiefee of iets anders?
- **Alleen het eerste model overwegen** — genereer minimaal 3. Je eerste idee is zelden het beste
- **Model kiezen op basis van concurrenten** — wat voor hen werkt hoeft niet voor jou te werken. Je doelgroep en product zijn anders
- **Geen validatie** — een verdienmodel is een hypothese tot je het hebt getest met echte klanten
- **Schaal verwarren met nu** — "we doen advertenties net als Google" werkt niet met 500 gebruikers
- **Gebruiker en betaler verwarren** — bij freemium betaalt 2-5%. Bij B2B is de manager de betaler, niet de gebruiker. Ken het verschil

---

## Zie ook

- **Prijsstrategie** — Nadat je een verdienmodel hebt gekozen: werk het uit naar concrete tiers, prijspunten en validatie.
- **Lean Canvas** — Het verdienmodel is één blok van je Lean Canvas. Start daar als je het volledige business model wilt schetsen.
- **Business Model Canvas** — Voor een completer overzicht van alle 9 bouwblokken, inclusief revenue streams.

---

## Bronnen

- Ash Maurya — *Running Lean* (2012) — verdienmodel als onderdeel van Lean Canvas
- Alex Osterwalder — *Business Model Generation* (2010) — de 9 bouwstenen, waaronder revenue streams
- Product Faculty — Revenue Model frameworks
- Strategyzer — Revenue Streams patterns
- Reforge — Monetization Strategy en pricing-product fit
