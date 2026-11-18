# E-Plopper Oliebollen Doseerder - Schematische Werking en Mechanisch Ontwerp

## Introductie

De **E-Plopper** is een volledig elektrische doseermachine voor oliebollen (en andere producten zoals krentenbollen, cakebeslag, ijs, etc.), ontwikkeld door Eyemation b.v. (www.oliebollenmachine.com). 

Het is de opvolger van de oudere pneumatische **Plopper** oliebollenmachine. De E-Plopper elimineert de noodzaak voor een compressor, wat leidt tot lager energieverbruik, minder geluid en meer mobiliteit (optionele accu).

**Belangrijkste specificaties (standaard model):**
- Materiaal: RVS
- Trechterinhoud: 42 liter
- Zuiger: 280 cc (doseert 2 oliebollen per slag)
- Volume: 10 – 280 cc (verdeeld over 2 bollen, 15-110 gram per bol)
- Snelheid: 2 – 120 oliebollen per minuut
- Voeding: 230 VAC, 0,5 A
- Afmetingen: ca. 590x268x176 mm (zonder trechter)
- Gewicht: 30 kg

Er is ook een XL-versie met hogere capaciteit (tot 390 oliebollen/min, 100L trechter, 3 doseerkamers, 6 bollen per dosering).

## Schematische Werking

De machine werkt als een **positieve verplaatsingsdoseerder** met een zuiger (piston).

### Werkingsprincipe:

1. **Vullen van de trechter**: Oliebollenbeslag (met of zonder vulling zoals krenten/rozijnen) wordt in de RVS-trechter gegoten.

2. **Aanzuigen**: De zuiger in de doseerkamer beweegt terug. Hierdoor wordt beslag uit de trechter in de doseerkamer gezogen (via zwaartekracht + onderdruk).

3. **Doseren**: De zuiger beweegt vooruit en perst het afgemeten volume beslag door de uitstroomopeningen (standaard 2 nozzles) uit. Dit vormt 2 oliebollen per slag, die direct in de frituur vallen of op een oppervlak worden gedoseerd.

4. **Herhaling**: De cyclus herhaalt zich met instelbare snelheid, volume en aantal.

### Schema (ASCII):

```
          [Trechter / Hopper]
                 |
                 | Beslag
                 v
     +-----------------------------+
     |      Doseerkamer            |
     |  [Zuiger] <--- Elektrische  |
     |               Aandrijving    |
     |               (servo/lineair)|
     +-----------------------------+
            /           \
           /             \
      [Nozzle 1]     [Nozzle 2]
          |               |
          v               v
     [Oliebol]       [Oliebol]
```

### Elektrische aandrijving vs. oude pneumatische versie

- **E-Plopper (elektrisch)**: Digitale regeling via display/keypad. Volume (slaglengte), snelheid en aantal elektronisch instelbaar. Laag stroomverbruik (0,5A). Optionele 48V accu voor draadloos gebruik (tot 15.000 bollen per lading).
- **Oude Plopper (pneumatisch)**: Volledig op perslucht, mechanisch. Volume instelbaar via sterknop (mechanische slagbegrenzer). Geen elektriciteit nodig voor de aandrijving, maar wel compressor. Minder gevoelig voor water, maar meer lawaai en energieverbruik.

### Extra functionaliteiten

- Digitale display met directe storingsmeldingen in tekst
- Teller (dag/totaal/countdown)
- Auto-stop na ingesteld aantal
- Noodstop
- Externe start/sensor mogelijk
- Demontabele doseerkamer voor eenvoudige reiniging
- Interne temperatuurcontrole met ventilatie

## Mechanisch Ontwerp

### Belangrijkste componenten:

1. **Trechter (Hopper)**: RVS, 42L, conisch om goed doorloop van plakkerig beslag te garanderen. Optioneel met coating.

2. **Doseerkamer**: Bevat de zuiger en cilinder. Demontabel (zie YouTube-video "E-plopper Doseerkamer demontage") voor reiniging en onderhoud. Ontworpen voor voedselveiligheid en eenvoudig schoonmaken.

3. **Zuiger (Piston)**: 280cc slagvolume. Precisie-afdichting om lekkage van beslag te voorkomen. Aangedreven door elektrische lineaire actuator of servomotor met spindel/kogelomloop.

4. **Aandrijving**: Volledig elektrisch. Waarschijnlijk een compacte servo- of stappenmotor met lineaire transmissie (spindel of krukas). Lage stroomsterkte duidt op efficiënte aandrijving.

5. **Uitstroom / Nozzles**: Twee uitgangen die het volume splitsen in twee gelijke oliebollen. Optioneel Minimes voor 3 mini-bollen. Voor bakkerij-optie: slang + diverse spuitmonden voor cake, soezen, etc.

6. **Besturing**: Digitaal paneel met keypad en display. Microcontroller regelt slag, snelheid en veiligheid.

7. **Frame / Behuizing**: Compacte RVS-behuizing. Montagepunten (4x M10) voor rail of verrijdbaar onderstel/liftkar.

### Voordelen van het ontwerp:

- Geen compressor → stiller, zuiniger, geen luchtslangen
- Compact en mobiel (accu-optie)
- Eenvoudig te reinigen (demontabele kamer)
- Hoge capaciteit en consistentie
- Veiligheidsfeatures (noodstop, startup checks)

## Bronnen

- Officiële website: https://www.oliebollenmachine.com/e-plopper/
- YouTube playlist Eyemation: E-Plopper Oliebollenmachine
- Belangrijke video's:
  - Product video: https://www.youtube.com/watch?v=LqNWM4OAiHw
  - Doseerkamer demontage: https://www.youtube.com/watch?v=GekowIcBvlc
  - Oude Plopper: https://www.youtube.com/watch?v=F9wE3Lb6y_E

*Dit document is gebaseerd op publiek beschikbare informatie van de fabrikant en video's. Gedetailleerde interne CAD-tekeningen zijn niet publiek beschikbaar.*

**Gemaakt voor documentatie doeleinden.**
