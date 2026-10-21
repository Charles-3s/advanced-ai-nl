# Kosten van de eventreactiesorteerder

> **Status: schatting.** Codex toont in deze chat geen exact tokenverbruik per run. De cijfers hieronder zijn daarom gebaseerd op de lengte van de prompt, testinput T01 en het verwachte JSON-antwoord.

Datum: 14 oktober 2026  
Model voor de schatting: GPT-6 Luna  
Rekenkoers: 1 dollar = 0,90 euro

## Kost van één run

| Deel | Geschat aantal tokens | Prijs per miljoen tokens | Kost |
|---|---:|---:|---:|
| Prompt en bezoekersreactie T01 (input) | 540 | $0,10 | $0,000054 |
| Label en korte reden (output) | 40 | $0,50 | $0,000020 |
| **Totaal** |  |  | **$0,000074 = €0,000067** |

Dat is ongeveer **0,007 eurocent per run**.

## Kost per maand

Bambata Openair organiseert twee evenementen per jaar: één open-aireditie en één indooreditie. Ik schat ongeveer 200 reacties per event, ook mondelinge feedback die eerst als tekst wordt genoteerd. Dat zijn 400 reacties per jaar, of gemiddeld ongeveer 33 reacties per maand.

Bron van het volume: eigen schatting op basis van ongeveer 5.000 bezoekers per event.

Formule:

```text
aantal reacties per maand × €0,000067
```

| Reacties per maand | Geschatte maandkost |
|---:|---:|
| 33 (mijn gemiddelde maandvolume) | €0,0022 |
| 333 (10×) | €0,0223 |
| 33.333 (1.000×) | €2,23 |

Eén event met 200 reacties kost naar schatting €0,0134.

## Vergelijking met GPT-6.1 Sol

| Deel | Geschat aantal tokens | Prijs per miljoen tokens | Kost |
|---|---:|---:|---:|
| Prompt en bezoekersreactie T01 (input) | 540 | $2,00 | $0,001080 |
| Label en korte reden (output) | 40 | $10,00 | $0,000400 |
| **Totaal** |  |  | **$0,001480 = €0,001332** |

GPT-6.1 Sol kost ongeveer **0,133 eurocent per run**: ongeveer twintig keer zoveel als GPT-6 Luna. Bij mijn gemiddelde volume kost Sol ongeveer €0,044 per maand; bij 1.000× volume ongeveer €44,36 per maand. Sol is dus duurder, maar kan nuttig zijn als hij moeilijke reacties merkbaar betrouwbaarder sorteert.

## Waarde van de tijdswinst

| Schakel | Waarde | Bron |
|---|---:|---|
| Handmatig | 20 seconden per reactie | eigen schatting: lezen, begrijpen en categoriseren |
| Met de tool | 8 seconden per reactie | werkhypothese: 3 s draaien + 5 s nakijken |
| Winst per reactie | 12 seconden | 20 s − 8 s |
| Volume | 400 reacties per jaar | eigen schatting: 2 events × 200 reacties |
| Uren gewonnen | 1 uur en 20 minuten per jaar | 400 × 12 s = 4.800 s |
| Uurwaarde | €15 per uur | aanname: waarde van vrijwilligerstijd |
| Waarde van de tijdswinst | €20 per jaar | 1,33 uur × €15 |
| Kost van de tool | ongeveer €0,03 per jaar | 400 × €0,000067 |
| **Netto waarde** | **ongeveer €19,97 per jaar** | €20 − €0,03 |

Mijn zwakste cijfer is de handmatige tijd van 20 seconden. Als die in werkelijkheid maar 10 seconden is, bespaart de tool slechts 2 seconden per reactie. Dan is de netto waarde ongeveer €3,31 per jaar.
