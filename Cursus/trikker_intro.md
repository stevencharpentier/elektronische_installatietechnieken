# Trikker: algemene introductie

## Wat is Trikker?

Trikker is een Belgisch tekenprogramma (Bluebits) specifiek gemaakt voor elektriciens: het laat je toe om een eendraadschema en een situatieplan van een elektrische installatie te tekenen volgens de regels van het AREI, en koppelt die twee aan elkaar. Je gebruikt dit in deze cursus om situatieplannen en eendraadschema's op een professionele, consistente manier te tekenen in plaats van met een algemeen tekenprogramma.

### Waarom Trikker en niet EPLAN?

**EPLAN (Electric P8)** is ook een gekend elektrotechnisch tekenprogramma, maar het is gebouwd voor een heel ander doelpubliek: het ontwerpen en documenteren van **industriële besturingssystemen en machines** (schakelkasten voor automatisatie, PLC-bekabeling, paneelontwerp), niet voor eendraadschema's en situatieplannen van gewone woning- of tertiaire installaties volgens het AREI.

Dat verschil in doelpubliek vertaalt zich rechtstreeks in prijs en complexiteit:

- **EPLAN**: pakketten vanaf ongeveer €4.000 tot meer dan €15.000, met een licentiemodel gericht op bedrijven met uitgebreide, industriële ontwerpnoden.
- **Trikker**: €360 tot €540 per jaar (of €45/maand), met gratis educatieve licenties voor scholen.

## De volgorde: je vertrekt steeds vanuit het eendraadschema

Trikker is opgebouwd rond een vaste volgorde, en dat is geen toeval: je begint **altijd bij het eendraadschema**, niet bij het situatieplan.

1. **Eendraadschema eerst**: je sleept AREI-symbolen (beveiligingen, stroombanen) op je blad en verbindt je kringen. Hier leg je vast welke stroombanen er zijn, hoe ze beveiligd zijn, en hoeveel aftakpunten elke kring heeft.
2. **Situatieplan daarna**: pas nadat je eendraadschema klaar staat, teken je het grondplan (of importeer je een bestaand plan als DWG/DXF-achtergrond) en plaats je de symbolen op hun werkelijke locatie.

Deze volgorde is logisch, niet arbitrair: zonder een eendraadschema weet Trikker niet welke kringletters en symbolen beschikbaar zijn om op je grondplan te plaatsen. De twee schema's blijven bovendien **gekoppeld**: wijzig je iets in het eendraadschema, dan loopt de kringletter en het symbool op het situatieplan automatisch gelijk.

## Werken met meerdere verdiepingen

Een situatieplan in Trikker bestaat uit **pagina's**. Bij een gebouw met meerdere verdiepingen teken je typisch **één pagina per verdieping**, elk met zijn eigen grondplan en de symbolen die daar effectief staan. In de gratis demoversie is dit beperkt tot 1 pagina; de volledige (betalende of educatieve) versie laat een onbeperkt aantal pagina's toe, dus ook gebouwen met meerdere verdiepingen.

## Automatische materiaallijst

Trikker stelt automatisch een **materiaallijst** samen op basis van je eendraadschema: alle symbolen die je gebruikt hebt (schakelaars, stopcontacten, beveiligingen,...) worden geteld en overzichtelijk gelijst, zodat je niet manueel moet bijhouden hoeveel van elk onderdeel je nodig hebt.

## Van materiaallijst naar bestellijst

De materiaallijst die Trikker genereert, is niet enkel een overzicht: het is je vertrekpunt om effectief materiaal aan te kopen. Op basis van die lijst zoek je bij verschillende **online winkels** (groothandels en webshops voor elektromateriaal) op wat elk onderdeel kost. Afhankelijk van je **budget** en het **doeleinde** van de installatie (bijvoorbeeld een eenvoudige woning versus een installatie met hogere eisen aan afwerking of merk) maak je dan een keuze: niet elk onderdeel in je materiaallijst moet van hetzelfde merk of prijsniveau komen, en die afweging maak je bewust per project.

### Enkele Belgische voorbeelden die hun prijzen online tonen

- **[Gamma](https://www.gamma.be), [Hubo](https://www.hubo.be) en [Brico](https://www.brico.be)**: drie zeer gelijkaardige doe-het-zelfketens, elk met een ruim assortiment schakelmateriaal (onder andere Niko), prijzen rechtstreeks zichtbaar op elke productpagina, geen account nodig.
- **[Groothandel.be](https://groothandel.be)**: een elektrogroothandel die zich uitdrukkelijk richt tot "particulieren, doe-het-zelvers en professionals", met groothandelsprijzen die voor iedereen zichtbaar zijn, ook zonder professioneel account.
- **[Zelektro](https://www.zelektro.be)**: een Belgische webshop (met ook een fysieke winkel in Bornem) voor schakelmateriaal en verlichting, gericht op woninginstallaties, met prijzen zichtbaar op elke productpagina.

Let op: niet elke elektrogroothandel toont prijzen publiek. Grotere professionele groothandels zoals Cebeo vragen doorgaans eerst een (gratis) klantaccount voor je prijzen te zien kan krijgen. Dat is geen toeval: het laat hen toe per klant andere (vaak lagere) staffelprijzen te hanteren dan de "kassa"-prijs voor een particulier.

## Andere functies

- **Import van bestaande plannen**: je kan een DWG- of DXF-tekening (bijvoorbeeld van een architect) inladen als achtergrond van je situatieplan, net zoals je een afbeelding zou plaatsen.
- **Export naar PDF**: je schema's druk je af naar een vectoriële PDF, in één klik klaar om bij een keuring voor te leggen.
- **Symbolenbibliotheek volgens AREI**: de beschikbare symbolen volgen de officiële AREI-grafische symbolen (zie ook schemas.md), georganiseerd per kringletter. Je kan ook eigen symbolen tekenen via de optie "Vrij tekenen".
- **Automatische lokale back-up**: je bestanden worden automatisch lokaal op je computer bewaard.
- **Community forum**: je kan er terecht met vragen en meekijken met vragen van andere gebruikers.

## Praktijkvoorbeeld: een tuinhuis als addendum bij een bestaande installatie

Om alles hierboven samen te brengen, werken we één volledig voorbeeld uit: een **tuinhuis**, bijgebouwd bij een bestaande woning, dat als addendum op de bestaande elektrische installatie aangesloten wordt. Dit is precies het soort opdracht waarvoor je Trikker in de praktijk gebruikt.

### Uitgangssituatie

- Het tuinhuis bestaat uit **1 ruimte**, met 1 deur en 2 ramen.
- **Binnen**: 5 stopcontactpunten, waarvan 3 dubbele boven het werkblad.
- **Buiten**: 1 stopcontactpunt.
- **Verlichting**: 1 lichtpunt binnen en 1 lichtpunt buiten, beide **vanuit binnen** geschakeld.
- Het tuinhuis krijgt een **eigen bordje**, aan de muur in het tuinhuis zelf.
- Het bestaande hoofdbord van de woning staat in de **kelder**, op **30 m** van het tuinhuis.

### Eén plaats, twee lichtpunten: de serieschakelaar

Binnen en buiten elk een lichtpunt, maar beide vanuit **dezelfde plaats** (binnen) bediend: dit is het schoolvoorbeeld van een **serieschakelaar** (zie schemas.md), die net gemaakt is om 2 lichtpunten vanaf 1 plaats apart te bedienen. Geen twee aparte enkelpolige schakelaars naast elkaar nodig.

### Indeling in stroombanen

- **Stopcontactkring**: alle 6 stopcontactpunten (5 binnen + 1 buiten) op **1 kring**, ruim onder de AREI-limiet van 8 aftakpunten. Kabeldikte 2,5 mm², automaat **20 A**: dit is een **zuivere** stopcontactkring (geen verlichting erbij gemengd), en 20 A is in België de gangbare praktijkwaarde voor zo'n zuivere stopcontactkring op 2,5 mm² (tabel 4.11 laat dit toe; 16 A hoort eerder bij een gemengde kring van stopcontacten én verlichting samen).
- **Verlichtingskring**: de 2 lichtpunten op een **aparte, zuivere verlichtingskring**, los van de stopcontacten. Kabeldikte 1,5 mm², automaat 10 A. Een aparte kring in plaats van alles op één gemengde kring proppen (wat qua aftakpuntentelling nét zou passen: 6 + 2 = 8) is bewust gekozen goede praktijk: een fout op de stopcontacten trekt dan niet meteen ook de verlichting mee uit.

### Voeding naar het tuinhuis: 30 m overbruggen

- **Kabel**: EXVB (of XGB) **3G6** (3 geleiders: fase, nul, aarde, elk 6 mm², voldoende voor deze eenfasige voeding), **ondergronds**, minstens **60 cm diep**, enkelvoudig gelegd (niet gebundeld met andere leidingen).
- **Doorsnede**: bepaald door de **spanningsval** over 30 m, niet enkel door de minimale doorsnede uit tabel 4.11. Met een gecombineerde ontwerpstroom van 20 A (stopcontactkring) + 10 A (verlichtingskring) = 30 A (zonder gelijktijdigheidsfactor, dus het ongunstigste geval):
  - 4 mm² → spanningsval ≈ 4,4%
  - **6 mm² → spanningsval ≈ 2,9%** (gekozen doorsnede, met voldoende marge binnen de +10%/-8%-tolerantie)
  - 10 mm² → spanningsval ≈ 1,8%

### Aarding: PE meekomt vanuit de woning

De aarde (PE) van het tuinhuis komt gewoon mee vanuit de bestaande aarding van de woning, via de 3G6-kabel. Geen eigen, lokale aardingspen nodig voor dit tuinhuis: de installatie blijft op die manier één consistente aarding delen met de rest van de woning.

### Het tuinhuisbordje zelf: één gecombineerd toestel aan het begin

In plaats van een aparte automaat (voor de kabel) en een aparte differentieel (als hoofdschakelaar) te combineren, gebruiken we hier **1 differentieelautomaat**.

- **Differentieelautomaat, 2P, Type A, 30 mA, 25 A**: dit ene toestel is tegelijk de overstroombeveiliging van de 6 mm²-voedingskabel, de 30 mA-bescherming, én de hoofdschakelaar-functie van het tuinhuisbordje (dat mag: een hoofdschakelaar van een onderverdeelbord mag een gewone schakelaar, een differentieel, of een automaat zijn).
- **Waarom 25 A, terwijl de twee kringen erachter samen 20 A + 10 A = 30 A kunnen vragen?** Dit is een bewuste keuze **mét gelijktijdigheidsfactor**: in de praktijk trekken de stopcontactkring en de verlichtingskring zelden allebei tegelijk hun volle, maximale stroom. Bij gelijktijdig piekgebruik van beide kringen zal deze 25 A-differentieelautomaat wel eerder afschakelen dan de kringautomaten zelf, dat is het bewuste compromis van deze keuze.
- Daarna **2 automaten**: 20 A voor de stopcontactkring, 10 A voor de verlichtingskring.

### IP-graad buiten

Het stopcontact en het lichtpunt buiten zijn niet beschut (geen overstek), dus kiezen we voorzichtig voor **IP65** (volledig stofdicht, bestand tegen waterstralen), in plaats van het minimum van IP44 dat voor een beschutte plaats zou volstaan.

### Materiaallijst voor dit voorbeeld

| Onderdeel | Aantal | Opmerking |
|---|---|---|
| Onderverdeelbord (wandmontage, tuinhuis) | 1 | |
| Differentieelautomaat 2P, Type A, 30 mA, 25 A | 1 | hoofdschakelaar + overstroom- + aardlekbeveiliging van het tuinhuisbordje |
| Automaat 20 A | 1 | stopcontactkring |
| Automaat 10 A | 1 | verlichtingskring |
| EXVB-kabel 3G6 | ±32 m | ondergronds, met reserve, aarde komt mee vanuit de woning |
| VOB/XVB 2,5 mm² | naar behoefte | bekabeling stopcontactkring binnen het tuinhuis |
| VOB/XVB 1,5 mm² | naar behoefte | bekabeling verlichtingskring binnen het tuinhuis |
| Stopcontact, dubbel, geaard | 3 | boven het werkblad |
| Stopcontact, enkel, geaard | 2 | overige binnenpunten |
| Stopcontact, IP65 | 1 | buiten |
| Lichtpunt-aansluiting | 1 | binnen |
| Lichtpunt-aansluiting, IP65 | 1 | buiten |
| Serieschakelaar | 1 | binnen geplaatst, bedient beide lichtpunten apart |
| Adereindhulzen | naar behoefte | voor de soepele bedrading in het bordje |

### In Trikker

Dit voorbeeld teken je exact volgens de vaste volgorde van hierboven: eerst het **eendraadschema** (2 kringen vanaf het tuinhuisbordje, gevoed vanuit een nieuwe stroombaan op het bestaand eendraadschema van de woning), dan het **situatieplan** (het tuinhuis als aparte pagina, met de stopcontacten, lichtpunten en de serieschakelaar op hun werkelijke plaats), en tot slot laat je Trikker de **materiaallijst** genereren, die je dan naast de voorbeelden van hierboven (Gamma, Hubo, Brico, Groothandel.be, Zelektro) kan leggen om een bestellijst op te maken.

## Waar vind je hulp?

De volledige handleiding zit **ingebouwd in het programma zelf**: open ze via het tabblad "Extra", of druk op **F1**. Deze handleiding volgt automatisch de versie die je geïnstalleerd hebt, dus de schermafbeeldingen kloppen altijd met wat je ziet. Bijkomend vind je op de website van Trikker een FAQ-pagina met enkele downloadbare voorbeeldbestanden (bijvoorbeeld een schema met zonnepanelen, een noodgenerator of een hoofdverdeling) als extra leermateriaal.

