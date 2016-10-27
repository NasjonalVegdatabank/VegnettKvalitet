# Skilt og feltstrekning

## Kontroll:
Kontroll av skiltplater mot feltstrekning.

Leser skiltplater med skiltnummer 
* 508.1 - Kollektivfelt, for buss
* 508.2 - Kollektivfelt for buss og drosje
* 509 - Sambruksfelt

Og identifiserer de som ikke har feltstrekning med samme vegident og angitt felt "K" innenfor 25 meter

Leser skiltplater med skiltnummer 
* 520 - Sykkelveg
* 521 - Sykkelfelt
* 521.2 - Sykkelfelt, midtstilt

Og identifiserer de som ikke har feltstrekning med samme vegident og angitt felt "S" innenfor 25 meter.
For skiltnummer 520 - Sykkelveg filtreres det på om det finnes skiltplate med skiltnummer 518 Gangveg på samme posisjon. Slike tilfeller er feil skilting av Gang- og sykkelveg, og tas ikke med i videre analyse. 

## Resultat:
Resultatene skrives til datomapper (eks 20161027) med følgende filer:
* Landsdekkende Excellark med fanser for avvik på kollektiv, avvik på sykkel + feil skilting på gang- og sykkelveg.
* Landsdekkende SpatialLite-database med en klasse for avvik på kollektiv og en for avvik på sykkel
* Fylkesvise feilfiler til bruk i GISLINE. 
