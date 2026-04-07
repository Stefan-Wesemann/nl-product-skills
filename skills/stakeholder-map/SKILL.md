---
name: stakeholder-map
description: Breng je stakeholders in kaart en prioriteer ze via Power × Interest grid met concrete actiepunten per groep.
tags:
  - stakeholder
  - stakeholder mapping
  - alignment
  - governance
triggers:
  - stakeholder
  - stakeholdermap
  - stakeholder mapping
  - stakeholder analyse
  - belanghebbenden
  - power interest
  - wie heeft invloed
---

# Stakeholder Map

## Metadata

**Activatietrigger:** Je wil weten wie er invloed heeft op jouw product/initiative, wat ze willen, en hoe je hen meeneemt.

**Doel:** Systematisch in kaart brengen wie je stakeholders zijn → inzicht in hun belangen en macht → strategie om alignment te bouwen.

**Principe:** "Alignment > Agreement" — je hebt niet iedereen het eens nodig, je hebt commitment nodig op een gedeelde richting.

**Output:** Stakeholder-overzicht met prioraties en Power × Interest grid + actieplan per quadrant.

---

## Instructies

### Fase 0: Context ophalen

**Stap 1 — Check wat er al is**
Scan uploads, gedeelde mappen en workspace op relevante bestanden (eerdere outputs, research, data). Lees ze door.

**Stap 2 — Slimme vragen stellen**
- **Wel context gevonden →** Bevestig kort wat je ziet ("Ik zie [X], klopt dat?"). Stel alleen vragen over wat je nog mist.
- **Geen context →** Stel onderstaande vragen.

---

### Fase 1: Identificatie via Doorvragen

Voordat je namen opschrijft, moet je weten: wie zijn de stakeholders echt?

Ik stel deze vragen:

1. **Financiële of strategische invloed:** Wie controleert budget, go/no-go beslissingen, roadmap-prioriteiten?
   - C-suite, investor, department head, CFO?

2. **Uitvoering:** Wie bouwt/voert dit uit?
   - Engineering lead, design lead, product operations?
   - Wie moet het dagelijks doen?

3. **Gebruikers/impact:** Wie gebruikt dit product? Wie voelt de impact?
   - End-user, administrator, customer support, sales?

4. **Externe factoren:** Wie buiten je organisatie heeft invloed?
   - Key customer, partner, regulator, competitor beweging?

5. **Informatie/expertise:** Wie weet iets wat anderen niet weten?
   - Data analyst, technical architect, customer success lead?

6. **Politieke spelers:** Wie zit in het netwerk van beslissers?
   - CEO's vertrouweling, longstanding team member, mentor van decision maker?

**Output Fase 1:** Lijst van 8-15 stakeholders (niet meer, niet minder). Groepeer ze in rollen.

---

### Fase 2: Onderzoeken per Stakeholder

Voor elke stakeholder, maak dit duidelijk:

| Stakeholder | Rol | Belang in dit initiatief | Hudig standpunt | Macht/Invloed | Motivatie/Bezorgdheid |
|---|---|---|---|---|---|
| Sarah (VP Eng) | Engineering-leider | Technische haalbaarheid, team capacity | "Interessant, maar druk" | HOOG (kan team blokkeren) | Wil niet overmand team; wil snelle wins |
| Marcus (CFO) | Finance | Budget, ROI | "Waar is de business case?" | HOOG (controleert geld) | Wil duidelijkheid op kosten/baten |
| Jaap (Head Sales) | Revenue | Klantwaarde, sales enablement | "Klanten vragen hier om" | HOOG (invloed op go-to-market) | Wil competitive advantage; wil geen delays |

**Doorvragen per stakeholder:**
- Hoe hebben zij belang bij succes of mislukking?
- Wat is hun grootste zorg?
- Wat zouden zij graag anders zien?
- Welke metrics tellen voor hen?

---

### Fase 3: Power × Interest Grid

Dit is de kern. Plot je stakeholders in 2×2:

```
           MACHT/INVLOED (hoog)
                    ↑
                    │
Manage       │ MANAGE CLOSELY │ KEEP SATISFIED
Closely    │                 │
         │                 │
         │                 │
         ├─────────────────┼──────────→ INTERESSE (in dit initiatief)
         │                 │
Monitor   │ MONITOR         │ KEEP INFORMED
          │ (Keep in loop)  │
                    │
                    ↓
           Macht/invloed (laag)
```

**Vier quadranten:**

**1. MANAGE CLOSELY** (Hoog macht + Hoog interesse)
- Dit zijn je champions EN potential blockers
- Voorbeeld: VP Engineering, key customer, CFO
- **Actie:** Regelmatig 1-op-1, transparantie, input vragen, aligned houden
- **Frequentie:** Wekelijks of bi-weekly check-ins
- **Risico:** Als deze groep niet aligned blijft, project stopt

**2. KEEP SATISFIED** (Laag macht + Hoog interesse)
- Dit zijn investerders van tijd/emotie, maar niet formele macht
- Voorbeeld: Product designer, passionate customer, team lead
- **Actie:** Houdt ze informed, laat ze voelen dat hun input telt, geeft ownerschap
- **Frequentie:** Bi-weekly updates of demos
- **Voordeel:** Kunnen grassroots momentum bouwen

**3. KEEP INFORMED** (Hoog macht + Laag interesse)
- Dit zijn people who could wreck it if annoyed, maar engaged niet echt
- Voorbeeld: CFO (zolang budget approved), executive sponsor, technical architect
- **Actie:** Status updates (niet volle briefings), vraag formeel akkoord als nodig
- **Frequentie:** Maandelijkse status, ad-hoc voor big decisions
- **Risico:** Negeren = ze krijgen vragen van anderen → worden tegen je

**4. MONITOR** (Laag macht + Laag interesse)
- Dit zijn people on the periphery
- Voorbeeld: Junior designer, HR (tenzij hiring), marketing later
- **Actie:** Informatie toegankelijk maken, maar niet proactief briefen
- **Frequentie:** Ad-hoc, of include in team meetings

---

### Fase 4: Alignment Strategie per Groep

**Voor MANAGE CLOSELY (je kritieke stakeholders):**

Maak per persoon een mini-strategie:

| Stakeholder | Hudig Standpunt | Kernbezorgdheid | Jouw move | Success metric |
|---|---|---|---|---|
| Sarah (VP Eng) | "Druk" | Team burnout, stability | Weekly 15-min sync; ik neem capacity-planning; ik stel scope-vragen VOOR je team | Sarah says: "This is doable, team feels good" |
| Marcus (CFO) | "Waar is het geld?" | Onrendabiliteit, budget slip | Duidelijke business case + 90-day check-in op spend vs. plan | Marcus approves budget + reviews monthly |

**Voor KEEP SATISFIED:**
- Zorg dat hun input echt GEBRUIKT wordt (niet theater)
- Toon impact: "Je feedback op user flows → hebben we dit zo gebouwd"
- Zet hen in early access, beta, user testing

**Voor KEEP INFORMED:**
- Keep it SHORT: 1-pager status, not 30-slide deck
- Geef optie: "Vragen? Otherwise assume you're good"
- Vraag formal sign-off alleen voor kritieke gates (budget, launch)

**Voor MONITOR:**
- Zorg ze niet overvallen door nieuws via andermans mond
- Optioneel checkin: "We're progressing on X, thought you'd want to know"

---

### Fase 5: Wat Bindt Iedereen?

Alignment gebeurt niet door iedereen het eens te zijn over details. Het gebeurt door een gedeelde richting.

**Stel deze vragen aan jezelf:**

1. **Wat willen alle stakeholders?** (Niet "wat wil elk individu", maar "waar overlappen wij?")
   - Voorbeeld: Alle stakeholders willen sneller op markt, blij klanten, geen technical debt
   
2. **Waar verschillen jullie?** (En wat is OK?)
   - VP Eng wil robustness, Sales wil features → beiden waar
   - Marcus wil efficiency, Product wil perfectionisme → tradeoff nodig

3. **Wat is non-negotiable?**
   - Ik zeg: "Dit moeten we doen" — wat zeggen stakeholders?
   - Aligned? Of conflict?

4. **Wat is onzeker?**
   - "We don't know yet if X will work" — welke stakeholder help je valideren?

---

### Fase 6: Communicatie-cadence

Zorg dat stakeholders niet voelen dat je ze ignoreert of overvalt.

**Wekelijks:**
- MANAGE CLOSELY: 1-op-1 sync of quick standup (15 min)

**Bi-weekly:**
- MANAGE CLOSELY: Formal status (written or meeting, 30 min)
- KEEP SATISFIED: Product demo or update

**Maandelijks:**
- KEEP INFORMED: Status email (1-pager)
- MONITOR: Optional, as-needed

**Ad-hoc:**
- Alle quadranten: Decisions, blockers, big changes (no surprises)

---

### Fase 7: Conflictopsporring

**Als stakeholders tegenstrijdige eisen hebben:**

1. **Map het conflict:** Wie wil wat en waarom?
   - Sarah: "Geen Big Bang launch, incremental rollout"
   - Jaap: "Launch moet indrukwekkend zijn, klanten wachten"

2. **Zoek de onderliggende need:**
   - Sarah: "Ik wil risico minimaliseren, team's stability"
   - Jaap: "Ik wil competitive advantage, klantwaarde"

3. **Vind de derde optie:**
   - Incremental launch MAAR spectacular per phase?
   - Launch voor segment A (test), dan B en C?

4. **Escaleer alleen als echt nodig:**
   - Probeer eerst zelf op te lossen
   - Als niet: escaleer naar shared boss + present beide standpunten + ask for direction

---

## Output

Je levert af:

1. **Stakeholder-lijst** (Naam, rol, interesse-level, macht-level)
2. **Power × Interest Grid** (Visueel of tabel met quadrants)
3. **Per-stakeholder strategie** (Wie, concern, actie, cadence)
4. **Alignment statement** (Wat bindt iedereen? Waar verschillen?)
5. **Communicatie-kalender** (Wie, wanneer, wat, hoe)

---

## Bronnen

- **Product Faculty** — Stakeholder Management & "Alignment > Agreement"
- **Reforge** — Product Management course (governing structures)
- **Andy Grove** — High Output Management (stakeholder sync, decision-making)

