# Bijdragen aan NL Product Skills

Leuk dat je wilt bijdragen. Dit project draait om kwalitatieve, Nederlandstalige product management skills. Hieronder staat wat je moet weten.

## Wat we zoeken

- **Verbeteringen** aan bestaande skills: betere vragen, scherpere frameworks, bugfixes
- **Nieuwe skills** die passen bij product management en nog niet bestaan
- **Feedback** via issues: wat werkt niet, wat mist, wat kan beter

## Kwaliteitseisen

### Taal
Alles in het Nederlands. Engelse vaktermen mogen als er geen gangbaar Nederlands alternatief is (bijv. "stakeholder", "framework").

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

    ## Wat we niet zoeken

    - Engelse skills (er zijn genoeg Engelstalige alternatieven)
    - Skills zonder onderliggend framework (geen "vraag AI om een lijstje")
    - Copy-paste van bestaande tools zonder eigen toevoeging
