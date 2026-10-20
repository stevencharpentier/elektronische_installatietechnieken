# Talstelsels

## Inleiding: wat is een talstelsel?

Wie professioneel met computers werkt, komt verschillende talstelsels tegen: tweetallig (**binair**), achttallig (**octaal**) en zestientallig (**hexadecimaal**). Dit hoofdstuk legt uit hoe die werken, en hoe je ertussen omrekent.

In het dagelijks leven gebruiken we **Arabische cijfers** om getallen op te schrijven. Maar dat is niet de enige mogelijke manier: Romeinse cijfers, turfjes zetten, of kralen schuiven op een telraam (abacus) kunnen exact dezelfde hoeveelheid weergeven. Dat brengt ons bij een belangrijk onderscheid:

- De **hoeveelheid** die je bedoelt (bijvoorbeeld een aantal appels in een mand).
- De **schrijfwijze** die je gebruikt om die hoeveelheid aan iemand anders duidelijk te maken.

Een hoeveelheid "bestaat" onafhankelijk van de techniek die je kiest om ze op te schrijven. Een talstelsel is dus niets anders dan een **afspraak over hoe je een hoeveelheid noteert**.

De Arabische cijfers zijn in de 16e eeuw in Europa ingevoerd door kooplieden en bankiers, en bleken veel handiger te werken dan de Romeinse cijfers. Het grote idee erachter: er is een cijfer om **nul** mee aan te duiden. De Romeinen hadden daar nooit een symbool voor bedacht, "niks" was voor hen niet iets om op te schrijven. Die nul levert een handige truc op: de **plaats** van een cijfer binnen een getal gaat mee de betekenis bepalen. Bij € 209.642 is de linker 2 veel waardevoller dan de rechter, en de 0 kan je niet zomaar schrappen, ook al stelt hij op zichzelf geen enkele euro voor. Dit principe heet een **positioneel talstelsel**, en daar gaat de rest van dit hoofdstuk over.

### Weetje: het talstelsel dat je elke dag gebruikt, maar niet meer actief kan rekenen

Naast het tiendelige (decimale) talstelsel leven we eigenlijk nog voortdurend met een **twaalftallig (duodecimaal) talstelsel**, zonder dat de meeste mensen er nog bewust mee kunnen rekenen:

- Een **dag telt 2 keer 12 uur**, en een klokwijzerplaat is in 12 opgedeeld.
- Een **jaar telt 12 maanden**.
- Een **dozijn** (12 stuks) en een **gros** (12 dozijn = 144 stuks) waren eeuwenlang de gangbare telmaat voor handelaars, bijvoorbeeld bij eieren, potloden of bestek.
- Het **Engelse maatsysteem** werkt voor lengtematen nog steeds grotendeels in twaalftallen: 12 inch (duim) in 1 foot (voet).
- Tot de omschakeling naar het decimale systeem in 1971 telde het **Britse pond** 12 pence in 1 shilling.

Twaalf is in veel opzichten praktischer dan tien als grondtal: 12 is deelbaar door 2, 3, 4 én 6 (tien enkel door 2 en 5), wat vroeger handig was om bijvoorbeeld een hoeveelheid goederen eerlijk in stukken te verdelen. Toch rekenen de meesten van ons niet meer vlot in twaalftallen: we gebruiken de losse restanten ervan (een dozijn eieren, 12 uur op de klok) zonder er nog actief sommen in op te lossen, in tegenstelling tot het binaire, octale en hexadecimale talstelsel die je in dit hoofdstuk wél leert gebruiken.

## Definities

### Een cijfer

Eén enkel numeriek symbool, bijvoorbeeld 7, of in het Romeinse systeem X.

### Een getal

Een getal bestaat uit één of meerdere cijfers. Elk getal groter dan het hoogste beschikbare cijfer in een talstelsel, bestaat dus noodzakelijk uit meerdere cijfers.

### Het grondtal van een talstelsel

Het grondtal is steeds gelijk aan het **aantal verschillende cijfers** dat een talstelsel gebruikt. We noteren het grondtal rechts onderaan het getal, bijvoorbeeld 437810 (het grondtal 10 in subscript).

### Een positioneel talstelsel

In een positioneel talstelsel bepaalt de **positie** van een cijfer binnen het getal zijn gewicht (eenheid, tiental, honderdtal,...). Het getal 1234 is dus iets helemaal anders dan 1324, ook al bestaan beide uit exact dezelfde vier cijfers. Uiterst rechts staat het **minst beduidende cijfer** (least significant digit), uiterst links het **meest beduidende cijfer** (most significant digit).

### Het gewicht van een cijfer

Het gewicht van een cijfer op een bepaalde positie is gelijk aan het **grondtal verheven tot de macht van die positie**, waarbij de uiterst rechtse positie steeds positie 0 heeft.

### De waarde van een getal

De waarde van een getal is de hoeveelheid die het voorstelt: de **som van elk cijfer vermenigvuldigd met zijn gewicht**.

### Opmerking: nullen toevoegen of weglaten verandert niets

De waarde van een getal verandert niet wanneer je links nullen toevoegt of weglaat, of rechts na de komma: 123 = 000123, en 431,16 = 431,1600000000. Dit mag je dus in beide richtingen vrij doen.

## De verschillende talstelsels

### Decimaal (grondtal 10)

Het alledaagse talstelsel, met 10 cijfers: 0 t.e.m. 9.

### Binair (grondtal 2)

Met 2 cijfers: 0 en 1. Het **geheugenelement van een computer** kan maar twee verschillende toestanden aannemen (bijvoorbeeld wel of geen spanning), vandaar dat alle schakelingen in een computer met het binaire talstelsel werken. Elk cijfer in een binair getal noemen we een **bit**.

Met 1 bit zijn er 2 mogelijkheden (0 en 1), met n bits zijn er 2ⁿ mogelijkheden:

| Aantal bits | Aantal mogelijkheden | Naam |
|---|---|---|
| 1 | 2¹ = 2 | bit |
| 4 | 2⁴ = 16 | nibble |
| 8 | 2⁸ = 256 | byte |
| 16 | 2¹⁶ = 65 536 | word |

### Octaal (grondtal 8)

Met 8 cijfers: 0 t.e.m. 7. De populariteit van het octale talstelsel komt door de **eenvoudige conversie** met het binaire talstelsel: elke groep van 3 bits komt overeen met precies 1 octaal cijfer (want 8 = 2³).

### Hexadecimaal (grondtal 16)

Met 16 "cijfers": de 10 decimale cijfers, aangevuld met de letters **A, B, C, D, E, F** voor de waarden 10 t.e.m. 15. Ook hier is de populariteit te danken aan de eenvoudige conversie met binair: elke groep van 4 bits komt overeen met precies 1 hexadecimaal cijfer (want 16 = 2⁴). In plaats van het binaire getal 1111 schrijf je dus gewoon het hexadecimale cijfer F: veel overzichtelijker bij lange binaire getallen. Je herkent een hexadecimaal getal soms aan het voorvoegsel `0x`, bijvoorbeeld `0x6F`.

### BCD (Binary Coded Decimal)

Bij BCD wordt **elk decimaal cijfer apart** omgezet naar zijn 4-bits binaire representatie, in plaats van het volledige getal in één keer om te zetten. Bijvoorbeeld 935 wordt 1001 0011 0101 (9 → 1001, 3 → 0011, 5 → 0101).

## De omzettingstabel

Deze tabel verbindt decimaal, binair (met de gewichten 8-4-2-1) en octaal/hexadecimaal met elkaar, en moet je **van buiten kennen**:

| Decimaal | Binair (8-4-2-1) | Octaal/Hexadecimaal |
|---|---|---|
| 0 | 0000 | 0 |
| 1 | 0001 | 1 |
| 2 | 0010 | 2 |
| 3 | 0011 | 3 |
| 4 | 0100 | 4 |
| 5 | 0101 | 5 |
| 6 | 0110 | 6 |
| 7 | 0111 | 7 |
| 8 | 1000 | 8 |
| 9 | 1001 | 9 |
| 10 | 1010 | A |
| 11 | 1011 | B |
| 12 | 1100 | C |
| 13 | 1101 | D |
| 14 | 1110 | E |
| 15 | 1111 | F |

## Omzetten naar het decimale talstelsel

Om de waarde van een getal in een ander talstelsel te kennen, vermenigvuldig je elk cijfer met het grondtal verheven tot de macht van zijn positie, en tel je alles op.

**Binair naar decimaal**, voorbeeld met 1100110₂:

```
1100110(2) = 1.2⁶ + 1.2⁵ + 0.2⁴ + 0.2³ + 1.2² + 1.2¹ + 0.2⁰
           = 64 + 32 + 0 + 0 + 4 + 2 + 0 = 102(10)
```

**Hexadecimaal naar decimaal**, voorbeeld met 1AB₁₆:

```
1AB(16) = 1.16² + A.16¹ + B.16⁰
        = 1.256 + 10.16 + 11.1
        = 256 + 160 + 11 = 427(10)
```

Dezelfde logica geldt voor het octale talstelsel, met machten van 8 in plaats van 16.

## Omzetten van het decimale talstelsel naar een ander talstelsel

Hier werk je in de **omgekeerde richting**: je deelt herhaaldelijk door het grondtal van het talstelsel waar je naartoe wil, en noteert telkens de rest. Je stopt zodra het quotiënt 0 wordt, en leest de resten van **onder naar boven**.

Voorbeeld: 102₁₀ omzetten naar binair (grondtal 2):

| Deling | Quotiënt | Rest |
|---|---|---|
| 102 / 2 | 51 | 0 |
| 51 / 2 | 25 | 1 |
| 25 / 2 | 12 | 1 |
| 12 / 2 | 6 | 0 |
| 6 / 2 | 3 | 0 |
| 3 / 2 | 1 | 1 |
| 1 / 2 | 0 | 1 |

Van onder naar boven gelezen: 102₁₀ = 1100110₂ (hetzelfde getal als in het vorige voorbeeld, in omgekeerde richting omgezet).

**Verkorte truc, enkel geldig voor binair**: is het getal in de linkerkolom oneven, dan is de rest 1; is het even, dan is de rest 0. Dat vermijdt de deling zelf telkens helemaal uit te schrijven.

Dezelfde methode (delen door 8, respectievelijk 16, in plaats van door 2) werkt voor de omzetting naar octaal en hexadecimaal.

## Rechtstreeks omzetten tussen binair, octaal en hexadecimaal

Omdat 8 = 2³ en 16 = 2⁴, kan je **rechtstreeks** tussen binair en octaal/hexadecimaal omzetten, zonder om te wegen via het decimale talstelsel:

- **Binair → octaal**: groepeer het binaire getal in groepjes van **3 bits**, te beginnen van rechts. Vul het meest linkse groepje zo nodig aan met nullen. Zet elk groepje om naar zijn octaal cijfer met de omzettingstabel.
- **Binair → hexadecimaal**: zelfde principe, maar in groepjes van **4 bits**.
- **Octaal/hexadecimaal → binair**: omgekeerd, elk cijfer wordt apart omgezet naar zijn binaire equivalent (3 respectievelijk 4 bits) met de omzettingstabel.
- **Octaal ↔ hexadecimaal**: hiervoor bestaat geen rechtstreekse kortere weg, je gaat altijd via het binaire talstelsel.

Voorbeeld, 1100110₂ omzetten naar hexadecimaal:

```
1100110(2) = 0110 0110   (aanvullen met een nul tot groepjes van 4)
           = 6    6
           = 66(16)
```

## Rekenen in het binaire talstelsel

### Optellen

Binair optellen werkt net als decimaal optellen, inclusief **overdracht** (carry): 1 + 1 = 10 in het binaire talstelsel (decimaal: 2), dus je schrijft een 0 en draagt een 1 over naar de volgende kolom.

```
  01011011   (91)
+ 00001101   (13)
  --------
  01101000   (104)
```

### Negatieve getallen: een probleem dat om een afspraak vraagt

Een computer kent enkel 0 en 1, geen minteken. Om toch met negatieve getallen te kunnen rekenen, zijn er door de tijd heen drie opeenvolgende technieken bedacht, elk met een eigen afspraak over hoe je het **meest linkse bit** (de tekenbit) gebruikt.

**1. Tekenbit**: de meest linkse bit van het getal geeft enkel het teken aan (0 = positief, 1 = negatief), de rest van de bits stelt de grootte voor zoals gewoonlijk. Eenvoudig, maar met twee problemen: het getal 0 heeft twee mogelijke voorstellingen (+0 en -0), en het optellen van een positief met een negatief getal geeft domweg een fout resultaat.

**2. 1-complement**: om het negatieve van een getal te vinden, **inverteer je alle bits** (elke 0 wordt een 1, elke 1 wordt een 0). Lost het optelprobleem gedeeltelijk op, maar het probleem van de dubbele voorstelling van 0 (+0 en -0) blijft bestaan, en een beperkt aantal optellingen blijft nog steeds fout.

Voorbeeld van de dubbele 0 (8 bits):

```
+0:  00000000
-0:  11111111  (1-complement van 00000000)
```

Voorbeeld van het optelprobleem: reken 4 + (-3) uit.

```
4:               00000100
3:               00000011
-3 (1-complement, alle bits omdraaien): 11111100

  00000100
+ 11111100
-----------
 100000000   (9 bits: er valt een 1 van de meest linkse positie af)
```

Laat je die overgevallen 1 gewoon vallen (zoals je bij 2-complement straks wél mag), dan hou je 00000000 over: dat is 0, terwijl 4 + (-3) natuurlijk 1 moet zijn. Bij 1-complement moet je die overgevallen bit nog apart **terug optellen** bij het resultaat (00000000 + 1 = 00000001 = 1, nu wel correct), een extra stap die makkelijk vergeten wordt. Dat is exact het probleem dat 2-complement oplost.

**3. 2-complement**: de uiteindelijke, correcte oplossing, gebruikt in alle hedendaagse computers. Je berekent eerst het 1-complement (alle bits inverteren), en telt er dan **1** bij op.

Voorbeeld 1: de 2-complement voorstelling van -7 (8 bits):

```
Binaire voorstelling van 7:        00000111
1-complement (alle bits omdraaien): 11111000
2-complement (+1):                  11111001
```

Voorbeeld 2: de 2-complement voorstelling van -18 (8 bits). Een positief getal verandert nooit: +18 is gewoon 00010010, tekenbit 0.

```
Binaire voorstelling van 18:       00010010
1-complement (alle bits omdraaien): 11101101
2-complement (+1):                  11101110
```

Voorbeeld 3: reken nu 9 + (-4) uit met 2-complement, en vergelijk met de 1-complement-aanpak hierboven.

```
9:                00001001
4:                00000100
-4 (2-complement): 11111100   (1-complement 11111011, +1)

  00001001
+ 11111100
-----------
 100000101   (9 bits: er valt opnieuw een 1 af)
```

Laat je die overgevallen 1 nu gewoon vallen (geen extra terugtel-stap nodig, in tegenstelling tot 1-complement), dan hou je 00000101 over = 5. En 9 + (-4) = 5, dat klopt meteen.

Met het 2-complement heeft 0 nog maar **één** voorstelling, en werkt optellen van een positief met een negatief getal altijd rechtstreeks correct: de overflow-bit op de meest linkse positie laat je gewoon vallen, zonder extra correctiestap.

### Omzetten van een 2-complement getal terug naar decimaal

1. Is de tekenbit 0? Dan is het een positief getal, zet rechtstreeks om naar decimaal.
2. Is de tekenbit 1? Dan is het een negatief getal: inverteer eerst alle bits en tel er 1 bij op, zet dat resultaat om naar decimaal, en zet er een minteken voor.

Voorbeeld: neem 11101110 uit voorbeeld 2 hierboven, en zet het terug om naar decimaal.

```
Gegeven (tekenbit 1, dus negatief): 11101110
Alle bits omdraaien:                00010001
+1:                                  00010010
00010010 in decimaal = 18
Dus 11101110 = -18
```

Dat is exact het getal waarmee we vertrokken zijn: de omzetting klopt in beide richtingen.

## Waarom dit alles kennen?

Dit lijkt abstract, maar is de basis van alles wat later in deze cursus komt: **digitale logica** werkt met exact deze 0'en en 1'en, en hexadecimale notatie kom je voortdurend tegen zodra je effectief met Logo en digitale schakelingen gaat werken (bijvoorbeeld bestandspermissies in Unix/Linux-systemen, of adressen en geheugenwaarden in een microcontroller).
