# Scenario's

Het BRO berichtenverkeer kent de volgende scenario's

De interactiepatronen worden sequentiediagrammen afgebeeld.

## Registreren
De verwerking van een registratieverzoek verloopt geheel automatisch en volgens een vaste opeenvolging van stappen. Dit is waar het in het kort op neerkomt:

1. De dataleverancier stuurt vanuit zijn systeem een registratieverzoek met daarin een brondocument. Het systeem van de BRO voert een toegangscontrole uit.
2. Wanneer toegang tot het systeem van de BRO is verkregen, begint de controle van het verzoek en wordt onder meer vastgesteld of het verzoek inhoudelijk aan de gestelde eisen voldoet.
3. Wanneer de inhoudelijke controle fouten oplevert, wordt het verzoek afgewezen en ontvangt het systeem van de dataleverancier een bericht van afwijzing.
4. Wanneer de inhoudelijke controle geen fouten oplevert en er geen technische problemen zijn, wordt het registratieverzoek door het systeem van de BRO geaccepteerd. De aangeboden gegevens worden met de gegevens die de BRO zelf genereert vastgelegd. Het BRO-systeem stuurt het systeem van de dataleverancier als antwoord het bericht dat diens registratieverzoek is verwerkt.

De stappen en de bijbehorende berichten voor het registeren van gegevens worden in het onderstaande sequentiediagram getoond.


Het resultaat van de verwerking is dat het brondocument in het register brondocumenten ondergrond is opgenomen, dat de gegevens eruit zijn gehaald en vastgelegd zijn in de registratie ondergrond. De gegevens zijn dan voor eenieder beschikbaar.

Het verzoek van de dataleverancier en het antwoord dat de BRO daarop normaliter geeft worden berichten genoemd. In het geval zich technische problemen voordoen wordt het antwoord een melding genoemd.

## Corrigeren
De verwerking van een correctieverzoek verloopt iets anders dan dat van een registratieverzoek. De eerste stappen in de verwerking zijn hetzelfde, maar nadat het BRO-systeem heeft gecontroleerd of alles goed is, neemt de registratiebeheerder de controle over. 
Dit is waar het in het kort op neerkomt:

1.	De dataleverancier stuurt vanuit zijn systeem een correctieverzoek met daarin een brondocument.
2.	Het systeem van de BRO voert een toegangscontrole uit.
3.	Wanneer toegang tot het systeem van de BRO is verkregen, begint de controle van het verzoek en wordt onder meer vastgesteld of het verzoek inhoudelijk aan de gestelde eisen voldoet. 
o	Wanneer de inhoudelijke controle fouten oplevert, wordt het verzoek afgewezen en ontvangt het systeem van de dataleverancier een bericht van afwijzing.
4.	Wanneer de inhoudelijke controle geen fouten oplevert en er geen technische problemen zijn, wordt het correctieverzoek door het systeem van de BRO geaccepteerd. Vervolgens neemt de registratiebeheerder de verwerking over. Hij beoordeelt de reden van het correctieverzoek en de gevolgen die het heeft voor de informatie in de registratie ondergrond .
o	Indien zijn beoordeling aangeeft dat er iets fout gaat, ontvangt de dataleverancier een e-mail waarin de registratiebeheerder toelicht waarom hij het verzoek heeft moeten afwijzen.
5.	Wanneer de registratiebeheerder geen problemen ziet, wordt het verzoek doorgeleid. De aangeboden gegevens worden, met de gegevens die de BRO zelf genereert, vastgelegd. Het BRO-systeem stuurt de dataleverancier per e-mail bericht dat het correctieverzoek is verwerkt.

Het resultaat van de verwerking is dat het brondocument in het register brondocumenten ondergrond is opgenomen, dat de gegevens eruit zijn gehaald en dat de onjuiste gegevens in de registratie ondergrond zijn verbeterd. De gegevens zijn dan voor eenieder beschikbaar.

De stappen en de bijbehorende berichten voor het corrigeren van gegevens worden in het onderstaande sequentiediagram getoond.


## Afnemen
