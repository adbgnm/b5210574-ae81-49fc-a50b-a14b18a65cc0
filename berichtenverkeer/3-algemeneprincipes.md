# Algemene principes

## Authenticatie en autorisatie
Een organisatie kan niet zomaar gegevens aan de BRO aanbieden. Een organisatie moet zich eerst als _dataleverancier_ bij de registerbeheerder hebben laten registreren en de registratie is gekoppeld aan een bepaald type registratieobject. Om de grondwatermonitoringput aan te mogen bieden moet een organisatie zich als dataleverancier van de grondwatermonitoringput laten registreren.

Wanneer het om een bronhouder gaat die zelf gegevens wil aanbieden, is er sprake van een bilaterale overeenkomst en kan de bronhouder zich direct als dataleverancier laten registreren. Wanneer een intermediaire partij namens een bronhouder gegevens wil aanleveren, is sprake van een overeenkomst tussen drie partijen.

De gegevens van de grondwatermonitoringput worden altijd via de innamewebservice aangeboden. De dataleverancier die de innamewebservice wil gebruiken moet over software beschikken die de webservice kan aanroepen. Met de eigen software heeft hij dan direct toegang tot het systeem van de basisregistratie ondergrond, het BRO-systeem, en kan hij snel en op betrouwbare wijze gegevens aanbieden.

Om zich bij de registerbeheerder als gebruiker van de webservice te laten registreren, moet de organisatie van de dataleverancier beschikken over een PKIoverheid services certificaat.

## Melding en bericht

Het verzoek van de dataleverancier en het antwoord dat de BRO daarop normaliter geeft worden _berichten_ genoemd. In het geval zich technische problemen voordoen wordt het antwoord een _melding_ genoemd.

## Uitwisselformaat
De gegevens die via de innamewebservice aan de BRO worden overgedragen staan in het IMBRO-XML formaat. Het IMBRO-XML formaat is de gegevensdefinitie omgezet naar de technische taal die voor de uitwisseling van gegevens met het systeem van de BRO gebruikt wordt. De technische uitwerking wordt toegelicht in de koppelvlakbeschrijving van de innamewebservice.

## Corrigeren
Voor het verbeteren van onjuistheden in de geregistreerde gegevens van een grondwatermonitoringput zijn verschillende typen verzoeken nodig. Dat komt doordat de verschillende registratieverzoeken elkaar netjes moeten opvolgen in de tijd om de materiële geschiedenis van de put in de registratie ondergrond correct op te bouwen. Een dataleverancier kan zich op allerlei manieren vergissen. Hij kan onjuiste gegevens aanleveren, maar ook vergeten een verzoek op tijd aan te bieden of een fout maken in een datum die in het brondocument staat. 

Er worden vier typen correctieverzoeken onderscheiden en dat zijn:
•	het verzoek gegevens te vervangen,
•	het verzoek gegevens in te voegen,
•	het verzoek gegevens te verwijderen, 
•	het verzoek gegevens te verplaatsen. 

De verschillende typen correctieverzoeken worden net als de registratieverzoeken via de innamewebservice aangeboden en de gegevens en controles verschillen per type verzoek. 

## Interactiepatronen
<mark>Bij het interactiepatroon verzoek-respons is er een onderscheid tussen synchroon en asynchroon berichtenverkeer. Bij synchroon berichtenverkeer wordt de respons verwacht op de verbinding waarover het bericht is verzonden. De verzender wacht, totdat de respons over die verbinding is ontvangen of oordeelt dat er.
</mark>
