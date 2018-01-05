# Algemene principes




## Interactiepatronen

<mark>Bij het interactiepatroon verzoek-respons is er een onderscheid tussen synchroon en asynchroon berichtenverkeer. Bij synchroon berichtenverkeer wordt de respons verwacht op de verbinding waarover het bericht is verzonden. De verzender wacht, totdat de respons over die verbinding is ontvangen of oordeelt dat er.</mark>

## Authenticatie en autorisatie

Een organisatie kan niet zomaar gegevens aan de BRO aanbieden. Een organisatie moet zich eerst als _dataleverancier_ bij de registerbeheerder hebben laten registreren en de registratie is gekoppeld aan een bepaald type registratieobject. Om de grondwatermonitoringput aan te mogen bieden moet een organisatie zich als dataleverancier van de grondwatermonitoringput laten registreren.

Wanneer het om een bronhouder gaat die zelf gegevens wil aanbieden, is er sprake van een bilaterale overeenkomst en kan de bronhouder zich direct als dataleverancier laten registreren. Wanneer een intermediaire partij namens een bronhouder gegevens wil aanleveren, is sprake van een overeenkomst tussen drie partijen.

De gegevens van de grondwatermonitoringput worden altijd via de innamewebservice aangeboden. De dataleverancier die de innamewebservice wil gebruiken moet over software beschikken die de webservice kan aanroepen. Met de eigen software heeft hij dan direct toegang tot het systeem van de basisregistratie ondergrond, het BRO-systeem, en kan hij snel en op betrouwbare wijze gegevens aanbieden.

Om zich bij de registerbeheerder als gebruiker van de webservice te laten registreren, moet de organisatie van de dataleverancier beschikken over een PKIoverheid services certificaat.

## Uitwisselformaat

