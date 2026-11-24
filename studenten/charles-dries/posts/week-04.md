# Week 4: Tijd winnen met bezoekersfeedback

## Mijn tool in cijfers

Mijn tool sorteert één bezoekersreactie in categorieën zoals bereikbaarheid, programma, catering, prijs en veiligheid. Als organisator kan ik daarna tellen welke verbeterpunten het vaakst terugkomen. Ik legde voor tien reacties vooraf het juiste label vast. Daarna testte ik dezelfde prompt twee keer op die testset.

In run 1 waren 10 van de 10 labels juist. In run 2 opnieuw 10 van de 10. Mijn resultaat is dus **20 op 20 juist (n = 10, 2 runs)**. De testset bevatte korte reacties, een Engelse reactie, positieve reacties en reacties met een duidelijk verbeterpunt. Voorbeelden zijn “Muziek was top!”, “Duur!” en een langere reactie over wegenwerken en bereikbaarheid bij Bambata Openair.

Dat resultaat betekent niet dat mijn tool altijd juist zal zijn. Bij een buurtest waren maar 1 van de 3 labels exact gelijk voordat ik mijn labels duidelijker maakte. Daarom voegde ik `locatie/bereikbaarheid` samen en behield ik ook `geen verbeterpunt`. De grootste beperking is dat mijn testset nog klein is. Ik moet later meer moeilijke en dubbelzinnige reacties toevoegen, want tien duidelijke voorbeelden bewijzen nog niet dat de tool in alle situaties goed werkt.

## Wat kost één run?

Ik gebruikte GPT-6 Luna. Codex toont in deze chat geen exact tokenverbruik per run, dus dit is een schatting op basis van mijn prompt, testreactie T01 en het verwachte JSON-antwoord. Mijn prompt plus de reactie telt ongeveer 540 inputtokens. Het korte label met reden telt ongeveer 40 outputtokens. Met de cursusprijzen van $0,10 per miljoen inputtokens en $0,50 per miljoen outputtokens komt dat uit op $0,000074, of **€0,000067 per reactie** bij een koers van $1 = €0,90. Dat is ongeveer 0,007 eurocent per reactie.

Voor Bambata Openair schat ik twee evenementen per jaar, met ongeveer 200 reacties per evenement. Dat zijn 400 reacties per jaar, of gemiddeld 33 per maand. Bij dat volume kost de tool ongeveer **€0,0022 per maand**. Bij tien keer zoveel reacties wordt dat €0,0223 per maand. Zelfs bij duizend keer het volume is de kost maar €2,23 per maand.

Ik vergeleek dit met GPT-6.1 Sol. Die kost naar schatting €0,001332 per reactie, ongeveer twintig keer zoveel als Luna. Bij mijn eigen volume is dat nog altijd maar €0,044 per maand, maar bij duizend keer het volume stijgt het naar ongeveer €44,36 per maand. Luna lijkt voor deze taak dus logischer, zolang een duurdere tool geen duidelijk betere resultaten geeft.

## Met de hand of met de tool?

Ik schat dat een organisator gemiddeld 20 seconden nodig heeft om één reactie te lezen, te begrijpen en in een categorie te plaatsen. Met mijn tool reken ik 3 seconden om de reactie te verwerken en 5 seconden om het antwoord na te kijken. Nakijken blijft nodig: een label is een hulpmiddel, geen beslissing die volledig zonder mens kan gebeuren.

De winst is dan 12 seconden per reactie. Bij 400 reacties per jaar is dat 4.800 seconden, of ongeveer 1 uur en 20 minuten. Ik waardeer vrijwilligerstijd bij Scouts Gooik en Bambata Openair op €15 per uur. De tijdwinst is dan ongeveer €20 per jaar. De toolkost is ongeveer €0,03 per jaar. De netto waarde is dus **ongeveer €19,97 per jaar**.

Dat bedrag is niet groot, maar de tool geeft ook een overzicht dat je met losse reacties minder snel krijgt. Als veel mensen bijvoorbeeld prijs of bereikbaarheid noemen, kan de organisatie dat sneller zien en meenemen naar een volgende editie. Voor een groter evenement met veel meer feedback kan dezelfde aanpak relevanter worden.

## Mijn zwakste cijfer

Mijn zwakste cijfer is de aanname van 20 seconden handmatig werk. Ik heb die tijd niet gemeten; ik heb hem geschat uit lezen, begrijpen en categoriseren. Als het handmatige werk in werkelijkheid maar 10 seconden duurt, bespaart de tool nog slechts 2 seconden per reactie. Dan zakt de netto waarde naar ongeveer **€3,31 per jaar**. De kost van de tool blijft dus klein. De echte vraag is niet of de tokens duur zijn, maar hoeveel tijd de organisatie werkelijk nodig heeft om feedback te verwerken en na te kijken.
