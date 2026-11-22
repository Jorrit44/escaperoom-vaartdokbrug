# Escape room: De Vaartdokbrug zit vast

Item voor **deel 2 van de opdracht Bruggenbouw 2026-2027** (groep XX).

**▶ Speel het spel:** https://Jorrit44.github.io/escaperoom-vaartdokbrug/

Een zeeschip vaart op de beweegbare Vaartdokbrug af, en de brug zit in storing. In zes ruimtes los je een probleem op met de cursus: de indeling van beweegbare bruggen, het uitbalanceren van een basculebrug, de kracht in de vijzels, het oplegschema, de remkracht en de keuze van een brugdekvoeg. De brug is fictief, de waarden zijn realistisch maar vereenvoudigd.

## Samenwerken

Het hele spel zit in **één bestand: `index.html`**. Elke wijziging op de `main`-branch staat na ongeveer een minuut online op de speellink.

- **Kleine aanpassing (tekst, getal):** open `index.html` op GitHub, klik op het potloodje, pas aan en klik op **Commit changes**.
- **Grotere aanpassing:** clone de repository, open `index.html` in je browser om te testen, en commit en push daarna.
  ```bash
  git clone https://github.com/Jorrit44/escaperoom-vaartdokbrug.git
  ```
- Haal altijd eerst de laatste versie binnen (`git pull`) voor je begint, en werk niet met twee tegelijk aan hetzelfde stuk.
- **Groepsleden toegang geven:** de eigenaar gaat naar *Settings → Collaborators → Add people* en voegt de GitHub-namen toe.

## Waar pas je wat aan in `index.html`

| Wat | Waar in het script |
|---|---|
| Groepsnummer en namen | `GROEP` bovenaan |
| Speeltijd, straf per hint of fout | `TOTAL`, `HINT_STRAF`, `FOUT_STRAF` |
| Namen van de ruimtes, cursusverwijzingen, letters | `ROOMS` |
| Puzzeltekst, cursustip, hints, uitleg, controle van het antwoord | `PUZ` (één blok per ruimte) |
| Gegevens van de brug op het startscherm | `BRUG` |
| Tekeningen | functies `elevation`, `ballastSVG`, `jackSVG`, `bearingSVG`, `laneSVG`, `jointSVG` |

Tip: met **Spelleidermodus** op het startscherm loopt er geen klok en zijn alle ruimtes open. Handig om te testen en voor de pitch.

## Nog te doen

- [ ] Groepsnummer en namen invullen (`GROEP`) en in deze README
- [ ] Taakverdeling invullen bij *Over dit spel → Gebruik van AI*
- [ ] Speltest door 2 à 3 medestudenten die het spel nog niet kennen, zonder AI; tijden noteren
- [ ] Tussentijdse feedback: donderdag 26/11
- [ ] Pitch van 5 minuten: donderdag 10/12

## Versies

- **v10:** eerste speelbare versie (30 minuten).
- **v11:** feedback van de speltest en controle met de cursus verwerkt: cursustermen (geen "val" meer), 45 minuten, gratis cursustip per ruimte, afrondingsfout in ruimte 6, verantwoording van de vaste oplegging, tekenfouten, uitleg na afloop, vergrootbare tekeningen en een radar met het naderende schip. De volledige lijst staat in het spel onder *Over dit spel*.

## Gebruik van AI

De code, de tekeningen en een eerste versie van de puzzelteksten werden gemaakt met Claude (Anthropic). Elke formule, waarde en vakterm werd vergeleken met de cursus Bruggenbouw 2026-2027; de paginaverwijzingen staan per ruimte in het spel. Wat we na controle aanpasten, staat in het spel onder *Over dit spel*.
