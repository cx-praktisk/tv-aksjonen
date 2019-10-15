Rask Rundtur
============
_Visste du at TV-aksjonen går inn for å besøke 2,3 millioner husstander i løpet av 2 timer?_

Hvordan planlegger du ruten så du rekker innom flest mulig hus?

Dette er en variant av korteste vei, men for å unngå å havne i TSP-land foreslås følgende:
- Man starter og slutter ruten på hovedkontoret
- Man må rekke innom alle husene og tilbake til kontoret igjen før kvelden er over, dvs. på 4 timer.
- Man kan gå innom samme flere ganger.
- Hver vei tar et gitt antall minutter å gå.

```json
{
    "hus": [
        "TV-aksjonen sitt kontor",
        "Jonas sitt hus",
        "Monika sitt hus",
        "Erik sitt hus",
        "Teodor sitt hus"
    ],
    "veier": [
        { "fra": "TV-aksjonen sitt kontor", "til": "Monika sitt hus", "minutterGange": 30 },
        { "fra": "TV-aksjonen sitt kontor", "til": "Erik sitt hus", "minutterGange": 60 },
        { "fra": "Jonas sitt hus", "til": "TV-aksjonen sitt kontor", "minutterGange": 120 },
        { "fra": "Jonas sitt hus", "til": "Monika sitt hus", "minutterGange": 15 },
        { "fra": "Jonas sitt hus", "til": "Erik sitt hus", "minutterGange": 50 },
        { "fra": "Monika sitt hus", "til": "Jonas sitt hus", "minutterGange": 15 },
        { "fra": "Monika sitt hus", "til": "Teodor sitt hus", "minutterGange": 20 },
        { "fra": "Erik sitt hus", "til": "TV-aksjonen sitt kontor", "minutterGange": 60 },
        { "fra": "Erik sitt hus", "til": "Jonas sitt hus", "minutterGange": 50 },
        { "fra": "Teodor sitt hus", "til": "TV-aksjonen sitt kontor", "minutterGange": 15 },
        { "fra": "Teodor sitt hus", "til": "Monika sitt hus", "minutterGange": 20 },
        { "fra": "Teodor sitt hus", "til": "Erik sitt hus", "minutterGange": 40 }
    ]
}
```

Man må med andre ord ikke finne den korteste ruten innom alle husene, det holder å finne en gitt rute innom alle husene. Så kan man f.eks. konkurrere om å lage den løsningen som klarer å finne kortest mulig rute.

Tilbyr et skall i Java, C# og Javascript.

Gi ut to testsett (for å unngå hardkoding av rutene).

Må definere output dersom språk er valgfritt (feks. totalt antall minutter + rekkefølge)

Krav til løsning
----------------
- Løsningen må printe ut hvor mange minutter rundturen tar, og en eller annen beskrivelse av rundturen, så man kan verifisere at turen faktisk går innom alle husene.
- Man kan kode i det språket man vil, men vi har gjort klart noe kode
    * C# - https://dotnetfiddle.net/a6RHRw (Løsning https://dotnetfiddle.net/WDWGp0 TODO fjern)
    * Java - github: https://github.com/cx-praktisk/rask-rundtur-java Jdoodle: jdoodle.com/a/1Cvy

Konkurranse
-----------
Her kommer litt mer.
