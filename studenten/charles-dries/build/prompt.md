# v2 — meerdere labels per reactie

Plak deze prompt in een nieuw, tijdelijk gesprek. Vervang alleen de tekst onder `REACTIE`.

```text
Je helpt een eventorganisator om één bezoekersreactie te ordenen. Geef precies één JSON-object terug, en verder niets.

Kies één of meer labels:
- "locatie/bereikbaarheid": een verbeterpunt over de eventlocatie, aanduiding, route, werken of bereikbaarheid.
- "programma": een verbeterpunt over optredens, stages of het programma.
- "catering": een verbeterpunt over eten of drinken.
- "prijs": een verbeterpunt over de kostprijs, tickets of consumpties.
- "personeel": een verbeterpunt over medewerkers, vrijwilligers of security.
- "veiligheid": een verbeterpunt over veiligheid, onveilig gedrag of drugs.
- "geen verbeterpunt": de reactie is uitsluitend positief of neutraal en bevat geen verbeterpunt.
- "onzeker/anders": de reactie is onduidelijk of past in geen label.

Regels:
- Geef elk duidelijk, verschillend verbeterpunt zijn eigen label. Een reactie over een te hoge prijs én slecht eten krijgt dus "prijs" en "catering".
- Kies "onzeker/anders" alleen als je geen betrouwbaar specifiek label kunt kiezen.
- Verzin geen feiten die niet in de reactie staan.
- Geef in "reden" één korte zin die alle gekozen labels alleen op basis van de reactie verklaart.

Formaat:
{"labels": ["locatie/bereikbaarheid"], "reden": "..."}

Voorbeeld:
Reactie: De straten lagen open, dus het was moeilijker bereikbaar. De locatie was niet zo goed aangeduid. Het eten was wel heel lekker.
Uitvoer: {"labels": ["locatie/bereikbaarheid"], "reden": "De reactie gaat over aanduiding en bereikbaarheid van de locatie."}

Voorbeeld:
Reactie: Muziek was top!
Uitvoer: {"labels": ["geen verbeterpunt"], "reden": "De reactie is uitsluitend positief over de muziek."}

Voorbeeld:
Reactie: Ik vond het te duur.
Uitvoer: {"labels": ["prijs"], "reden": "De bezoeker vindt de kostprijs te hoog."}

REACTIE
[plak hier één bezoekersreactie]
```
