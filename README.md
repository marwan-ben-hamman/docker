# Installatieprocedure nodige tools

## Stap 1: Installeren docker desktop

Ga naar [de site van docker](https://www.docker.com/products/docker-desktop/) en volg daar de nodige installatiestappen om docker desktop te installeren

## Stap 2: Clone deze repository voor de nodige docker files lokaal te hebben

Maak een kopie van deze repository (download, clone, ...) om van de nodige docker files een lokale kopie te hebben. Onthou waar je deze files plaatst.
Deze repository bevat files voor twee versies van het hadoop ecosysteem:
- De default versie waardoor een hadoop-cluster met 4 datanodes opgestart wordt (docker-compose.yml)
- Een light versie waardoor een hadoop-cluster met 1 datanode opgestart wordt (docker-compose-light.yml)

In de stappen hieronder wordt vanuit gegaan dat je de default-versie volgt. Als je de andere versie wil gebruiken, moet je de andere compose file aanpassen.

## Stap 3: Pas de gewenste volumes aan

Pas de volgende zaken aan in de docker-compose.yml file

