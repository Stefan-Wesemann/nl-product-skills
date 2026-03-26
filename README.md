# 🇳🇱 NL Product Skills

**Nederlandstalige product management skills voor AI-assistenten.**

Gebouwd door een Product Manager, voor product managers, consultants en ondernemers die in het Nederlands werken.

---

## Waarom dit bestaat

Er zijn honderden Engelstalige PM-skills. Geen enkele is in het Nederlands. Dat is een probleem als je:

- Nederlandse klanten bedient en deliverables in het Nederlands schrijft
- Stakeholders hebt die geen Engels willen lezen
- Werkt in een Nederlandse marktcontext met eigen dynamiek
- AI wilt inzetten maar niet elke output handmatig wilt vertalen

Deze skills zijn **geen vertalingen**. Ze zijn geschreven voor de Nederlandse markt, met Nederlandse voorbeelden, en bevatten eigen frameworks naast bewezen methodieken.

## Wat maakt deze skills anders

- **Diepgang boven snelheid** — elke skill stelt eerst vragen, vraagt door, en accepteert geen oppervlakkige antwoorden
- **FORCES Framework** — het 6-krachtenmodel (Motivatie, Enablement, Momentum vs Wrijving, Angst, Inertie) loopt door meerdere skills heen
- **Seven Powers** — Hamilton Helmers verdedigbaarheidsmodel als standaard lens bij strategie
- **Blue Ocean Strategy** — ERRC Grid en Six Paths als positioneringsframework
- **Nederlandse context** — poldermodel, LinkedIn NL, BTW, MKB vs enterprise, nuchterheid

## Skills

### Strategie

| Skill | Beschrijving |
|-------|--------------|
| `product-strategie` | Product Strategy Canvas (9 secties), Seven Powers, Moat Statement |
| `waardepropositie` | JTBD + FORCES Framework (6 krachten), Leverage Statement |
| `positionering` | Blue Ocean (ERRC Grid, Six Paths), Counter Positioning |
| `north-star-metric` | North Star Metric, sub-metrics, KPI-boom |
| `concurrentie-analyse` | 3 concurrenten diep, moat-analyse, relatieve positie |
| `prijsstrategie` | Modelkeuze, Van Westendorp, AI-kostenmodel (conditioneel) |
| `product-visie` | Korte, begrijpbare productvisie — intern gericht |

### Discovery

| Skill | Beschrijving |
|-------|--------------|
| `klantinterview` | The Mom Test + FORCES als doorvraag-lens |
| `aannames-bedenken` | Twee paden (nieuw/bestaand), multi-perspectief, Leverage hypotheses |
| `experiment-ontwerp` | Pretotyping & A/B tests, YODA principle, success thresholds |
| `doelgroepkeuze-primair` | 4 criteria, smallest viable audience, gedragssegmentatie |
| `discovery-plan` | *In ontwikkeling* |

### Executie

| Skill | Beschrijving |
|-------|--------------|
| `prd-schrijven` | 8-sectie PRD, producthypothese, aannames, AI-checklist (conditioneel) |
| `stakeholder-map` | Mapping + prioritering, Power × Interest grid |
| `pre-mortem` | Tigers / Paper Tigers / Elephants, risico-triage |
| `go-to-market` | FORCES per levenscyclusfase, StoryBrand messaging, STEPPS |

### Analyse

| Skill | Beschrijving |
|-------|--------------|
| `swot-analyse` | Gerichte vragen, cross-referentie matrix, Seven Powers lens |
| `ai-evals` | Evaluatiecriteria voor AI-output vanuit business-perspectief |

## Installatie

### Claude Code (plugin marketplace)
```bash
# Voeg de marketplace toe
claude plugin marketplace add SedanWeerman/nl-product-skills

# Installeer alle skills
claude plugin install nl-product-skills
```

### Claude Cowork / Claude.ai
Upload individuele `SKILL.md` bestanden als custom skills via de instellingen.

### Cursor / Copilot / andere AI-assistenten
Kopieer de `skills/` map naar je project of global skills directory. De `SKILL.md` bestanden volgen de [Agent Skills open standaard](https://agentskills.io/) en werken cross-platform.

## Hoe het werkt

Elke skill is een `SKILL.md` bestand — een markdown-document met instructies die je AI-assistent automatisch volgt wanneer relevant. Vraag om een productstrategie, en de `product-strategie` skill wordt geladen. Vraag om een klantinterview voor te bereiden, en de `klantinterview` skill wordt geactiveerd.

Skills staan los van elkaar — geen onderlinge afhankelijkheden. Je kunt ze individueel gebruiken.

## Frameworks & Bronnen

Deze skills bouwen voort op bewezen methodieken:

- **FORCES Framework** (Product Faculty) — 6-krachtenmodel voor gedragsverandering
- **Seven Powers** (Hamilton Helmer) — verdedigbare concurrentievoordelen
- **Blue Ocean Strategy** (Kim & Mauborgne) — ERRC Grid, Six Paths, Noncustomers
- **The Mom Test** (Rob Fitzpatrick) — klantinterviews zonder bias
- **JTBD** (Clayton Christensen) — waardepropositie vanuit klantperspectief
- **StoryBrand** (Donald Miller) — messaging framework
- **Contagious STEPPS** (Jonah Berger) — viraliteitsprincipes
- **AI Product Design** (MIT xPRO) — UX-principes voor AI-producten
- **Leverage Discovery** (Product Faculty) — iteratief strategisch inzicht

## Over de maker

**Stefan Wesemann** — Product Consultant & AI-strateeg. PSPO III gecertificeerd, MIT "Designing and Building AI Products", Product Faculty "AI Product Strategy". Werkt als freelance Product Manager voor Nederlandse opdrachtgevers vanuit WMNN Outcomes BV.

- [LinkedIn](https://linkedin.com/in/stefanwesemann)
- [GitHub](https://github.com/SedanWeerman)

## Licentie

Apache 2.0 — vrij te gebruiken, ook commercieel. Zie [LICENSE](LICENSE).

## Bijdragen

Suggesties, verbeteringen en nieuwe skills zijn welkom. Open een issue of stuur een pull request. Houd de taal Nederlands en de kwaliteit hoog.
