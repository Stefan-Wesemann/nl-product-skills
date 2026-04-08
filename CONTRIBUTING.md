# Bijdragen aan NL Product Skills

Sharing is caring. Tof dat je wilt bijdragen aan het verder verbeteren van deze skills! Dit project draait om kwalitatieve, Nederlandstalige product management skills. Hieronder staat wat je moet weten.

## Wat dit beter maakt

- **Verbeteringen** aan bestaande skills: verbetere inhoud, scherpere vragen, nog relevantere frameworks, bugfixes
- **Nieuwe skills** die passen bij product management en de set aan Nederlandstalige skills completer maken
- **Feedback** via issues: wat werkt niet, wat mist, wat kan beter

## Kwaliteitseisen

### Taal
Alles in het Nederlands. Jargon in het Engels is natuurlijk wel goed (bijv. "stakeholder", "framework").

### Skill structuur
Elke skill volgt dit format:

```
skills/naam-van-skill/
├── SKILL.md              # Hoofdinstructie (verplicht)
├── README.md             # Korte uitleg en installatie
├── references/           # Ondersteunende documenten
│   └── *.md
└── evals/                # Testcases
    └── evals.json
    ```

    ### SKILL.md vereisten
    - YAML frontmatter met `name`, `description`, en `triggers`
    - `description` maximaal 200 tekens
    - De skill moet doorvragen — geen directe generieke output
    - Gebaseerd op een erkend framework of bewezen methode
    - Bronvermelding bij gebruikte frameworks

    ### Evals
    Nieuwe skills hebben bij voorkeur minimaal 2 testcases in `evals/evals.json`.

    ## Hoe bij te dragen

    ### Bug of verbetering melden
    Open een issue met het template "Skill verbetering".

    ### Nieuwe skill voorstellen
    Open een issue met het template "Skill idee". Beschrijf welk probleem de skill oplost en welk framework je wilt gebruiken.

    ### Pull request
    1. Fork de repo
    2. Maak een branch (`git checkout -b naam-van-skill`)
    3. Volg de skill structuur hierboven
    4. Test je skill handmatig in Claude
    5. Open een PR met een korte beschrijving van wat de skill doet en waarom

    ## Wat ik niet zoek

    - Engelse skills (er zijn genoeg Engelstalige alternatieven)
    - Skills zonder onderliggend framework (geen "vraag AI om een lijstje")
    - Copy-paste van bestaande tools zonder eigen toevoeging
