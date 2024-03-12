# Opdracht Vélo

## Projectbeschrijving

Dit project is gericht op het bouwen van een reeks applicaties voor het beheren van een gedeeld fietssysteem. De applicatie moet in staat zijn om fietsen te registreren, verhuren en retourneren, en ook om klantgegevens bij te houden.

Je bouwt een simulatietool voor het fietsdeelsysteem "Velo" van de stad Antwerpen. Je vindt een JSON-dataset met startinformatie op deze locatie: [Open Data Stad Antwerpen - Velo's](https://portaal-stadantwerpen.opendata.arcgis.com/datasets/velo/explore).

Een basisuitleg over het deelsysteel vind je op [Wikipedia](https://nl.wikipedia.org/wiki/Velo_Antwerpen) en op de [officiële website](https://www.velo-antwerpen.be/).

## Technische vereisten

1. De applicatie moet worden ontwikkeld met Python, met behulp van het Flask-framework.
2. De applicatie moet een PostgreSQL-database gebruiken om gegevens op te slaan.
3. De applicatie moet een gebruikersvriendelijke interface hebben.

### Taken

1. Analyseer de huidige bedrijfsprocessen om de vereisten voor de applicatie te begrijpen.
2. Ontwerp de database en de applicatiearchitectuur.
3. Implementeer de applicatie volgens het ontwerp.
4. Test de applicatie grondig om ervoor te zorgen dat deze correct werkt.
5. Documenteer uw code en het gebruik van de applicatie.

### Functionele vereisten

- Je bouwt een realistisch model bestaande uit objecten van minstens de volgende elementen: (fiets-)stations, slots (ook plaatsen genoemd), fietsen, gebruikers, fietstransporteurs, loggen van fietsgebruik.
    - Stations bevatten een aantal plaatsen of slots, fietsen kunnen gekoppeld zijn aan een slot enz...
    - Fietstransporteurs zijn de vrachtwagens die rondrijden door de stad en in bulk fietsen verdelen van volle stations naar legere stations. Je modelleert ze als een bijzondere soort gebruikers.
    - Je logt alle verplaatsingen en houdt ze bij in objecten die je via compositie bindt aan de juiste objecten.
- Bij de eerste start van je toepassing creëer je aan de hand van de JSON-dataset een “reële” situatie (er zijn bvb. ca. 4200 fietsen, 309 stations en +55000 gebruikers).
    - Je vult deze set aan met eigen data, je genereert bvb random namen en familienamen voor gebruikers.
    - Je zorgt ervoor dat de data wordt opgeslagen en bijgehouden in één of meerdere bestanden. Start je de toepassing opnieuw dan geef je de keuze om opnieuw te beginnen of om verder te gaan vanaf de bestaande situatie. 
- De interface is een webapplicatie. Je zorgt er voor dat de toepassing relatief gebruiksvriendelijk is.
    - Acties die manueel moeten kunnen geïnitieerd worden zijn het ontlenen van (een) fiets(en), het terug inchecken van (een) fiets(en) voor zowel gebruikers als transporteurs.
    - Je zorgt ook voor een simulatiemodus waarbij je de tijd kan versnellen en het registreren van verplaatsingen doorheen de stad kan automatiseren. De simulatiemodus kan worden gestart vanuit de terminal-interface, maar ook door de applicatie te starten met “-s” argument.
- Je mag uiteraard extra functionaliteit toevoegen bovenop het gevraagde en gebruik maken van Python/web-libraries.

## Tijdlijn

De verwachte tijdlijn voor dit project is 8 weken. We verwachten dat je regelmatig updates geeft over uw voortgang.

## Hoe en wat dien je in?

- Je dient een .zip-bestand in met als naam `2324_python_AchternaamVoornaam_stageopdracht.zip`
- Je werkt met een virtual environment (.venv) en lijst gebruikte libraries op in een requirements.txt bestand.
- Je stuurt de .venv-folder zelf niet mee!
- Je maakt ook een folder reflectie aan met daarin een markdown (.md) bestand waarin je een reflectieverslag maakt over je toepassing. Je beschrijft de werking, de features en de keuzes die je hebt gemaakt. Je beschrijft tot slot ook kort de eventuele moeilijkheden die je hebt ervaren, en eventuele problemen die je niet hebt kunnen oplossen.

## Hulpmiddelen

Je kan vragen stellen en er worden tips en bijkomende uitleg gegeven tijdens de contactmomenten voorzien in de planning. Zorg dus zeker dat je er telkens bij bent.

## Deadline

Je dient deze opdracht in uiterlijk op 31 mei 2024.