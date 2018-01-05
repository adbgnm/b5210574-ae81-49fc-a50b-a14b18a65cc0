# Ontwerpprincipes

## Actoren en systemen

De basisregistratie ondergrond is een systeem dat een schakel vormt in een informatieketen. 

Aan het begin van de keten staan bestuursorganen die opdracht geven tot de productie van gegevens, of zelf gegevens produceren. Die bestuursorganen worden _bronhouders_ genoemd. De geproduceerde gegevens worden door een _dataleverancier_ geleverd aan de beheerder van het systeem, de _registerbeheerder_. De bronhouder is verantwoordelijk voor de levering van gegevens. Hij kan besluiten zelf dataleverancier te zijn of andere partijen een machtiging voor levering te verlenen. De beheerder van de BRO registreert de aangeleverde gegevens en levert ze voor (her)gebruik door aan allerlei afnemers.


## Communicatie tussen twee systemen

De dataleverancier die voor het aanbieden van gegevens van de grondwatermonitoringput gebruik maakt van de innamewebservice, gebruikt via zijn eigen systeem algemene BRO-software die via het internet voor iedereen te vinden is. 
Het adres van de BRO-webservices is te vinden op www.broinfo.nl. 

De webservice zorgt ervoor dat het systeem van de data-leverancier een verzoek tot het innemen van gegevens aan het BRO-systeem kan aanbieden, zorgt voor de verwerking van het verzoek en geeft het resultaat daarvan als antwoord van de BRO terug aan het systeem van de dataleverancier (Figuur 2). 

## Inname

De dataleverancier biedt gegevens aan met het doel de gegevens op te laten nemen in de registratie ondergrond. Het proces van inname begint aan de kant van de dataleverancier met een verzoek. Vervolgens beoordeelt de basisregistratie ondergrond dat verzoek om, als alles goed is, de gegevens in het systeem op te nemen. Gaat er iets onverhoopt fout, dan wijst de basisregistratie ondergrond het verzoek af. In alle gevallen krijgt de dataleverancier een antwoord op het verzoek terug. 

De basisregistratie ondergrond handelt de verzoeken altijd per object af. Dat wil zeggen één grondwatermonitoringput tegelijk. Het begrip innameverzoek heeft in de context van de basisregistratie ondergrond altijd betrekking op één grondwatermonitoringput.

De gegevens die onderwerp zijn van een innameverzoek, vormen een geheel en dat wordt in de taal van de basisregistratie ondergrond een brondocument genoemd. Een brondocument bevat de gegevens die de dataleverancier van een bepaald object overdraagt aan de basisregistratie ondergrond. 

Er bestaan twee categorieën innameverzoeken. Het hangt er namelijk vanaf wat de dataleverancier precies beoogt. 
Wil een leverancier nieuwe gegevens aan de BRO overdragen die net beschikbaar zijn gekomen, of wil hij fouten verbeteren in de gegevens die al aanwezig zijn. In de basisregistratie ondergrond spreekt men van registratieverzoeken, resp. correctieverzoeken. 
De verwerking van registratieverzoeken verloopt anders dan van correctieverzoeken. 

Via een innameverzoek kan een dataleverancier niet alle gegevens van een registratieobject laten verwijderen. Verwijderen, of beter het uit registratie nemen van een object is een ingrijpende verandering in de registratie ondergrond, en daartoe kan pas worden besloten na zorgvuldig onderzoek. Het onderzoek begint bij de registratiebeheerder en uiteindelijk kan een object alleen na akkoord van de bronhouder uit registratie genomen worden. Het is bovendien goed om te weten dat de gegevens niet uit de registratie verwijderd worden. De gegevens blijven bestaan maar zijn niet langer voor gebruikers toegankelijk.

## Uitgifte

