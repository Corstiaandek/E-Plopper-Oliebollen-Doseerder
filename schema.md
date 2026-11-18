# Gedetailleerd Schema Werking E-Plopper

## Processtroom

1. Beslag klaarmaken en in trechter gieten
2. Machine instellen (volume, snelheid, aantal) via digitaal display
3. Start dosering
4. Zuiger cyclus:
   - Retract: Aanzuigen beslag
   - Extend: Uitpersen via 2 nozzles
5. Oliebollen vallen in frituur
6. Herhaal tot ingesteld aantal of stop

## Timing per cyclus
Bij 100 oliebollen/min = 50 slagen/min ≈ 1,2 seconde per slag (incl. heen en terug).

## Elektrisch schema (hoog niveau)

```
230VAC → Voeding → Controller (MCU)
                    ↓
               Motor driver → Lineaire aandrijving → Zuiger
                    ↑
               Display + Keypad
                    ↑
               Sensoren (positie, veiligheid, temp)
```

Optioneel: Accu 48V in plaats van netspanning.
