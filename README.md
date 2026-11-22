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
| Namen van de ruimtes en cursusverwijzingen | `ROOMS` |
| Wachtwoord van de finale (letters worden per spel willekeurig verdeeld) | `FINAL_WORD` |
| Radioberichten tijdens het spel en wanneer ze komen | `RADIO` |
| Puzzeltekst, cursustip, hints, uitleg, controle van het antwoord | `PUZ` (één blok per ruimte) |
| Gegevens van de brug op het startscherm | `BRUG` |
| Tekeningen | functies `elevation`, `ballastSVG`, `jackSVG`, `bearingSVG`, `laneSVG`, `jointSVG` |

Tip: met **Spelleidermodus** op het startscherm loopt er geen klok en zijn alle ruimtes open. Handig om te testen en voor de pitch.

De voortgang wordt in de browser bewaard: wie de pagina vernieuwt, kan op het startscherm met **Ga verder** verder spelen (de klok loopt intussen door). Met **Opnieuw beginnen** wis je het bewaarde spel.

## Nog te doen

- [ ] Groepsnummer en namen invullen (`GROEP`) en in deze README
- [ ] AI-verklaring opstellen (verplicht volgens de opdracht; staat momenteel niet in het spel)
- [ ] Speltest door 2 à 3 medestudenten die het spel nog niet kennen, zonder AI; tijden noteren
- [ ] Tussentijdse feedback: donderdag 26/11
- [ ] Pitch van 5 minuten: donderdag 10/12

## Versies

- **v10:** eerste speelbare versie (30 minuten).
- **v11:** feedback van de speltest en controle met de cursus verwerkt: cursustermen (geen "val" meer), 45 minuten, gratis cursustip per ruimte, afrondingsfout in ruimte 6, verantwoording van de vaste oplegging, tekenfouten, uitleg na afloop, vergrootbare tekeningen en een radar met het naderende schip. De volledige lijst staat in de beschrijving van de v11-commit.
- **v12:** voortgang bewaren en hervatten, radioberichten van het schip en geluid (met dempknop), letters van de finale per spel in willekeurige volgorde, en een interactieve ballastkist in ruimte 2: blokken bijleggen en de balans testen, waarbij het brugdek zichtbaar reageert.
- **v13:** vlottere indeling en controlekamerstijl: elke ruimte is een werkbank (tekening met de bediening eronder, rechts opdracht, cursus, gegevens en hints), een beloningsscherm met de nieuwe letter na elke opgeloste ruimte, statuslampjes in de routebalk, een kaartknop in plaats van de grote "Je bent hier"-tekening, gegevens in een compact raster, zachte overgangen en een titelscherm.
- **v14:** ruimte 3, 4 en 6 interactief: vijzelkracht instellen met een schuifknop en een proefopening tegen de wind (het brugdek blijft steken of zwaait met een schok open), opleggingen aanklikken in de tekening en testen bij +54 °C (wat klemt kleurt rood, wat te vrij staat oranje), en een voegtest van −18 tot +54 °C met een meter die toont wat elk voegtype kan opnemen.
- **v15:** ruimte 1 en 5 interactief: na het bevestigen toont elk vakje van tabel 18.1 een animatie van hoe het gekozen brugtype echt beweegt (met ✓ of ✗), en de remkracht wordt in twee delen ingevuld met een meter voor de grenzen van 180 en 800 kN en een vrachtwagen die op het dek remt.

## Gebruik van AI

De code, de tekeningen en een eerste versie van de puzzelteksten werden gemaakt met Claude (Anthropic). Elke formule, waarde en vakterm werd vergeleken met de cursus Bruggenbouw 2026-2027; de paginaverwijzingen staan per ruimte in het spel. Wat we na controle aanpasten, staat in de beschrijving van de v11-commit.
