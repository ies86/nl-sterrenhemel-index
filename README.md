# Sterrenhemel-index van Nederland, per gemeente

Voor alle 342 Nederlandse gemeenten: hoe donker de nachthemel er is (Bortle-klasse) en hoeveel
van de 219 bekendste sterrenhemelobjecten (Messier + Caldwell) er over het jaar gerekend goed te
zien zijn met een telescoop van 200 mm. Volledig berekend uit openbare bronnen, narekenbaar.

Gemaakt door [Telescoopwijzer](https://telescoopwijzer.nl/sterrenhemel-per-gemeente) (Orai Media).

## Methode (kort)

1. RIVM-raster "Berekende hemelhelderheid in de nacht, zonder bewolking" (model 2015, 250 m,
   kunstlicht in mcd/m2, publiek domein): mediaan van maximaal 25 rasterpunten in een 5x5-grid
   (stap 1 km) rond het PDOK-gemeentemiddelpunt.
2. Plus 0,28 mcd/m2 natuurlijke hemelachtergrond (RIVM Kentallen).
3. SQM = 20,08 - 2,5*log10(L), de door het RIVM zelf gepubliceerde omrekening.
4. SQM naar Bortle-klasse via de gangbare grenzen; objectentelling met de openbare formules van
   telescoopwijzer.nl/methode, op de breedtegraad van de gemeente.

IJkpunt: de dorpskern van Schiermonnikoog komt op 21,2 mag/arcsec2, tegen 21,4 gemeten door het
RIVM Meetnet destijds op een punt buiten het dorp; consistent binnen de marge.

## Eerlijke beperkingen

- Model uit 2015, geen actuele meting; onzekerheid ongeveer een halve klasse.
- Alleen Nederlandse lichtbronnen: grensgemeenten (Zuid-Limburg, Zeeuws-Vlaanderen, Twente,
  Oost-Groningen) zijn in werkelijkheid iets lichter dan berekend.
- Binnen een gemeente verschilt de hemel van kern tot buitengebied; dit is het middelpunt.

## Kolommen

gemeente; provincie; bortle (1-9); klasse (label); sqm_mediaan (mag/arcsec2, 1 decimaal,
indicatief); objecten_200mm (van de 219, jaarrond, makkelijk+matig); breedtegraad.

## Bronnen en licentie

Bronnen: [RIVM hemelhelderheid](https://data.overheid.nl/dataset/61269-berekende-hemelhelderheid-in-de-nacht--zonder-bewolking)
(CC Public Domain Mark 1.0), [RIVM Kentallen Schiermonnikoog](https://www.rivm.nl/sites/default/files/2018-11/Kentallen%20Schiermonnikoog.pdf),
[PDOK Locatieserver](https://www.pdok.nl/), [OpenNGC](https://github.com/mattiaverga/OpenNGC) (CC BY-SA 4.0).

Deze afgeleide dataset: **CC BY 4.0**, naamsvermelding "telescoopwijzer.nl".
