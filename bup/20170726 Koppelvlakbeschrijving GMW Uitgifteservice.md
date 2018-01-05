Basisregistratie Ondergrond (BRO) Koppelvlakbeschrijving

GMW Uitgiftewebservice

Colofon

|         | Bestuurskern Dir. Ruimtelijke Ontwikkeling Plesmanweg 1-6 Den Haag        |
|---------|---------------------------------------------------------------------------|
|         |                                                                           |
| Contact | Programmabureau BRO Directoraat-Generaal Ruimte en Water <bro@minienm.nl> |
|         |                                                                           |
| Versie  | 1.0.2                                                                     |
|         |                                                                           |
| Auteur  | TNO Geologische Dienst Nederland                                          |
|         |                                                                           |

**Inhoudsopgave**

[1 Inleiding 8](#inleiding)

[1.1 Doel en doelgroep 8](#doel-en-doelgroep)

[1.2 Gebruik van dit document 8](#gebruik-van-dit-document)

[1.3 Samenhang met andere formele documentatie
8](#samenhang-met-andere-formele-documentatie)

[1.4 Leeswijzer 9](#leeswijzer)

[1.5 Referenties 9](#referenties)

[1.6 Versiehistorie 10](#versiehistorie)

[1.7 Contact 10](#contact)

[2 Opvragen van grondwatermonitoringput
11](#opvragen-van-grondwatermonitoringput)

[2.1 Inleiding 11](#inleiding-1)

[2.2 Communicatie tussen twee systemen 11](#communicatie-tussen-twee-systemen)

[2.3 Communicatiestandaarden 11](#communicatiestandaarden)

[2.3.1 Gegevens- en berichtenstandaarden 12](#gegevens--en-berichtenstandaarden)

[2.3.2 Logistieke standaard 12](#logistieke-standaard)

[2.3.3 Netwerkstandaard 13](#netwerkstandaard)

[2.4 Toegangscontrole 13](#toegangscontrole)

[3 API voor het opvragen van grondwatermonitoringput
14](#api-voor-het-opvragen-van-grondwatermonitoringput)

[3.1 Inleiding 14](#inleiding-2)

[3.2 Operaties 14](#operaties)

[3.3 Verwerking 14](#verwerking)

[3.4 Berichten bij opvragen kengegevens 16](#berichten-bij-opvragen-kengegevens)

[3.4.1 Request: verzoek tot levering van kengegevens
16](#request-verzoek-tot-levering-van-kengegevens)

[3.4.2 Response: bericht van afwijzing 16](#response-bericht-van-afwijzing)

[3.4.3 Response: bericht van verzending 17](#response-bericht-van-verzending)

[3.5 Berichten bij opvragen gegevens 17](#berichten-bij-opvragen-gegevens)

[3.5.1 Request: verzoek tot levering 17](#request-verzoek-tot-levering)

[3.5.2 Response: bericht van afwijzing 18](#response-bericht-van-afwijzing-1)

[3.5.3 Response: bericht van verzending 18](#response-bericht-van-verzending-1)

[3.6 Berichten bij technische fouten 19](#berichten-bij-technische-fouten)

[3.6.1 Softwarefout 19](#softwarefout)

[3.6.2 Systeemfouten 19](#systeemfouten)

[4 Modellering van het interface 20](#modellering-van-het-interface)

[4.1 Packagestructuur 20](#packagestructuur)

[4.2 Modelleerregels 21](#modelleerregels)

[4.2.1 CodeList 21](#codelist)

[4.2.2 DataType 21](#datatype)

[4.2.3 Enumeration 21](#enumeration)

[4.2.4 FeatureType 22](#featuretype)

[4.2.5 Type 22](#type)

[4.2.6 Union 22](#union)

[4.2.7 Voidable 22](#voidable)

[5 Package dsgmw – de uitgiftewebservice interface
23](#package-dsgmw-de-uitgiftewebservice-interface)

[5.1 De WSDL 23](#de-wsdl)

[5.1.1 Types 23](#types)

[5.1.2 Message 24](#message)

[5.1.3 PortType 24](#porttype)

[5.1.4 Binding 24](#binding)

[5.1.5 Service 24](#service)

[5.2 De XSD-bestanden 24](#de-xsd-bestanden)

[6 Package dsgmw-messages – de berichten XSD
25](#package-dsgmw-messages-de-berichten-xsd)

[6.1 DispatchCharacteristicsRequest 25](#dispatchcharacteristicsrequest)

[6.1.1 VerticalPositionRange 26](#verticalpositionrange)

[6.2 DispatchDataRequest 26](#dispatchdatarequest)

[6.2.1 DataToBeDelivered 26](#datatobedelivered)

[6.3 DispatchCharacteristicsResponse 27](#dispatchcharacteristicsresponse)

[6.3.1 DispatchCharacteristics 27](#dispatchcharacteristics)

[6.3.2 Characteristics 28](#characteristics)

[6.3.3 DiameterRange 29](#diameterrange)

[6.3.4 ScreenPositionRange 29](#screenpositionrange)

[6.3.5 StatusOverview 29](#statusoverview)

[6.4 DispatchDataResponse 29](#dispatchdataresponse)

[6.4.1 DispatchData 30](#dispatchdata)

[6.4.2 ElectrodeData 30](#electrodedata)

[6.4.3 EventData 31](#eventdata)

[6.4.4 EventName 31](#eventname)

[6.4.5 GeoOhmCable 31](#geoohmcable)

[6.4.6 GroundwaterMonitoringWell 32](#groundwatermonitoringwell)

[6.4.7 IntermediateEvent 33](#intermediateevent)

[6.4.8 MonitoringTube 33](#monitoringtube)

[6.4.9 Screen 34](#screen)

[6.4.10 TubeData 34](#tubedata)

[6.4.11 WellData 35](#welldata)

[6.4.12 WellHistory 35](#wellhistory)

[7 Package gmwcommon 36](#package-gmwcommon)

[7.1 Codelijsten 36](#codelijsten)

[7.2 DeliveredLocation 36](#deliveredlocation)

[7.3 DeliveredVerticalPosition 37](#deliveredverticalposition)

[7.4 Electrode 37](#electrode)

[7.5 InsertedPart 37](#insertedpart)

[7.6 MaterialUsed 37](#materialused)

[7.7 Meetwaarden 38](#meetwaarden)

[7.8 PlainTubePart 39](#plaintubepart)

[7.9 SedimentSump 39](#sedimentsump)

[8 Package brocommon 40](#package-brocommon)

[8.1 AbortReason 40](#abortreason)

[8.2 Area 40](#area)

[8.3 Characteristics 40](#characteristics-1)

[8.4 ChamberOfCommerceNumber 41](#chamberofcommercenumber)

[8.5 Circle 41](#circle)

[8.6 CoordinateTransformation 41](#coordinatetransformation)

[8.7 CorrectionRequest 42](#correctionrequest)

[8.8 CriteriaSet 42](#criteriaset)

[8.9 CriterionError 42](#criterionerror)

[8.10 DatePeriod 43](#dateperiod)

[8.11 DeregisteredObject 43](#deregisteredobject)

[8.12 DispatchDataRequest 43](#dispatchdatarequest-1)

[8.13 DispatchResponse 44](#dispatchresponse)

[8.14 Enumeraties 44](#enumeraties)

[8.15 IntakeResponse 45](#intakeresponse)

[8.16 ParseFault 46](#parsefault)

[8.17 PartialDate 47](#partialdate)

[8.18 Radius 48](#radius)

[8.19 RegistrationHistory 48](#registrationhistory)

[8.20 RegistrationObject 48](#registrationobject)

[8.21 RegistrationObjectCode 49](#registrationobjectcode)

[8.22 RegistrationRequest 49](#registrationrequest)

[8.23 RegistrationStatus 50](#registrationstatus)

[8.24 SOAP Fault 50](#soap-fault)

[8.25 SourceDocumentError 51](#sourcedocumenterror)

[8.26 StandardizedLocation 51](#standardizedlocation)

[9 Package gml-profile 53](#package-gml-profile)

[9.1 AbstractFeature 53](#abstractfeature)

[9.2 AbstractGML 53](#abstractgml)

[9.3 CodeWithAuthority 53](#codewithauthority)

[9.4 Doublelist 54](#doublelist)

[9.5 Envelope 55](#envelope)

[9.6 Measure 55](#measure)

[9.7 Point 56](#point)

[9.8 TM\_TimeInstant 57](#tm_timeinstant)

[9.9 TM\_Position 57](#tm_position)

[10 Package xlink-profile 59](#package-xlink-profile)

[10.1 Href 59](#href)

[10.2 HrefType 59](#hreftype)

[10.3 SimpleAttrs 59](#simpleattrs)

[10.4 Type 59](#type-1)

[10.5 TypeType 60](#typetype)

[11 Bijlagen 61](#bijlagen)

[11.1 Bijlage A: Vertaalslag Engels – Nederlands
61](#bijlage-a-vertaalslag-engels-nederlands)

[11.1.1 A1: dsgmw-messages 61](#a1-dsgmw-messages)

[11.1.2 A2: gmwcommon 64](#a2-gmwcommon)

[11.1.3 A3: brocommon 64](#a3-brocommon)

[11.1.4 A4: Domeinen van het type codelijst
66](#a4-domeinen-van-het-type-codelijst)

[11.2 Bijlage B: Voorbeeldberichten 67](#bijlage-b-voorbeeldberichten)

[11.2.1 DispatchCharacteristicsRequest 67](#dispatchcharacteristicsrequest-1)

[11.2.2 DispatchDataRequest 67](#dispatchdatarequest-2)

[11.2.3 DispatchDataResponse – gebruiksfout
68](#dispatchdataresponse-gebruiksfout)

[11.2.4 Softwarefout 68](#softwarefout-1)

[11.2.5 Systeemfout 68](#systeemfout)

Inleiding
=========

Dit document beschrijft het koppelvlak van de uitgiftewebservice voor het
registratieobject grondwatermonitoringput (GMW) voor de Basisregistratie
Ondergrond (BRO). Deze koppelvlakbeschrijving gaat in op de technische werking
van het koppelvlak om GMW-gegevens uit te kunnen wisselen tussen het systeem van
de data-afnemer en het systeem van de BRO.

Doel en doelgroep
-----------------

Doel van dit document is inzicht bieden in de werking van de uitgiftewebservice.
Het proces van gegevensuitgifte zoals beschreven in het ‘Uitgiftehandboek
Grondwatermonitoringput’ (zie [www.broninfo.nl](http://www.broninfo.nl)) is in
dit document vertaald naar het technische koppelvlak van de webservice: de
Application Programming Interface (API).

Dit document richt zich op de technisch specialisten die de aansluiting
realiseren tussen de systemen van de data-afnemers en het systeem van de BRO.
Kennis van XML en webservices is daarvoor vereist. Het document is echter zo
geschreven dat overige belangstellenden de technische werking van het koppelvlak
kunnen volgen.

Gebruik van dit document
------------------------

Dit document is te gebruiken om zicht te krijgen in de werking van het
koppelvlak. Deze koppelvlakbeschrijving is onderdeel van een serie formele
documenten die de technisch inhoudelijke werking van de BRO beschrijven.

Om daadwerkelijk een systeem aan te sluiten op de BRO moet de ‘Handleiding voor
aansluiten op webservices’ worden gevolgd (zie www.broinfo.nl). Die handleiding
bevat voor zowel softwareontwikkelaars als andere betrokken medewerkers
praktische informatie en beschrijft de stappen van het aansluiten. Ook wordt in
de handleiding beschreven welke extra bestanden beschikbaar zijn, zoals
voorbeeld clients, om te gebruiken bij het aansluiten op de BRO.

Samenhang met andere formele documentatie
-----------------------------------------

Voor ieder registratieobject in de BRO worden de volgende formele, beschrijvende
documenten opgesteld:

-   een catalogus

-   de handboeken voor inname en uitgifte

-   de koppelvlakbeschrijvingen voor inname en uitgifte.

De *catalogus* beschrijft de inhoud van een registratieobject en vormt de basis
voor de andere beschrijvende documenten. In de catalogus staan de definities van
de gegevens die betrekking hebben op een registratieobject en alle regels
waaraan zij moeten voldoen.

De *handboeken* beschrijven het proces dat bij inname of uitgifte van gegevens
wordt doorlopen. Alle registratieobjecten kunnen aangeboden worden via
webservices. Bepaalde registratieobjecten kunnen ook aangeboden worden via een
innameloket. Bij uitgifte is de situatie anders en kan de afnemer voor alle
objecten kiezen tussen uitgifte via webservices of via DINOloket. In een
handboek staan ook de definities van de gegevens die betrekking hebben op het
proces van inname of uitgifte.

De *koppelvlakbeschrijvingen* zijn geschreven voor softwareontwikkelaars en zijn
bedoeld voor de partijen die de webservices gaan gebruiken. Op basis van de twee
vorige type documenten staat hierin beschreven hoe het registratieobject en de
processen van inname of uitgifte zijn vertaald naar het technische koppelvlak
dat is gerealiseerd door middel van webservices. De koppelvlak­beschrijving gaat
dus in op de technische kant van de overdracht van gegevens.

Deze documenten hangen samen zoals hierna afgebeeld.

![](media/e0943db3993e2c4973fa3a09b7a35283.png)

Leeswijzer
----------

Hoofdstuk 2 beschrijft de algemene technische werking van het koppelvlak van de
uitgiftewebservice. Dit hoofdstuk is bedoeld voor de lezer die een globaal idee
wil krijgen hoe de geautomatiseerde gegevensuitwisseling van de BRO werkt.

Hoofdstuk 3 beschrijft vervolgens het koppelvlak van de BHR uitgiftewebservice
in technische termen: de Application Programming Interface (API). De
functionaliteit voor opvragen van de kengegevens van een verzameling
registratieobjecten die voldoen aan bepaalde zoekcriteria en de functionaliteit
voor het opvragen van de gegevens van een bepaald registratieobject komen
daarbij aan bod.

De hoofdstukken 4 en verder beschrijven het UML-model van de uitgiftewebservice.
Dezelfde structuur is van toepassing op de WSDL en XSD-bestanden van de
uitgiftewebservice.

Bijlage A bevat de vertalingen van de berichten en de codelijsten van het Engels
naar het Nederlands. Deze bijlage is een praktisch hulpmiddel aangezien de
Engelstalige XML-berichten gebaseerd zijn op Nederlandse definities uit het
uitgiftehandboek en de catalogus.

Bijlage B bevat voorbeeldberichten om een beeld te krijgen hoe de berichten
eruit kunnen zien.

Referenties
-----------

| Titel                                                       | Vindplaats                                                    |
|-------------------------------------------------------------|---------------------------------------------------------------|
| [1] Nederlandse Overheid Referentie Architectuur 3.0 (NORA) | NORA, website                                                 |
| [2] Digikoppeling 3.0                                       | Logius, website                                               |
| [3] NEN3610:2011                                            | Geonovum, website                                             |
| [4] Guidance and profile of GML for use with Aviation Data  | OGC 12-028                                                    |
|                                                             | http://www.opengis.net/doc/dp/gml-aviation-guidance           |

Versiehistorie
--------------

| Versie | Datum           | Omschrijving                                                                                                                                                                           |
|--------|-----------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 0.7    | 17 oktober 2016 | Initiële versie                                                                                                                                                                        |
| 0.7.2  | 2 december 2016 | Bijgewerkt n.a.v. OGC profielen                                                                                                                                                        |
| 0.8    | 16 mei 2017     | Consolidatie met andere registratieobjecten.                                                                                                                                           |
| 1.0    | 21 juni 2017    | Bijgewerkt n.a.v. review commentaar.                                                                                                                                                   |
| 1.0.1  | 25 juli 2017    | Stereotype FeatureType toegevoegd aan RegistrationObject                                                                                                                               |
| 1.0.2  | 26 juli 2017    | Figuren in 6.3.2 en 6.4.6 vervangen i.v.m. toevoegen NITGCode en wellCode; tabel in 11.1.1 uitgebreid m.b.t. NITGCode en wellCode en tabel in 11.1.3 gecompleteerd i.r.t. hoofdstuk 8. |

Contact
-------

Algemene informatie, documentatie en voorbeeld XML berichten kunt u vinden op
www.broinfo.nl.

Als uw organisatie is aangemeld bij de BRO kunt u voor vragen, suggesties of
opmerkingen contact opnemen met de BRO Selfservicedesk via support.gdnnet.nl.

In alle andere gevallen kunt u contact opnemen met de BRO Servicedesk via
contact\@broinfo.nl.

Opvragen van grondwatermonitoringput
====================================

Inleiding
---------

Dit hoofdstuk beschrijft hoe het opvragen van gegevens van het
GMW-registratieobject werkt. Hierbij wordt ingegaan op de algemene technische
werking van het koppelvlak van de GMW uitgiftewebservice. Er wordt uitgelegd hoe
het systeem van de data-afnemer en het BRO-systeem communiceren en welke
standaarden worden gehanteerd. Dit geeft een beeld hoe de geautomatiseerde
gegevensuitwisseling met de BRO werkt.

Communicatie tussen twee systemen
---------------------------------

Een data-afnemer kan geautomatiseerd gegevens van het GMW-registratieobject
opvragen bij de BRO via de GMW uitgiftewebservice. Het systeem van de
dataleverancier stuurt hiervoor een verzoek (*request*) aan de GMW
uitgiftewebservice van de BRO. Het systeem van de BRO reageert op dit verzoek
met een antwoord (*response*). Deze *response* bevat het resultaat van de
verwerking van het *request*. Onderstaande afbeelding geeft dit schematisch
weer.

![](media/5d7fb3abe9e905b65a9f0e527829f5c8.png)

Via het verzoek aan de GMW uitgiftewebservice kunnen met verschillende
bewerkingen (*operaties*) verschillende gegevensverzamelingen worden opgevraagd.
Elke operatie heeft een eigen *request* en een eigen *response*. De GMW
uitgiftewebservice is daarmee het koppelvlak ofwel de Application Programming
Interface (API) voor de uitgifte van GMW.

Communicatiestandaarden
-----------------------

De communicatie tussen het systeem van de data-afnemer en het BRO-systeem
verloopt over een aantal lagen. In de volgende afbeelding is per laag aangegeven
welke communicatiestandaard van toepassing is.

![](media/8b681acc13187f6dd108d67f52c68408.png)

De keuzes van de communicatiestandaarden die zijn gebruikt bij de inrichting van
het BRO-systeem zijn gebaseerd op de NORA (Nederlandse Overheid Referentie
Architectuur [1]) en de Digikoppeling specificaties ([2]).

### Gegevens- en berichtenstandaarden

Omdat alle registratieobjecten van de BRO een relatie hebben met een locatie op
het aardoppervlak, zijn de gegevens en berichten volgens de NEN3610 standaard
([3]) gemodelleerd.

### Logistieke standaard

Als logistieke standaard is voor de BRO het 2W-be profiel van Digikoppeling
([2]) gehanteerd. Het koppelvlak is daarom gerealiseerd als een WUS-webservice
waarvoor een aantal onderliggende standaarden zijn voorgeschreven, waaronder
WSDL 1.0 en SOAP 1.1. In onderstaande afbeelding is dat schematisch weergegeven.

![](media/0fe1fe81fb73f04daa471958345a03ec.png)

Het WSDL-document (Web Service Definition Language) beschrijft in technische
termen de volledige API (Application Programming Interface) van de GMW
uitgiftewebservice (zie hoofdstuk 3). Het beschrijft de operaties, inclusief
*request* en *response*, maar ook het protocol (in dit geval SOAP) waarmee
*request* en *response* worden uitgewisseld en de URL waarop de webservice
benaderd kan worden.

SOAP (Simple Object Access Protocol) is een protocol voor het versturen van
berichten. Een SOAP bericht bestaat uit een *Envelope* met daarin de *Header* en
de *Body*. De *Body* bevat het eigenlijke XML-bericht dat uitgewisseld wordt.
Ieder XML-bericht dat als onderdeel van een SOAP-bericht met het BRO-systeem
uitgewisseld wordt, is beschreven in een aantal BRO XML-schema’s (XSD). Deze
structuur van een SOAP-bericht is in de volgende afbeelding samengevat.

![](media/3e498d142da3af63c5ed1cb793a4ead2.png)

De XML-schema’s (XSD) volgen de gegevensdefinities van de catalogus nauwkeurig,
maar soms leidt de toepassing van de NEN3610 standaard tot afwijkingen. Daar
waar wordt afgeweken van de catalogus wordt dat expliciet toegelicht. Omdat de
XSD is uitgewerkt in het Engels en de catalogus in het Nederlands is beschreven,
is in bijlage A een vertaling van de berichtgegevens opgenomen.

### Netwerkstandaard

Als netwerkstandaard wordt TCP/IP over het internet gehanteerd.

Toegangscontrole
----------------

Voordat een bericht terecht komt in een operatie van de applicatie laag, vindt
er een toegangscontrole plaats binnen de logistieke laag. Dit gebeurt conform de
Digikoppeling standaard (zie referentie [2]). De toegangscontrole bestaat uit
versleuteling, identificatie, authenticatie en autorisatie. Nadere details staan
beschreven in paragraaf 3.3.

API voor het opvragen van grondwatermonitoringput
=================================================

Inleiding
---------

In dit hoofdstuk wordt het koppelvlak in technische termen beschreven: de API
(Application Programming Interface). Hierbij staan de twee functionaliteiten van
de GMW uitgiftewebservice centraal: opvragen van kengegevens en opvragen van
gegevens.

Elke functionaliteit heeft verschillende operaties. Deze worden beschreven in
paragraaf 3.2. Paragraaf 3.3 beschrijft het patroon van verwerking van de
operaties. De daaropvolgende paragrafen beschrijven de mapping van de berichten
uit het uitgiftehandboek op *requests* en *responses* in de API. De inhoud van
de *requests/responses* wordt beschreven in hoofdstuk 4 en verder.

Operaties
---------

De API voor het opvragen van grondwatermonitoringput biedt de data-afnemer
basale functionaliteit. Deze functionaliteit wordt gerealiseerd door twee
operaties van de GMW uitgiftewebservice:

-   dispatchCharacteristics voor het opvragen van de kengegevens van
    grondwatermonitoring-putten, die voldoen aan bepaalde kenmerken.

-   dispatchData voor het opvragen van de gegevens van een bepaalde
    grond­water­moni­toring­put.

Onderstaande tabel bevat een samenvatting van de operaties en de bijbehorende
requests:

| Operatie                | Request                        | Response                        |
|-------------------------|--------------------------------|---------------------------------|
| dispatchCharacteristics | dispatchCharacteristicsRequest | dispatchCharacteristicsResponse |
| dispatchData            | dispatchDataRequest            | dispatchDataResponse            |

Elke operatie heeft een eigen *request* en *response*, die de verschillende
verzoeken en antwoorden realiseren die in het uitgiftehandboek beschreven zijn.
In de volgende paragrafen wordt deze mapping kort toegelicht.

Verwerking
----------

De verwerking van een uitgifteverzoek verloopt volgens een vast patroon. Een
uitgifte operatie van de GMW uitgiftewebservice begint bij het doen van een
uitgifteverzoek door middel van een *request* en eindigt met de *response*. Het
patroon van de verwerking van een uitgifte operatie is hieronder weergegeven.

![](media/562b5654e93df3c57390b0afb0ba996d.png)

Stap 1: Doen van een verzoek tot levering

Het initiatief om een operatie te beginnen ligt bij het systeem van de
data-afnemer. Dat roept de betreffende operatie van de uitgiftewebservice aan
met het *request* als parameter.

Stap 2: Uitvoeren toegangscontrole

Dit bestaat uit identificatie, authenticatie, versleuteling en autorisatie.

Voor de beveiliging van de gegevensuitwisseling worden, conform de Digikoppeling
specificaties, PKIoverheid services server certificaten gebruikt. Zowel de
data-afnemer als de BRO beschikt over een dergelijk certificaat. In het
certificaat is een **identificatie** op basis van 20 cijfers opgenomen die uniek
is voor de houder van het certificaat.

Op het moment dat het systeem van een data-afnemer een operatie aanroept van de
webservice van het BRO-systeem wisselen beide systemen eerst hun PKIoverheid
services server certificaten uit. Aan de hand van de identificatie in de
certificaten weten beide partijen met wie gegevens­uitwisseling plaatsvindt. De
techniek van het PKIoverheid services server certificaat garandeert dat de
identificatie in het certificaat ook daadwerkelijk van die partij is
(**authenticatie**).

Als authenticatie succesvol is verlopen, worden beide certificaten vervolgens
gebruikt om al het dataverkeer tussen de systemen te **versleutelen**. Deze
versleuteling maakt het voor derden onmogelijk om de data te lezen of te
wijzigen.

Voor het opvragen van gegevens bij het BRO-systeem zijn rechten nodig. Aan de
hand van de identificatie in het certificaat wordt bepaald of het systeem van de
data-afnemer **geautoriseerd** is de operatie uit te voeren. Als hierbij een
fout optreedt, ontvangt de data-afnemer een melding met een http-statuscode.

Als niet wordt voldaan aan de toegangscontrole, dan leidt dit tot:

-   Een http ‘401 Unauthorized’ foutmelding.

-   Of een ‘ssl error invalid certificate’ foutmelding.

-   Of een andere http-foutmelding met een http-statuscode anders dan ‘200 OK’.

Stap 3: Controleren verzoek

Als de toegangscontrole succesvol is verlopen, dan wordt het *request* technisch
en inhoudelijk gecontroleerd.

De technische controle vindt plaats door het *request* te valideren op basis van
de XSD. Als hierbij fouten gevonden worden, dan worden deze beschouwd als een
technische fout van het systeem van de data-afnemer en teruggegeven als een
*parseFault*.

De inhoudelijke controle vindt plaats door het *request* te controleren volgens
de regels die zijn gedefinieerd in de catalogus of het uitgiftehandboek
(*business rules*). Deze regels zijn niet in de XSD vastgelegd, maar worden
gecontroleerd door de programmatuur van het BRO-systeem. Voorbeelden van
controles zijn:

-   Is een waarde niet groter dan de toegestane maximale waarde?

-   Voldoet een waarde aan de toegestane waardes voor een gegeven?

Als hierbij fouten worden gevonden, dan worden deze beschouwd als een
gebruiksfout en teruggegeven in een *response* bericht.

Stap 4: Verzamelen van gegevens

Als alle controles succesvol zijn verlopen dan verzamelt het BRO-systeem de
opgevraagde gegevens en wordt het resultaat teruggegeven in een *response*
bericht.

Berichten bij opvragen kengegevens
----------------------------------

Bij het opvragen van kengegevens zijn drie berichten van toepassing: een verzoek
tot levering, een bericht van afwijzing en een bericht van verzending.

### Request: verzoek tot levering van kengegevens

Het verzoek tot levering van kengegevens wordt gerealiseerd door
*DispatchCharacteristicsRequest*. Onderstaande figuur geeft de mapping weer van
het verzoek tot levering in het uitgiftehandboek op het datatype
*DispatchCharacteristicsRequest* in dit document (zie paragraaf 6.1), zoals
gebruikt door de *dispatchCharacteristics* operatie (zie hoofdstuk 5).

![](media/14e7108a8225bf9f915f6b59d34d6668.png)

Het (platte) element *requestReference* is een voor de data-afnemer unieke
aanduiding van het request.

Het (gestructureerde) element *criteria* specificeert de afzonderlijke kenmerken
waaraan de registratieobjecten moeten voldaan.

Zie paragraaf 6.1 voor nadere details.

### Response: bericht van afwijzing

Het uitgiftehandboek benoemt als mogelijke reactie op een uitgifteverzoek een
bericht van afwijzing. De webservice gebruikt hiervoor een *response* van het
datatype *DispatchCharacteristicsResponse*.

![](media/cb63ad8ecfd52955a0511038eff6c3a8.png)

Het handboek definieert een aantal berichten als antwoord op een
uitgifteverzoek. In de SOAP webservice definities mag elk *request* slechts één
*response* hebben. Daarom is het element *responseType* toegevoegd, om de
betekenis van de *response* te duiden. In dit geval heeft het element
*responseType* de vaste waarde *rejection*.

De waarde van het element *requestReference* is overgenomen uit het *request*.
De waarde van de overige elementen wordt toegekend door de webservice. Het
element *rejectionReason* bevat een waarde uit de tabel met gebruiksfouten; zie
het uitgiftehandboek.

Als deze *response* wordt gegeven omdat er een of meer gebruiksfouten in het
element *criteria* in het *request* zijn geconstateerd, dan is de waarde van
*rejectionReason* “er zijn 1 of meer fouten geconstateerd in de
kenmerkenverzameling” en volgen er na dit element een of meer *criterionErrors*.

### Response: bericht van verzending

Het uitgiftehandboek benoemt als mogelijke reactie op een uitgifteverzoek een
bericht van verzending. De webservice gebruikt hiervoor een *response* van het
datatype *DispatchCharacteristicsResponse.*

![](media/a502cc418ed6cb4a5bdead49f35969d9.png)

Het handboek definieert een aantal berichten als antwoord op een
uitgifteverzoek. In de SOAP webservice definities mag elk request slechts één
*response* hebben. Daarom is het element *responseType* toegevoegd, om de
betekenis van de *response* te duiden. In dit geval heeft het element
*responseType* de vaste waarde *dispatch*.

De waarde van het element *requestReference* is overgenomen uit het *request*.
De waarde van de overige elementen wordt toegekend door de webservice. Het
tijdstip van verzending en het aantal uitgiftedocumenten staan in de elementen
*dispatchTime* en *numberOfDocuments*. De kengegevens van de objecten, die
voldoen aan de kenmerkenverzameling in het *request*, staan in de lijst met
*dispatchDocuments*.

Berichten bij opvragen gegevens
-------------------------------

Bij het opvragen van gegevens van een bepaald registratieobject zijn drie
berichten van toepassing: een verzoek tot levering, een bericht van afwijzing en
een bericht van verzending.

### Request: verzoek tot levering

Onderstaande figuur geeft de mapping weer van het uitgifteverzoek in het
uitgiftehandboek op het datatype *DispatchDataRequest* in dit document (zie
paragraaf 6.2), zoals gebruikt door de *dispatchData* operatie (zie hoofdstuk
5).

![](media/520fc60513229fb3051f664cdd5379e6.png)

Het element *requestReference* is een voor de data-afnemer unieke aanduiding van
het *request*.

Het element *broId* is de unieke aanduiding van het registratieobject waarvan de
gegevens worden opgevraagd.

Het element *dataToBeDelivered* geeft aan welke gegevens worden opgevraagd:

-   actueel: alleen de actuele gegevens van het registratieobject worden
    opgevraagd.

-   actueelHistorisch: naast de actuele gegevens worden ook de waarden die het
    registratieobject in het verleden heeft gehad, de materiële geschiedenis,
    opgevraagd.

Zie paragraaf 6.2 voor nadere details.

### Response: bericht van afwijzing

Het uitgiftehandboek benoemt als mogelijke reactie op een uitgifteverzoek een
bericht van afwijzing. De webservice gebruikt hiervoor een *response* van het
datatype *DispatchDataResponse*.

![](media/8ddef6b91acb470308abf4ac43ff816a.png)

Het handboek definieert een aantal berichten als antwoord op een
uitgifteverzoek. In de SOAP webservice definities mag elk *request* slechts één
*response* hebben. Daarom is het element *responseType* toegevoegd, om de
betekenis van de *response* te duiden. In dit geval heeft het element
*responseType* de vaste waarde *rejection*.

De waarde van het element *requestReference* is overgenomen uit het *request*.
De waarde van de overige elementen wordt toegekend door de webservice. Het
element *rejectionReason* bevat een waarde uit de tabel met gebruiksfouten; zie
het uitgiftehandboek.

### Response: bericht van verzending

Het uitgiftehandboek benoemt als mogelijke reactie op een uitgifteverzoek een
bericht van verzending. De webservice gebruikt hiervoor een *response* van het
datatype *DispatchDataResponse.*

![](media/3c0c7cbb9391860129dc48b5fae5f7de.png)

Het handboek definieert een aantal berichten als antwoord op een
uitgifteverzoek. In de SOAP webservice definities mag elk *request* slechts één
*response* hebben. Daarom is het element *responseType* toegevoegd, om de
betekenis van de *response* te duiden. In dit geval heeft het element
*responseType* de vaste waarde *dispatch*.

De waarde van het element *requestReference* is overgenomen uit het *request*.
De waarde van de overige elementen wordt toegekend door de webservice. Het
tijdstip van verzending staat in het elementen *dispatchTime*. Het element
*dispatchDocument* bevat de gegevens over de opgevraagde
grondwatermonitoringput.

Berichten bij technische fouten
-------------------------------

Er zijn twee soorten berichten mogelijk bij een technische fout: een
softwarefout of een systeemfout. In de volgende paragrafen wordt dit toegelicht.

### Softwarefout

Als bij de technische controle van het *request* fouten in het verzoek en/of het
brondocument worden gevonden (bijvoorbeeld het *request* is niet een welgevormd
XML bericht of het *request* voldoet niet aan de schemavalidatie), dan worden
deze beschouwd als een softwarefout in het systeem van de data-afnemer. Het
BRO-systeem stuurt dan een melding in de vorm van een *parseFault*. Zie
paragraaf 8.16 voor nadere details.

![](media/d33439738863ed795352c0a0dc300aa5.png)

### Systeemfouten

Tijdens de uitvoering van een operatie kan er een onverwachte fout optreden in
het BRO-systeem. Hiervoor kunnen verschillende oorzaken zijn, zoals het falen
van bepaalde software of hardware. Deze onverwachte fouten worden beschouwd als
een technische fout veroorzaakt door het BRO-systeem. De BRO stuurt dan een
bericht in de vorm van een generieke *SOAP:Fault*. Zie paragraaf 8.24 voor
nadere details.

Modellering van het interface
=============================

Dit hoofdstuk en de volgende hoofdstukken beschrijven in detail de interface van
de GMW uitgiftewebservice aan de hand van een UML-model.

Packagestructuur
----------------

De interface beschrijving is onderverdeeld in verschillende packages. Deze
paragraaf beschrijft de samenhang van de packages. Deze onderverdeling is ook
van toepassing op de WSDL en XSD-bestanden. De hoofdstukken 5 en verder
beschrijven elk een van de packages.

Onderstaande figuur geeft een overzicht van de packagestructuur.

![](media/fe1c5d074d8aa775a8feda4a6fea552c.emf)

De interfaces van de innamewebservice en de uitgiftewebservice zijn gemodelleerd
in de *isgmw* en *dsgmw* packages.

Om de beheerbaarheid van de modellen en de software te vergroten, is gestreefd
naar herbruikbaarheid van gemodelleerde gegevenstypes. Er is bijvoorbeeld veel
overlap in de gegevens in het registratieverzoek en de objectgegevens bij
uitgifte. Door deze overlappende gegevens onder te brengen in een
gemeenschappelijk model voor inname en uitgifte is hergebruik mogelijk.

De gegevenstypes voor de inname- respectievelijk uitgiftewebservice zijn
gemodelleerd in package *isgmw-messages* respectievelijk *dsgmw-messages*.

Herbruikbare gegevenstypes die specifiek zijn voor GMW zijn gemodelleerd in
package *gmwcommon*.

Gegevenstypes die herbruikbaar zijn voor alle registratieobjecten van de BRO
zijn gemodelleerd in *brocommon*.

GMW maakt verder op diverse manieren gebruik van concepten uit de GML-standaard
van de OGC (ISO 19136). Aan het gebruik van deze standaard kleven enkele
praktische bezwaren:

-   De standaard is omvangrijk en slechts een klein deel wordt gebruikt in de
    BRO.

-   De software om de standaard te ondersteunen is omvangrijk.

-   Het gebruik van de standaard is niet eenvoudig.

Om deze bezwaren weg te nemen zijn in overleg met GeoNovum profielen opgesteld.
Rand­voor­waarde bij het opstellen van de profielen was dat berichten die
voldoen aan de profielen ook moeten voldoen aan de OGC-standaarden. Het
GML-profiel is gemodelleerd in package gml-profile.

De volgende hoofdstukken beschrijven deze packages als gegevensmodel voor de GMW
uitgiftewebservice. De packages *isgmw* en *isgmw-messages* worden buiten
beschouwing gelaten, aangezien deze de innamewebservice betreffen.

Modelleerregels
---------------

In het UML-model worden de volgende stereotypes gebruikt om bepaalde
functionaliteit te duiden.

### CodeList

De catalogus maakt een onderscheid in beheerde en niet-beheerde enumeraties.

Het domein van een **beheerde enumeratie** is een uitbreidbare opsomming van
toegestane waarden. Er wordt voor een beheerde enumeratie gekozen als niet alle
waarden bekend zijn en uitbreiding mogelijk moet zijn (zie paragraaf 4.2.3 voor
niet-beheerde enumeraties).

Het stereotype *CodeList* wordt in UML gebruikt om aan te geven dat een datatype
een beheerde enumeratie is. In de XSD leidt dit tot een *complexType* wat een
restrictie is van het gml *complexType CodeWithAuthority* (zie paragraaf 9.3).

### DataType

Het stereotype *DataType* wordt in UML gebruikt om aan te geven dat een data
type een niet-identificeerbaar, gestructureerd data type is. In de XSD leidt dit
tot een *complexType* zonder een *gml:id* attribuut.

### Enumeration

De catalogus maakt een onderscheid in beheerde en niet-beheerde enumeraties.

Het domein van een **niet-beheerde enumeratie** is een vaste, limitatieve
opsomming van toegestane waarden. Er wordt voor een niet-beheerde enumeratie
gekozen als alle waarden bekend zijn en uitbreiding niet nodig is (zie paragraaf
4.2.1 voor beheerde enumeraties).

Het stereotype *Enumeration* wordt in UML gebruikt om aan te geven dat een
datatype een niet-beheerde enumeratie is. In de XSD leidt dit tot een
*simpleType* als restrictie van het type *string* met een lijst van benoemde
waarden. Voorbeeld:

| \<simpleType name=*"IndicationYesNoEnumeration"*\> \<restriction base=*"string"*\> \<enumeration value=*"ja"*\> \<enumeration value=*"nee"*\> \</restriction\> \</simpleType\> |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


### FeatureType

Het stereotype *FeatureType* wordt in UML gebruikt om aan te geven dat een
klasse een identificeerbaar fenomeen in de werkelijkheid representeert, dat
direct of indirect is geassocieerd met een locatie relatief ten opzichte van de
aarde. In de XSD leidt dit tot een *complexType* dat is afgeleid van
*AbstractFeature* uit het GML-profiel (zie paragraaf 9.1). In een XML-bericht
heeft een object van deze klasse een *gml:id* attribuut.

### Type

Het stereotype *Type* wordt in UML gebruikt om aan te geven dat een klasse een
identificeerbaar object anders dan een *FeatureType* (zie paragraaf 4.2.4)
representeert. In de XSD leidt dit tot een *complexType* dat is afgeleid van
*AbstractGML* uit het GML-profiel (zie paragraaf 9.2). In een XML-bericht heeft
een object van deze klasse een *gml:id* attribuut (zie paragraaf 9.1).

### Union

Het stereotype *Union* wordt in UML gebruikt om aan te geven dat in een
voorkomen precies een van de eigenschappen aanwezig is (polymorfisme). In de XSD
wordt dit gerealiseerd als een *choice*.

### Voidable

Het stereotype *Voidable* wordt in UML gebruikt om aan te geven dat een element
aanwezig is maar geen waarde heeft. De modellering in UML en XSD en het gebruik
in XML is afhankelijk van het datatype of domein van het betreffende attribuut:

-   Codelijst, enumeratie

    -   De uitwerking is opgenomen in de lijst met toegestane waarden.

    -   In het UML-model is het stereotype *Voidable* niet opgenomen.

    -   In een XSD-bestand krijgt zo’n element niet het attribuut
        *nilllable=”true”*.

    -   Als in een XML-bericht het element wordt opgenomen, dan heeft het
        element een waarde uit de codelijst.

-   Integer, double, string

    -   Het gegeven is aanwezig, maar heeft geen waarde.

    -   In het UML-model is het stereotype *Voidable* opgenomen voor deze
        situatie.

    -   In een XSD-bestand krijgt zo’n element het attribuut *nilllable=”true”*.

    -   In een XML-bericht wordt in voorkomende gevallen het element opgenomen,
        met een lege waarde en met het attributen *xsi:nil=”true”*.

    -   Er wordt geen onderscheid gemaakt in de waarden geen, onbekend, o.i.d.

-   PartialDate

    -   Voor IMBRO/A-gegevens kan de situatie zich voordoen, dat er wel een
        waarde is, maar dat deze onbekend is bij de dataleverancier.

        -   Voor deze situatie voorziet het UML-model de optie *voidReason* met
            als vaste waarde *onbekend*.

        -   In een XSD-bestand krijgt zo’n element niet het attribuut
            *nilllable=”true”*.

        -   In een XML-bericht wordt het element opgenomen, met als kind-element
            *voidReason* met als waarde *onbekend*.

    -   Daarnaast kan (tot nu toe alleen bij IMBRO/A) sprake zijn van het feit,
        dat het gegeven überhaupt geen waarde heeft.

        -   In het UML-model wordt het stereotype *Voidable* opgenomen.

        -   In een XSD-bestand krijgt zo’n element het attribuut
            *nilllable=”true”*.

        -   In een XML-bericht wordt het element opgenomen met een lege waarde
            (er is geen kind-element *voidReason* aanwezig).

Package dsgmw – de uitgiftewebservice interface
===============================================

De onderstaande figuur geeft het interface van de GMW uitgiftewebservice weer:

![](media/3d0640e7daed49d5deebbed8ac954063.emf)

Onderstaande tabel bevat een samenvatting van operaties met bijbehorende
datatype van het *request* en *response*:

| Operatie                | Request datatype               | Response datatype               |
|-------------------------|--------------------------------|---------------------------------|
| dispatchCharacteristics | DispatchCharacteristicsRequest | DispatchCharacteristicsResponse |
| dispatchData            | DispatchDataRequest            | DispatchDataResponse            |

Zie hoofdstuk 6 voor de *request* en *response* datatypes uit de package
*dsgmw-messages*. Technische fouten (zie paragraaf 3.6) worden afgehandeld met
een *Fault* bericht uit de *SOAP*-package.

De WSDL 
--------

De GMW uitgiftewebservice wordt technisch volledig beschreven door de WSDL van
de GMW uitgiftewebservice (*dsgmw.wsdl)*. De onderdelen van dit bestand worden
hieronder kort toegelicht.

### Types

Het onderdeel *types* in een WSDL definieert een XML-schema met daarbinnen
XML-types en XML-elementen. Voor de GMW uitgiftewebservice zijn deze opgenomen
in een afzonderlijke berichten XSD (*dsgmw-messages.xsd*) die in het *types*
element wordt geïmporteerd.

### Message

Het onderdeel *message* in een WSDL specificeert de berichten die per operatie
worden uitgewisseld, uitgedrukt in parts. In de parts worden XML-elementen uit
het *types* onderdeel van de WSDL gebruikt. Voor elke operatie wordt een
*request* message en een *response* message gespecificeerd.

### PortType

Het onderdeel p*ortType* in een WSDL specificeert de beschikbare functionaliteit
van de webservice in de vorm van een of meer operaties (*operations)* met hun
*request* en *response* messages en de *parseFault*.

### Binding

Het onderdeel *binding* in een WSDL specificeert details over het
transportmechanisme dat gebruikt wordt voor de webservice, waaronder het
communicatieprotocol en het formaat van de input en de output. Digikoppeling
schrijft als binding SOAP 1.1, ‘document-literal wrapped’ met als transport
binding http voor. Voor elke operatie is de *style* ‘document’ en de *input* en
*output use* ‘literal’.

### Service

Het onderdeel *service* in een WSDL beschrijft volgens welke *portType* en op
welke URL de webservice gepubliceerd is.

De XSD-bestanden
----------------

In de XSD-bestanden worden alle XML types en elementen gedefinieerd die gebruikt
worden in de WSDL voor de GMW uitgiftewebservice. In alle XSD-bestanden van de
BRO wordt, conform de NEN3610 voorschriften, gebruik gemaakt van verschillende
XSD-bestanden van de internationale W3C en OGC-standaarden.

Deze schema’s worden in de navolgende hoofdstukken beschreven, elk schema in een
eigen hoofdstuk. De opbouw van een element of datatype in een schema wordt
afgebeeld in een diagram en waar relevant worden bijzonderheden in de tekst
toegelicht. Voor de inhoudelijke betekenis van de afzonderlijke gegevens wordt
verwezen naar het uitgiftehandboek en de catalogus van de GMW.

De XSD-bestanden zijn opgesteld in het Engels. De vertaling naar Nederlandse
termen die gebruikt worden in het uitgiftehandboek en in de catalogus staat in
Bijlage A (zie paragraaf 11.1).

Package dsgmw-messages – de berichten XSD
=========================================

De package dsgmw-messages bevat datatypes voor de *requests*, *responses*,
kenmerkenverzameling en uitgiftedocumenten voor de uitgifteverzoeken.

DispatchCharacteristicsRequest
------------------------------

Het *DispatchCharacteristicsRequest* bevat alleen een (plat) element
*requestReference* en een (gestructureerd) element *criteria*.

![](media/388c4966cf03720a74c143e24a3d45b0.emf)

Het element *criteria* van type *CriteriaSet* bevat een aantal optionele
elementen voor de selectiecriteria. Het datatype *CriteriaSet* in de package
*dsgmw-messages* is een specialisatie van *CriteriaSet* in de package
*brocommon* (zie paragraaf 8.8), waaraan enkele GMW specifieke elementen worden
toegevoegd.

Merk op dat *CriteriaSet* in de package *brocommon* een verplicht element *area*
bevat (zie paragraaf 8.2). Alleen kengegevens van registratieobjecten, waarvan
de gestandaardiseerde locatie (zie paragraaf 8.26) valt binnen het opgegeven
gebied, worden uitgeleverd.

Zie het uitgiftehandboek voor nadere details over de betekenis en toepassing van
de kenmerkenverzameling.

### VerticalPositionRange

Het datatype *verticalPositionRange* bevat een begin en eindwaarde, beiden van
het datatype *VerticalPosition* (zie paragraaf 7.7), zodat in de *criteriaSet*
een voorwaarde kan worden opgenomen waarbij de verticale positie van een
eigenschap van de put in het opgegeven bereik moet liggen.

![](media/2fa715f527bf243aefd4f25f55b25800.emf)

Merk op dat beide elementen verplicht zijn.

DispatchDataRequest 
--------------------

Het *DispatchDataRequest* is een specialisatie van de abstract klasse
*Dispatch­Data­Request* in de package *brocommon* (zie paragraaf 8.12), waaraan
het een element *dataToBeDelivered* toevoegt.

![](media/c72b221066f09e0ca1c577c071aa1a2b.emf)

Het element *dataToBeDelivered* geeft aan welke gegevens over het
registratieobject worden opgevraagd.

### DataToBeDelivered

Datatype met een niet-beheerde enumeratie (zie ook paragraaf 4.2.3) van
toegestane waarden.

![](media/1cb2080c72aef8c7bfd421237ab569a1.emf)

De betekenis van de waarden is als volgt:

-   *actueel*: alleen de actuele gegevens van het registratieobject worden
    opgevraagd.

-   *actueelHistorisch*: naast de actuele gegevens worden ook de waarden die het
    registratieobject in het verleden heeft gehad, de (volledige) materiële
    geschiedenis, opgevraagd.

DispatchCharacteristicsResponse
-------------------------------

Het *DispatchCharacteristicsResponse* is een specialisatie van
*DispatchResponse* in de package *brocommon* (zie paragraaf 8.13), waaraan het
een element *numberOfDocuments* en een optionele lijst met *dispatchDocuments*
toevoegt.

![](media/db4730023dc59269a0dae48d124665dd.emf)

Merk op dat *DispatchResponse* in *brocommon* naast de platte elementen ook een
optionele lijst met *criterionErrors* bevat. Zie voor nadere informatie hierover
en over welke elementen onder welke omstandigheden verwacht kunnen worden
paragraaf 3.4.2.

De kardinaliteit van de lijst met *dispatchDocuments* is onbegrensd
(*maxOccurs=”unbounded”*), maar het BRO-systeem beperkt de lijst softwarematig
tot maximaal 2000 uitgiftedocumenten.

### DispatchCharacteristics

Het datatype *DispatchCharacteristics* bevat de kengegevens van een
GMW-registratieobject.

![](media/7e862b1a93ba818120891e3b41b6f954.emf)

Het datatype heeft het stereotype *Union* (zie ook paragraaf 4.2.6), waarmee
wordt aangegeven dat het datatype polymorf is en dat voor ieder element een van
de twee mogelijke alternatieven uitgegeven zal worden:

-   met de naam *BRO\_DO* en van het datatype *DeregisteredObject* (zie
    paragraaf 8.11) met de kengegevens van een grondwatermonitoringput dat
    voldoet aan de criteria in het request en dat uit registratie is genomen.

-   met de naam *GMW\_C* en van het datatype *Characteristics* (zie volgende
    paragraaf) met de kengegevens van een grondwatermonitoringput dat voldoet
    aan de criteria in het request en dat niet uit registratie is genomen.

In de XSD is dit gerealiseerd als een *choice* uit een lijst van elementen met
paarsgewijs de naam en het datatype zoals aangegeven in bovenstaande figuur.
Merk op dat de naam van het alternatief opgenomen moet worden in het element
*dispatchDocument*; daarmee wordt bij een gegeven verzameling kengegevens
eenduidig bekend welk alternatief gekozen is voordat de feitelijke elementen van
dat alternatief aan bod komen. Voorbeeld:

| \<dispatchCharacteristicsResponse xmlns:brocom=*"http://www.broservices.nl/xsd/dsgmw/1.0"*  xmlns:brocom=*"http://www.broservices.nl/xsd/brocommon/3.0"*\> \<brocom:responseType\>dispatch\</brocom:responseType\> ... \<numberOfDocuments\>1\</numberOfDocuments\> \<dispatchDocument\> \<GMW\_C\> \<broId\>GMW123456789012\</broId\> ... \</GMW\_C\> \</dispatchDocument\> \</dispatchCharacteristicsResponse\> |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


### Characteristics

Het datatype *DispatchCharacteristics* bevat de kengegevens van een
GMW-registratieobject dat niet uit registratie is genomen.

![](media/cbd2caab0179f14dc340a84f5c1ab03a.emf)

Het type *Characteristics* is een specialisatie van *Characteristics* in de
package *brocommon* (zie paragraaf 8.3), waaraan het een aantal GMW specifieke
elementen en gerelateerde datatypes toevoegt.

De elementen *NITGCode* en *wellCode* zijn beiden optioneel, maar er wordt
altijd een van de twee uitgeleverd. De waarde voor *wellCode* wordt tijdens
inname door de BRO vastgelegd op basis van de aangeleverde waarde voor
*mapSheetCode* (zie Koppelvlakbeschrijving GMW innameservice).

Merk op dat een aantal elementen het stereotype *Voidable* heeft (zie paragraaf
4.2.7).

### DiameterRange

Het element *DiameterRange* geeft het interval aan waarbinnen de diameters van
de bovenkant van de monitoringbuizen liggen.

![](media/f8bb7984849f46a7784d8533eaa408cf.emf)

Het datatype van de kleinste en grootste diameter is een meetwaarde van het type
*Diameter* (zie paragraaf 7.7).

### ScreenPositionRange

Het element *ScreenPositionRange* geeft het interval aan waarbinnen de verticale
posities van de filters liggen.

![](media/19e52da1dc3d4f8595f1807ec6ccee80.emf)

Het datatype van de ondiepste en diepste verticale positie is een meetwaarde van
het type *VerticalPosition* (zie paragraaf 7.7).

### StatusOverview

Het element *StatusOverview* geeft aan welke statussen het registratieobject
heeft doorlopen.

![](media/2e52e07356eea060e862447d4e7c085c.emf)

De kardinaliteit van het element tubeStatus is gemodelleerd als vier, omdat
*Tubestatus* als beheerde enumeratie (zie paragraaf 4.2.1) vier toegestane
waarden heeft.

DispatchDataResponse
--------------------

Het *DispatchDataResponse* is een specialisatie van *DispatchResponse* in de
package *brocommon* (zie paragraaf 8.13), waaraan het een element
*dispatchDocument* toevoegt.

![](media/31850407156db45d3b2a0c15a9eb799b.emf)

Merk op dat *DispatchResponse* in *brocommon* naast de platte elementen ook een
optionele lijst met *criterionErrors* bevat. Zie voor nadere informatie hierover
en over welke elementen onder welke omstandigheden verwacht kunnen worden
paragraaf 3.5.2.

### DispatchData

Het datatype *DispatchData* bevat de gegevens van een GMW-registratieobject.

![](media/86e6ee99ae819e2c9b32ee76d6a5455f.emf)

*DispatchData* heeft het stereotype *Union* (zie ook paragraaf 4.2.6), waarmee
wordt aangegeven dat het datatype polymorf is. Onderstaande tabel geeft aan
onder welke omstandigheden welk alternatief zal worden uitgegeven:

| Object is uit registratie genomen | Opgevraagde gegevens | Data-afnemer is bronhouder of dataleverancier | Alternatief  |
|-----------------------------------|----------------------|-----------------------------------------------|--------------|
| Ja                                | Doet er niet toe     | Doet er niet toe                              | BRO\_DO      |
| Nee                               | Actueel              | Ja                                            | GMW\_PO      |
| Nee                               | Actueel              | Nee                                           | GMW\_PO\_DP  |
| Nee                               | ActueelHistorisch    | Ja                                            | GMW\_PPO     |
| Nee                               | ActueelHistorisch    | Nee                                           | GMW\_PPO\_DP |

De eerste variant is van het type *DeregisteredObject* in de package *brocommon*
(zie paragraaf 8.11), de overige varianten zijn van het type
*GroundwaterMonitoringWell*.

### ElectrodeData

Het element *electrodeData* bevat de gegevens over een elektrode, in een
geo-Ohmkabel bevestigd aan een buis, die ten gevolge van een tussentijdse
gebeurtenis gewijzigd zijn.

![](media/edbcf5bde4ebafeb7fd1a527d360870b.emf)

### EventData

Het element *eventData* bevat de putgegevens die ten gevolge van de gebeurtenis
gewijzigd zijn, dat wil zeggen wijzigingen in de put zelf (*wellData)*,
wijzigingen in monitoringbuizen (*tubeData*) en/of wijzigingen in elektrodes in
de geo-Ohmkabel bevestigd aan een monitoringbuis (*electrodeData*).

![](media/1e64b4638b1f7905bf68f6944d70439b.emf)

### EventName

Beheerde enumeratie voor het element *eventName* in een *intermediateEvent* van
de *wellHistory* (zie paragraaf 6.4.12).

![](media/c318a9bbbd7d784e72a80ea3e27ed1f3.emf)

Zie paragraaf 4.2.1 voor nadere informatie over het stereotype *CodeList*. Zie
paragraaf 9.3 voor de modellering in XSD en de toepassing in een XML bericht.

### GeoOhmCable

Het datatype *GeoOhmCable* bevat de gegevens van een geo-Ohmkabel die bevestigd
is aan een buis, bijvoorbeeld ten behoeve van het bepalen van het zoutgehalte.

![](media/09cc76a9dac8e3d2d27a2c2885410744.emf)

Een element *GeoOhmCable* bevat een verplicht element *cableNumber*, een
optioneel element *cableInUse* en een lijst met minstens 2 *electrodes*.

Het element *cableInUse* wordt niet aangeleverd door de dataleverancier, tijdens
inname vastgelegd door de BRO.

### GroundwaterMonitoringWell 

Het datatype *GroundwaterMonitoringWell* bevat de gegevens van een
GMW-registratieobject dat niet uit registratie is genomen.

![](media/c550aeeb384b987843107c2c6b852b01.emf)

Het datatype *GroundwaterMonitoringWell* heeft het stereotype *FeatureType*, wat
aangeeft dat een object van dit datatype een fenomeen in de werkelijkheid
representeert, dat direct of indirect is geassocieerd met een locatie relatief
ten opzichte van de aarde (zie paragraaf 4.2.4).

Het datatype *GroundwaterMonitoringWell* is een specialisatie van
*Registration­Object* in de package *brocommon*. De attributen die specifiek
zijn voor de uitgifte van een GMW-registratieobject zijn toegevoegd. Ook zijn
associaties naar *StandardizedLocation* en *RegistrationHistory* uit package
*brocommon* toegevoegd en GMW specifieke associaties naar *DeliveredLocation*,
*DeliveredVerticalPosition*, *WellHistory* en *MonitoringTube*.

De elementen *NITGCode* en *wellCode* zijn beiden optioneel, maar er wordt
altijd een van de twee uitgeleverd. De waarde voor *wellCode* wordt tijdens
inname door de BRO vastgelegd op basis van de aangeleverde waarde voor
*mapSheetCode* (zie Koppelvlakbeschrijving GMW innameservice).

De informatie in *RegistrationHistory*, *StandardizedLocation* en *WellHistory*
worden niet aangeleverd door de dataleverancier, maar tijdens inname vastgelegd
door de BRO.

De elementen *maintenanceResponsibleParty*, *objectIdAccountableParty* en
*delivery­Responsible­Party* worden alleen uitgegeven als de data-afnemer tevens
bronhouder en/of dataleverancier is van het opgevraagde object.

### IntermediateEvent

Het datatype *IntermediateEvent* bevat de geregistreerde gegevens over een
tussentijdse gebeurtenis die in de werkelijkheid heeft plaats gevonden, na de
constructie maar voor het opruimen van de grondwatermonitoringput.

![](media/ffbde299c68c2b829e70f99aead9e75c.emf)

Het elementen *eventName* bevat de naam van de gebeurtenis (zie de catalogus).
Het element *eventDate* bevat de datum waarop de gebeurtenis heeft plaats
gevonden (zie paragraaf 8.17 voor een toelichting over het datatype
*partialDate*). Het element *eventData* bevat de putgegevens die ten gevolge van
de gebeurtenis gewijzigd zijn.

### MonitoringTube

Het datatype *monitoringTube* bevat de gegevens over een monitoringbuis.

![](media/9d022a056afa4bbcd11d3a6179ec823d.emf)

De elementen *tubePartInserted* en *tubeInUse* worden niet aangeleverd door de
dataleverancier, maar tijdens inname vastgelegd door de BRO.

Merk op dat het element *tubeTopdiameter* het stereotype *Voidable* heeft (zie
paragraaf 4.2.7).

### Screen

Het datatype *Screen* bevat de gegevens van een filter van een monitoringbuis,
het deel dat is voorzien van openingen waardoor het grondwater kan
binnenstromen.

![](media/f423e00d1051f504fab808524f3c9997.emf)

Een element *Screen* bevat twee verplichte elementen en twee optionele
elementen.

De elementen *screenTopPosition* en *screenBottomPosition* wordt niet
aangeleverd door de dataleverancier, maar tijdens inname vastgelegd door de BRO.

### TubeData

Het element *tubeData* bevat de gegevens over een monitoringbuis die ten gevolge
van een tussentijdse gebeurtenis gewijzigd zijn.

![](media/8ee32cc1c6ab063f15faac8bd75052bb.emf)

### WellData

Het element *wellData* bevat de gegevens over de put zelf die ten gevolge van
een tussentijdse gebeurtenis gewijzigd zijn.

![](media/855a18561f06de2980752d3ba9d05e87.emf)

### WellHistory 

Het datatype *WellHistory* bevat gegevens over de materiële geschiedenis van een
GMW-registratieobject.

![](media/ec9c74b3b558ed15cb291619ccb7d16b.emf)

Het datatype *WellHistory* bevat twee platte elementen: de datum waarop de put
is geconstrueerd en de datum waarop de put is opgeruimd (indien van toepassing).
Beide datums zijn van het datatype *PartialDate* (zie paragraaf 8.17), omdat bij
gegevens aangeleverd onder het IMBRO/A-regime deze datums in het geheel onbekend
of niet volledig bekend kunnen zijn.

Als in een *DispatchDataRequest* de actuele gegevens en materiële historie van
een GMW-registratieobject worden opgevraagd, dan wordt de *WellHistory*
uitgebreid met een lijst van *IntermediaEvents*.

Package gmwcommon
=================

De package *gmwcommon* bevat de entiteiten en relaties, die gemeenschappelijk
zijn voor zowel de GMW innamewebservice als de GMW uitgiftewebservice.

Codelijsten
-----------

De package *gmwcommon* bevat een aantal codelijsten. Zie paragraaf 11.1.4 voor
een overzicht. In de XSD zijn deze gerealiseerd als een complexType wat een
restrictie is van het GML complexType *CodeWithAuthority* (zie paragraaf 9.3).
Voorbeeld:

![](media/a29000de4c4396166aaf55dfc85e2858.emf)

DeliveredLocation
-----------------

Het datatype *DeliveredLocation* bevat de gegevens, zoals die zijn aangeleverd
door de data-leverancier aan de basisregistratie ondergrond, over de plaats op
het aardoppervlak waar de grondwatermonitoringput zich bevindt.

![](media/8f328494225a5a0d5c1c22e9a6c200af.emf)

Het datatype *DeliveredLocation* bevat een element *location* van het
GML-datatype *Point*. Zie paragraaf 9.7 voor nadere details over het datatype
*GML:Point*. Voorbeeld van het element *deliveredLocation* in een XML-bestand:

| \<deliveredLocation\> \<location gml:id=*"BRO\_0001"* srsName=*"urn:ogc:def:crs:EPSG::28992"*\> \<gml:pos\>134750.000 477800.000\</gml:pos\> \<location\> \<horizontalPositioningMethod\>RTKGPS10tot50cm\</horizontalPositioningMethod\> \</deliveredLocation\> |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


DeliveredVerticalPosition
-------------------------

Het datatype *DeliveredVerticalPosition* bevat de gegevens over de verticale
positie van de grondwatermonitoringput. Het element *groundLevelPosition* heeft
het GML-stereotype *Voidable* datatype *Point*. Zie onderstaande figuur.

![](media/4595bca2ff8461cfe324bd502fbf808a.emf)

Electrode
---------

Het datatype *Electrode* bevat de gegevens over een geleider die in het
stroomcircuit ter bepaling van de elektrische geleidbaarheid gebruikt wordt om
contact te maken met het grondwater.

![](media/f87cf3c81b11b5fef05b4c9485fa60c5.emf)

InsertedPart
------------

Het datatype *InsertedPart* bevat de gegevens over de stijgbuis die in de
monitoringbuis is geplaatst en de functie van het oorspronkelijke stijgbuisdeel
overneemt.

![](media/e3f6cb72b3047e2374edeb11ebeed2a4.emf)

MaterialUsed
------------

Het datatype *MaterialUsed* bevat de gegevens over de toegepaste materialen die
gebruikt zijn voor de monitoringbuis en de vulling van de ruimte in de put rond
de buis.

![](media/52b9687c703e1db8fdb163f7a0c8e52b.emf)

Meetwaarden
-----------

De package *gmwcommon* bevat een aantal meetwaarden, dat wil zeggen datatypes
die de waarde uitdrukken in een zekere eenheid. In de catalogus zijn deze
attributen gespecificeerd met Getalswaarde.

![](media/8173f979a55dcc8895d09dd833c34762.emf)

In de koppelvlakdefinitie is ervoor gekozen om deze types naar fysische
grootheid te modelleren als extensie van het GML-datatype *Measure* en met het
stereotype *DataType*. Dit heeft als voordeel, dat er minder types nodig zijn en
dat de meeteenheid expliciet kan worden vastgelegd in het attribuut *uom* (unit
of measure). Zie bovenstaande figuur. Het formaat in de constraint *syntax*
wordt niet door de XSD afgedwongen, maar wordt door de webservice softwarematig
gecontroleerd.

Zie paragraaf 4.2.2 voor nadere details over het GML-datatype stereotype
*Datatype*. Zie paragraaf 9.6 voor nadere details over het GML-datatype
*Measure* en de realisatie in de XSD.

Voorbeeld van een element met een zo’n datatype in een GML bericht:

| \<offset uom=*"m"*\>3.300\</offset\> |
|--------------------------------------|


PlainTubePart
-------------

Het datatype *PlainTubePart* bevat de gegevens over het stijgbuisdeel, het deel
van de monitoringbuis boven het filter dat dient om het grondwater op te vangen
dat via het filter binnenstroomt.

![](media/71b1f291a94bb9c9821af6747670d9c0.emf)

SedimentSump
------------

Het datatype *SedimentSump* bevat de gegevens over de zandvang, het deel van de
monitoringbuis dat dient om het sediment op te vangen dat via het filter de buis
in komt.

![](media/7f91a81be160a16e558ec72db650c969.emf)

Package brocommon
=================

De package brocommon bevat de entiteiten en relaties, die gemeenschappelijk zijn
voor alle registratieobjecten.

AbortReason
-----------

Zie *ParseFault* in paragraaf 8.16.

Area
----

Het datatype *Area* geeft de begrenzing aan van een geografisch gebied aan het
aardoppervlak.

![](media/e4fb7f9c806e3bf5dbe2d8c0cf9a7c68.emf)

Het datatype heeft een stereotype *Union* (zie paragraaf 4.2.6) wat aangeeft dat
óf een *enclosingCircle* (zie paragraaf 8.5) óf een *boundingBox* (zie paragraaf
9.5) moet worden opgenomen.

Characteristics
---------------

Het datatype *Characteristics* bevat de registratieobject onafhankelijke
kengegevens van een registratieobject dat niet uit registratie is genomen.

![](media/c2aa9893d1ab1710bff57ffea602c40d.emf)

Het datatype *DispatchCharacteristics* bevat naast enkele platte elementen ook
twee gestructureerde elementen *deliveredLocation* en *standardizedLocation*,
beiden van het datatype *GML:Point* (zie paragraaf 9.7). Het element
*standardizedLocation* wordt niet aangeleverd door de dataleverancier, maar
tijdens inname vastgelegd door de BRO.

ChamberOfCommerceNumber
-----------------------

Het datatype *ChamberOfCommerceNumber* bevat het Kamer van Koophandel nummer.

![](media/a1be5d3148c4f0dc49ee4afafb56e28a.emf)

In de XSD is dit een extensie van het type string. Merk op dat het formaat in de
constraint *Value* niet door de XSD wordt afgedwongen, maar dat dit
softwarematig door het BRO-systeem wordt gecontroleerd.

Circle
------

Het datatype *Circle* geeft een cirkelvormige begrenzing aan van een gebied aan
het aardoppervlak.

![](media/a4505685a5515f62252c0758ad0e7244.emf)

De cirkel wordt gedefinieerd door het middelpunt (element *center* met datatype
*doublelist*; zie paragraaf 9.4) en de straal (element *radius* met datatype
Radius, een lengtemaat in kilometers; zie paragraaf 9.6). Het attribuut
*srsName* geeft aan in welk coördinatensysteem het middelpunt is uitgedrukt (zie
paragaaf 9.7).

CoordinateTransformation
------------------------

Het datatype *CoordinateTransformation* is een beheerde enumeratie en het heeft
daardoor een stereotype *CodeList* (zie paragraaf 4.2.1). De waarde geeft aan
welke transformatiemethode is toegepast. Merk op dat de toegestane waarde anders
kan zijn voor IMBRO dan voor IMBRO/A.

![](media/d714d9e061e53e4c7e95864ebac33cfd.emf)

CorrectionRequest
-----------------

Het datatype *CorrectionRequest* bevat de gemeenschappelijke gegevens voor het
samenstellen van een request om de gegevens voor een bepaald registratieobject
te corrigeren.

![](media/e7dc4dda0747c0ad7d2ac437541ed948.emf)

Het element *requestReference* is een voor de data-afnemer unieke aanduiding van
het request.

Het element *deliveryAccountableParty* bevat het kamer van koophandel nummer van
de bronhouder. Dit element is verplicht als de dataleverancier niet de
bronhouder is. Dit element is verboden als de dataleverancier tevens bronhouder
is.

Het element *broId* is de unieke aanduiding van het registratieobject waarvoor
gegevens worden gecorrigeerd.

Zie de *catalogus* voor aanvullende informatie over de andere elementen.

CriteriaSet
-----------

Het datatype *CriteriaSet* is een abstract datatype ten behoeve van het
samenstellen van *DispatchCharacteristicsRequest*.

![](media/c45ef1c88cb935661c2897f5e0fdc0e9.emf)

Het abstracte datatype *CriteriaSet* definieert een aantal optionele elementen
voor de kenmerkenverzameling en één verplicht element *area* (zie paragraaf
8.2). Alleen kengegevens van registratieobjecten, waarvan de gestandaardiseerde
locatie (zie paragraaf 8.26) valt binnen het opgegeven gebied worden
uitgeleverd.

CriterionError
--------------

Het datatype *CriterionError* bevat als onderdeel van een *DispatchResponse*
(zie paragraaf 8.13) één foutmelding met betrekking tot een geconstateerde fout
in de kenmerkenverzameling van een uitgifteverzoek, bestaande uit een volgnummer
en een omschrijving.

![](media/ebb6f0c34716d1e6f6570fb003fc725f.emf)

DatePeriod
----------

Het datatype *DatePeriod* bevat een begin en eindwaarde, beiden van het
standaard datatype *Date*, zodat in de *CriteriaSet* een periode kan worden
opgenomen waarbinnen een datum moet liggen.

![](media/70d287f9ed71d08af5c9aa203439163d.emf)

Merk op dat beide elementen verplicht zijn en niet een lege waarde mogen hebben.

DeregisteredObject
------------------

Het datatype *DeregisteredObject* bevat de gegevens over een registratieobject
dat uit registratie is genomen.

![](media/272505337c189af8301601a48ae8cb64.emf)

DispatchDataRequest
-------------------

Het datatype *DispatchDataRequest* bevat de gemeenschappelijke gegevens voor het
samenstellen van een *request* om de gegevens over een bepaald registratieobject
op te vragen.

![](media/f0c8dd1d8357e306bab13230721b36b3.emf)

Het element *requestReference* is een voor de afnemer unieke aanduiding van het
*request*.

Het element *broId* is de unieke aanduiding van het registratieobject waarvan de
gegevens worden opgevraagd.

DispatchResponse
----------------

Het datatype *DispatchResponse* is een abstract datatype voor het samenstellen
van een *response* als reactie op een uitgifteverzoek (dispatch *request*).

![](media/49d106647d7c23ba96ad4d697befff1f.emf)

Het datatype *DispatchResponse* is een generiek *response*. Het definieert een
aantal platte elementen, sommigen verplicht en anderen optioneel, inclusief een
optionele lijst met foutmeldingen (zie paragraaf 8.9). Zie hoofdstuk 3 voor een
beschrijving van welke velden onder welke omstandigheden gevuld zullen worden.

Enumeraties
-----------

De catalogus maakt een onderscheid in beheerde en niet-beheerde enumeraties. Het
stereotype *Enumeration* wordt in UML gebruikt om aan te geven dat een datatype
een niet-beheerde enumeratie is (zie paragraaf 4.2.3).

De package brocommon definieert zes datatypes met als domein een enumeratie van
toegestane waarden.

![](media/9e80506a24df304d9231cdcfd44ce8b6.emf)

In de XSD zijn deze gerealiseerd als een simpleType als restrictie van het
standaard XSD type string. Voorbeeld:

| \<simpleType name=*"IndicationYesNoEnumeration"*\> \<restriction base=*"string"*\> \<enumeration value=*"ja"* /\> \<enumeration value=*"nee"* /\> \</restriction\> \</simpleType\> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


Voorbeeld van een element in een XML bericht:

| \<deregistered\>nee\</deregistered\> |
|--------------------------------------|


IntakeResponse
--------------

Als het BRO-systeem na de toegangscontrole het *request* kan verwerken zonder
dat er fouten worden geconstateerd in het *request* en/of het *sourceDocument*
en zonder dat er een onverwachte fout optreedt in het BRO-systeem, dan reageert
het BRO-systeem met een functionele *response*. Deze functionele *response* is
van het datatype *IntakeResponse*.

![](media/3a6ba945fbda56fe075397e74d7ed942.emf)

Het element *responseType* geeft aan of het *request* succesvol kon worden
verwerkt (waarde *completion* bij een *RegistrationRequest*; waarde *acceptance*
bij een *CorrectionRequest*) of dat de verwerking om functionele redenen niet
succesvol is (waarde *rejection*).

De waarde voor het element *requestReference* wordt overgenomen uit het
*request*, zodat de zendende partij weet voor welk *request* dit een *response*
is.

De waarde voor het element *transactionId* wordt toegekend door het
transactieregister. De zendende partij kan dit gegeven gebruiken in de
(mondelinge) communicatie met de BRO Servicedesk, zodat deze de transactie kan
terugvinden in het transactieregister.

Het element *broId* bevat de identificatie van het object in de BRO. Dit element
is afwezig als de *response* een reactie is op een *RegistrationRequest* en als
het element *responseType* een waarde *rejection* heeft.

Het element *ObjectIdAccountableParty* is alleen aanwezig als de *response* een
reactie is op een *RegistrationRequest* en als het element *responseType* een
waarde *rejection* heeft. De waarde wordt overgenomen uit het
*RegistrationRequest*, zodat de zendende partij weet wat zijn identificatie is
van het geweigerde registratieobject.

Van de elementen *acceptanceTime*, *completionTime* en *rejectionTime* zal
steeds één daarvan aanwezig zijn, afhankelijk van de waarde voor het element
*responseType*. In deze elementen staat het (datum en) tijdstip waarop het
*request* is geaccepteerd, het *request* is verwerkt of het *request* is
afgewezen.

Als het *request* is afgewezen, dan staat in element *rejectionReason* de reden.
Als de reden is dat er een of meer gebruiksfouten in het *sourceDocument* zijn
geconstateerd, dan is de waarde van *rejectionReason* “er zijn 1 of meer fouten
geconstateerd in het brondocument” en bevat *IntakeResponse* een lijst
*sourceDocumentErrors*, waarbij iedere *sourceDocumentError* bestaat uit een
*sequenceNumber* (voor het sorteren van de gebruiksfout) en een *specification*
(een tekstuele beschrijving van de gebruiksfout).

ParseFault
----------

Als het BRO-systeem, na de toegangscontrole, fouten constateert in het *request*
en/of het *sourceDocument* (bijvoorbeeld het *request* is niet een welgevormd
XML-bericht of het *request* voldoet niet aan de schemavalidatie), dan worden
deze geduid als een softwarefout in het systeem van de dataleverancier. Het
BRO-systeem reageert dan niet met een *IntakeResponse*, maar met een
*SOAP:Fault*, waarbij het element *detail* van het datatype *ParseFaultDetail*
is. Het datatype *ParseFaultDetail* bevat één element *parseFault* van het
datatype *ParseFault*.

![](media/d8ce6c396a57c0f7c8239cb249f44637.emf)

De elementen van *SOAP:Fault* hebben de volgende betekenis:

| SOAP:Fault    | Inhoud                                                 |
|---------------|--------------------------------------------------------|
| *Faultcode*   | Vaste waarde “soap:Client”                             |
| *Faultstring* | Vaste waarde “Het verzoek voldoet niet aan het schema” |
| *Detail*      | *ParseFaultDetail*                                     |

Het datatype *ParseFault* bevat drie platte elementen en een lijst met
*abortReasons*. De lijst *abortReasons* bestaat uit minimaal 1 en maximaal 99
voorkomens van het complex type *AbortReason*.

![](media/3286ffeb71cbbca9fbece03cc382f5aa.emf)

De elementen van *ParseFault* en *AbortReason* hebben de volgende betekenis:

| ParseFault         | Inhoud                                                                                                                                                   |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|
| *RequestReference* | Waarde overgenomen uit *request* (dit element is optioneel omdat de softwarefout geconstateerd kan worden voordat het *request* is gelezen).             |
| *TransactionId*    | Waarde toegekend door transactieregister (dit element is optioneel omdat de softwarefout geconstateerd kan worden voordat een transactie is aangemaakt). |
| *AbortTime*        | Tijdstip, toegekend door webservice, waarop de fout is opgetreden.                                                                                       |
| *AbortReason*      | Numerieke waarde bedoelt om de lijst met schema validatie fouten te kunnen sorteren Omschrijving van de validatie fout                                   |

-   *SequenceNumber*  
    

-   *Specification*

PartialDate
-----------

Het datatype *PartialDate* ondersteunt een datum met een aantal mogelijke
nauwkeurigheden.

![](media/3a368dffbb0009f57d7e405ddab83366.emf)

*PartialDate* heeft het stereotype *Union* (zie paragraaf 4.2.6), waarmee wordt
aangegeven dat het element met dit datatype polymorf is en dat bij een voorkomen
precies een van de alternatieven gekozen moet worden. De beschikbare
alternatieven zijn:

-   date: Volledig datum tot op de dag nauwkeurig (formaat "YYYY-MM-DD")

-   yearMonth: Onvolledige datum tot op de maand nauwkeurig (formaat "YYYY-MM")

-   year: Onvolledige datum tot op het jaar nauwkeurig (formaat "YYYY")

-   voidReason: Geen datum bekend (vaste waarde *onbekend*)

Gegevens met dit datatype, die worden aangeleverd onder het kwaliteitsregime
IMBRO, mogen alleen het alternatief *date* gebruiken. Onder het kwaliteitsregime
IMBRO/A mogen alle vier alternatieven gebruikt worden.

De datatypes *Date*, *gYearMonth* en *gYear* zijn standaard XSD-datatypes, met
een bereik conform ISO 8601. Deze datatypes mogen optioneel worden aangevuld met
een tijdzone (Z voor UTC; +01:00 voor wintertijd in Nederland; +02:00 voor
zomertijd in Nederland).

Voorbeelden van een aantal keren hetzelfde element in een XML bericht met als
waarde steeds een andere variant van het type partialDate:

| \<researchReportDate\> \<brocom:date\>2015-10-28\</brocom:date\> \</researchReportDate\> \<researchReportDate\> \<brocom:date\>2015-10-28+02:00\</brocom:date\> \</researchReportDate\> \<researchReportDate\> \<brocom:date\>2015-10-28Z\</brocom:date\> \</researchReportDate\> \<researchReportDate\> \<brocom:yearMonth\>2015-10\</brocom:yearMonth\> \</researchReportDate\> \<researchReportDate\> \<brocom:year\>2015\</brocom:year\> \</researchReportDate\> \<researchReportDate\> \<brocom:voidReason\>onbekend\</brocom:voidReason\> \</researchReportDate\> |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


Radius
------

Het datatype *Radius* is voor het uitdrukken van een straal in kilometers. Zie
paragraaf 9.6 voor nadere details over het GML-datatype *Measure* en de
realisatie in de XSD.

![](media/4f5c981b9ecbc8a49937c510fc433ee8.emf)

Voorbeeld van zo’n element in een GML bericht, waarbij de straal 8,5 kilometer
is:

| \<radius uom=*"km"*\>8.5\</radius\> |
|-------------------------------------|


RegistrationHistory
-------------------

Het datatype *RegistrationHistory* bevat gegevens die de geschiedenis van het
object in de registratie markeren.

![](media/fe1a666dbd3817bc9ffda4aa0a3e0cab.emf)

Registration­Object
-------------------

Het abstract datatype *RegistrationObject* bevat de algemene gegevens van een
registratieobject dat niet uit registratie is genomen.

![](media/914c7653f4becd3d9f6718ae346ddbb2.emf)

Het datatype *RegistrationObject* heeft het stereotype *FeatureType* (zie
paragraaf 4.2.4), wat aangeeft dat een object van dit datatype een fenomeen in
de werkelijkheid representeert, dat direct of indirect is geassocieerd met een
locatie relatief ten opzichte van de aarde en dat een element van dit datatype
een verplicht attribuut *gml:id* heeft.

Het datatype *RegistrationObject* definieert een aantal platte elementen en twee
gestructureerde elementen: *RegistrationHistory* en *StandardizedLocation*.

De informatie in *RegistrationHistory* en *StandardizedLocation* worden niet
aangeleverd door de dataleverancier, maar tijdens inname vastgelegd door de BRO.

De elementen *objectIdAccountableParty* en *delivery­Responsible­Party* worden
alleen uitgegeven als de data-afnemer tevens bronhouder en/of data-afnemer is
van het registratieobject. Voor andere data-afnemers worden deze attributen weg
gelaten.

RegistrationObjectCode
----------------------

Het datatype *RegistrationObjectCode* is een restrictie van het standaard
datatype string. De eerste drie posities zijn de afkorting van type
registratieobject, gevolgd door een twaalf cijferig, registratieobject
afhankelijk volgnummer.

![](media/b8850c2a6785c6cef0dbe61491da689f.emf)

RegistrationRequest
-------------------

Het datatype *RegistrationRequest* bevat de gemeenschappelijke gegevens voor het
samenstellen van een *request* om de gegevens voor een bepaald registratieobject
te registreren.

![](media/41379507b80ad7fcafea174bc7db45bd.emf)

Het element *requestReference* is een voor de data-afnemer unieke aanduiding van
het *request*.

Het element *deliveryAccountableParty* bevat het kamer van koophandel nummer van
de bronhouder. Dit element is verplicht als de dataleverancier niet de
bronhouder is. Dit element is verboden als de dataleverancier tevens bronhouder
is.

Het element *broId* is de unieke aanduiding van het registratieobject waarvoor
gegevens worden geregistreerd. Dit element is verboden bij de initiële
registratie van de gegevens van een registratieobject.

Zie de *catalogus* voor aanvullende informatie over de andere elementen.

RegistrationStatus
------------------

Het datatype *RegistrationStatus* is een beheerde enumeratie en het heeft
daardoor een stereotype *CodeList* (zie paragraaf 4.2.1). Zie de *catalogus*
voor het domein en de betekenis van de waarden.

![](media/220356fa467cfdf336e5e776d2d78b3c.emf)

SOAP Fault
----------

Als tijdens de uitvoering van een operatie er een onverwachte fout optreedt in
het BRO-systeem, dan reageert het BRO-systeem niet met een *IntakeResponse*,
maar met een *SOAP:Fault*.

![](media/002011a5988f496a9fb606f77ebc0210.emf)

Alhoewel dit een standaard niet-gemodelleerde fout is uit de SOAP namespace,
wordt dit hier toch beschreven als tegenhanger van de ParseFault, wat gebruikt
wordt in geval van een softwarefout.

De elementen van *SOAP:Fault* hebben de volgende betekenis:

| SOAP:Fault    | Inhoud                                                         |
|---------------|----------------------------------------------------------------|
| *Faultcode*   | Vaste waarde “soap:Server”                                     |
| *Faultstring* | Vaste waarde “Er is een fout in het BRO-systeem geconstateerd” |
| *Detail*      | Optioneel complex element (zie volgende tabel)                 |

Binnen het element *detail* zal het BRO-systeem de volgende elementen opnemen:

| Element            | Inhoud                                                                                                                                                   |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|
| *RequestReference* | Waarde overgenomen uit *request* (dit element is optioneel omdat de softwarefout geconstateerd kan worden voordat het *request* is gelezen).             |
| *TransactionId*    | Waarde toegekend door transactieregister (dit element is optioneel omdat de softwarefout geconstateerd kan worden voordat een transactie is aangemaakt). |
| *AbortTime*        | Tijdstip, toegekend door webservice, waarop de fout is opgetreden.                                                                                       |

Er wordt summiere informatie teruggegeven dat de fout is opgetreden en dat het
verzoek niet is verwerkt. Deze fouten kunnen niet door de data-afnemer worden
opgelost. Neem contact op met de BRO Servicedesk voor de verdere afhandeling van
dit type fouten.

De *requestReference* is opgenomen in de foutmelding, zodat de zendende partij
weet bij welk verzonden bericht de systeemfout is opgetreden, ook als deze
foutmelding buiten de context van de synchrone *request* – *response* interactie
geanalyseerd wordt. Dit kan behulpzaam zijn bij de analyse en reproductie het
probleem.

De *transactionId* is opgenomen in de foutmelding, zodat de zendende partij dit
kan doorgeven aan de BRO-helpdesk. De BRO-helpdesk kan daarmee de mislukte
transactie terugvinden in het transactieregister, waarin aanvullende informatie
(zoals een deel van de stacktrace) is opgeslagen.

De *abortTime* is opgenomen in de foutmelding, zodat de zendende partij, in het
bijzonder in het geval de beide voorgaande gegevens niet bekend zijn, in ieder
geval dit gegeven kan doorgeven aan de BRO-helpdesk, waarmee een technisch
BRO-medewerker gericht kan zoeken in de logfiles.

SourceDocumentError
-------------------

Zie *IntakeResponse* in paragraaf 8.15.

StandardizedLocation
--------------------

Het datatype *StandardizedLocation* bevat een element *location* van het
GML-datatype *Point* (zie paragraaf 9.7) en een element
*CoordinateTransformation* met toegestane waarden uit een codelijst (zie
paragraaf 8.6).

![](media/eae0d3bb87eb9695f8c2e55b91f95069.emf)

De *StandardizedLocation* maakt het mogelijk alle gegevens in de registratie
ondergrond in een en hetzelfde referentiestelsel te ontsluiten.

Het coördinatensysteem van het element *location* binnen *StandardizedLocation*
is altijd ETRS89, oftewel de waarde van attribuut *srsName* van element
*location* is urn:ogc:def:crs:EPSG::4258.

Het BRO-systeem berekent tijdens inname de gestandaardiseerde locatie op basis
van de aangeleverde locatie. Het element *CoordinateTransformation* geeft aan
welke transformatiemethode daarbij is toegepast.

Voorbeeld van het element *location* binnen *StandardizedLocation* in een
XML-bestand:

| \<location gml:id=*"BRO\_0001"* srsName=*"urn:ogc:def:crs:EPSG::4258"*\> \<gml:pos\>52.28782 5.09042\</gml:pos\> \</location\> |
|--------------------------------------------------------------------------------------------------------------------------------|


Package gml-profile
===================

De package gml-profile bevat het GML-profiel, oftewel die concepten uit de
GML-standaard van de OGC die gebruikt worden in de BRO.

AbstractFeature
---------------

Een aantal gegevens in de BRO is conform NEN3610 geclassificeerd met een
FeatureType stereotype. Dit heeft tot gevolg dat hun XML-schema-type is afgeleid
van *AbstractFeature*.

![](media/ecd24f8f86f27d228975e12a112bddff.emf)

Hierdoor overerft een element van dit datatype het attribuut *gml:id* met als
datatype het XML-standaard type *ID*. Zie paragraaf 9.2.

AbstractGML
-----------

Het datatype *AbstractGML* definieert een verplicht attribuut *id*.

![](media/7545b1d5511636fd636d639813143151.emf)

Dit XML-attribuut voorziet in het gebruik als referentie binnen één XML-bericht.
Het datatype van het attribuut *id* is het XML-standaard type ID, zodat het
uniek is binnen het XML-document waarin het voorkomt. In de BRO wordt deze
identificatie niet gebruikt en daarom ook niet opgeslagen. Bij uitgifte wordt de
identificatie gegenereerd. Een element kan op ander moment een andere waarde
krijgen.

| \<registrationObject gml:id=*"ro-4774"*\> |
|-------------------------------------------|


CodeWithAuthority
-----------------

Het complexType *CodeWithAuthority* wordt gebruikt voor beheerde enumeraties
c.q. codelijsten (zie paragraaf 4.2.1).

Het complexType *CodeWithAuthority* is een restrictie van het type string,
waaraan het een attribuut *codespace* van het type *anyURI* toevoegt. Deze
*codespace* bevat de naam van de codelijst. Elke codelijst in de BRO heeft
daarom een eigen *codespace* die in de XSD als vaste waarde is opgenomen. Zie
onderstaande figuur.

![](media/982d996445f8ff63a80d300f27973973.emf)

In een XSD leidt dit tot een restrictie van het complexType *CodeWithAuthority*.
Voorbeeld van een codelijst in XSD:

| \<complexType name=*"DeliveryContext"*\> \<simpleContent\> \<restriction base=*"gml:CodeWithAuthorityType"*\> \<attribute name=*"codeSpace"* type=*"anyURI"* use=*"required"* fixed=*"urn:bro:BHR:DeliveryContext"*/\> \</restriction\> \</simpleContent\> \</complexType\> |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


Voorbeeld van een element, met als datatype een codelijst, in een XML bericht.
Zo’n element heeft een attribuut *codeSpace*, waarvan de waarde aangeeft in
welke tabel de toegestane waarden zijn vastgelegd, en als waarde een van de
waarden uit die tabel. Voorbeeld:

| \<deliveryContext codeSpace=*"urn:bro:BHR:DeliveryContext"*\>publiekeTaak\</deliveryContext\> |
|-----------------------------------------------------------------------------------------------|


Merk op dat in de catalogus en in het UML-diagram het domein expliciet wordt
benoemd. Het domein is niet opgenomen in het XSD-bestand, omdat een
*CodeWithAuthority* wordt gebruikt voor een beheerde enumeratie zodat een
wijziging in het domein zal leiden tot een wijziging in het XSD-bestand als dat
wel het geval zou zijn. Daarom wordt het domein niet afgedwongen door het
XSD-bestand en valideert het BRO-systeem de gebruikte waarde softwarematig via
een database tabel.

Merk op dat bij een codelijst de toegestane waarden anders kunnen zijn voor
IMBRO dan voor IMBRO/A. Zie de catalogus voor nadere details.

Doublelist
----------

Het datatype *doublelist* bevat een reeks floating point getallen als waarde
voor een element of een attribuut.

![](media/436372f31d7c05338aeb46bc489513e5.emf)

De getallen worden gescheiden door een spatie. De decimalen worden gescheiden
van de eenheden door een punt.

Envelope
--------

Het datatype *Envelope* geeft een rechthoekige begrenzing aan van een gebied aan
het aardoppervlak.

![](media/838f392f380f9d93cdc65c5a60637e79.emf)

Het datatype *Envelope* is een extensie van *AbstractGeometricPrimitive*,
waaraan het twee elementen toevoegt.

De rechthoek wordt gedefinieerd door het onderhoek (element *lowerCorner* met
als coördinatenpaar de minimale waarden voor de twee dimensies binnen de
rechthoek) en de bovenhoek (element *upperCorner* met als coördinatenpaar de
minimale waarden voor de twee dimensies binnen de rechthoek). Beide locaties
zijn van het datatype *doublelist* (zie paragraaf 9.4).

Zie paragaaf 9.7 voor een toelichting op de attributen die geërfd worden van
*AbstractGeometricPrimitive*.

Voorbeeld een element van het datatype *Envelope*, zijnde een vierkant van 10 \*
10 km in RD-coördinaten:

| \<boundingBox gml:id=*"BRO\_0001"* srsName=*"urn:ogc:def:crs:EPSG::28992"*\> \<gml:lowerCorner\>136000.0 472000.0\</gml:lowerCorner\> \<gml:upperCorner\>146000.0 482000.0\</gml:upperCorner\> \</boundingBox\> |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


Measure
-------

Het datatype *Measure* is een extensie van het standaard XSD type double,
waaraan het een verplicht attribuut *uom* (unit of measure) toevoegt:

![](media/1b52d3ba452dfd56387fb3104e15a08d.emf)

In de koppelvlakdefinitie is ervoor gekozen om deze types naar fysische
grootheid te modelleren. Dit heeft als voordeel, dat er minder types nodig zijn
en dat de meeteenheid expliciet kan worden vastgelegd in het attribuut *uom*.

NB: het attribuut uom is verplicht, ook als de elementwaarde leeg is.

Point
-----

Point is een datatype voor elementen met een puntlocatie aan het aardoppervlak.
Het definieert een element *pos* en drie attributen *id*, *srsName* en
*srsDimension*.

![](media/1bede76f0a167a23ef25b9f8c3a12041.emf)

Het attribuut *id* voorziet in een referentie voor het XML-element dat een
GML-object vertegenwoordigt. Het gebruik ervan is verplicht voor alle
GML-objecten. Het datatype is het standaard XML-type ID, zodat het uniek is
binnen het XML-document waarin het voorkomt.

Het attribuut *srsName* bevat de URI van het coördinatensysteem waarin de
locatie van het punt wordt uitgedrukt. Onderstaande tabel geeft de toegestane
waarden binnen GMW.

| Naam   | Betekenis                                  | Waarde voor srsName        |
|--------|--------------------------------------------|----------------------------|
| ETRS89 | European Terrestrial Reference System 1989 | urn:ogc:def:crs:EPSG:4258  |
| RD     | Rijks Driehoeksmeting – Amersfoort RD New  | urn:ogc:def:crs:EPSG:28992 |

Het attribuut *srsDimension* bevat het aantal dimensies van de coördinaten.
Omdat het attribuut *srsDimension* optioneel is en omdat de referentiestelsels
ETRS89 en RD beiden tweedimensionaal zijn, is alleen *srsDimension=”2”*
toegestaan. Daarom en om inconsistenties te voorkomen wordt aangeraden het
attribuut weg te laten (zie referentie [4]).

Conform NEN3610 wordt voor het coördinatenpaar van de locatie het attribuut
*pos* gebruikt van datatype *doublelist* (zie paragraaf 9.4). Het bereik en de
betekenis is afhankelijk van het gebruikte coördinatensysteem. Onderstaande
tabel geeft per coördinatensysteem de betekenis en de eenheid van het
coördinatenpaar.

| Naam   | Betekenis coördinaten | Eenheid         |
|--------|-----------------------|-----------------|
| ETRS89 | Latitude, Longitude   | Decimale graden |
| RD     | X, Y                  | Meter           |

In een XSD ziet de definitie van een element met dit datatype er bijvoorbeeld
als volgt uit:

| \<element name=*"location"* type=*"gml:PointType"*/\> |
|-------------------------------------------------------|


In een XML-bericht krijgt een element van het type GML-datatype *Point* drie
attributen en als inhoud een *pos* element. Voorbeeld:

| \<location gml:id=*"BRO\_0001"* srsName=*"urn:ogc:def:crs:EPSG::4258"*\> \<gml:pos\>52.08860451 5.16575333\</gml:pos\> \</location\> \<location gml:id=*"BRO\_0001"* srsName=*"urn:ogc:def:crs:EPSG::28992"*\> \<gml:pos\>139794.52 455443.35\</gml:pos\> \</location\> \<location gml:id=*"BRO\_0001"* srsName=*"urn:ogc:def:crs:EPSG::4326"*\> \<gml:pos\>52.08860451 5.16575333\</gml:pos\> \</location\> |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


TM\_TimeInstant
---------------

Het datatype *TM\_TimeInstant* bevat een identificeerbare datum of tijdstip.

![](media/03a4c9c0c3c4c8bd03cde069361b5626.emf)

Het element *position*, met als datatype *TM\_Position* (zie paragraaf 9.9),
bevat de datum of datum en tijd, inclusief tijdzone, in ISO 8601 formaat.

Het overerfde attribuut *id* is verplicht (zie de beschrijving in paragraaf 9.2)
en kan gebruikt worden om te verwijzen naar een specifiek tijdstip. Elementen
van het type *TM\_TimeInstant* die dezelfde datum of hetzelfde tijdstip
vertegenwoordigen (al kan de waarde gezien de tijdzone kan verschillen) hebben
dezelfde waarde voor het attribuut *id*.

Voorbeeld van een datum en tijd volgens Nederlandse zomertijd:

| \<phenomenonTime gml:id=*"to-3772"*\> \<gml:timePosition\>2013-07-12T10:04:38+02:00\</gml:timePosition\> \</phenomenonTime\> |
|------------------------------------------------------------------------------------------------------------------------------|


TM\_Position 
-------------

![](media/24a7f02b7fefcafd8c9cd4fe14e22e47.emf)

Dit type is een Union waarin verschillende mogelijkheden voor het beschrijven
van een positie in de tijd uit de ISO 19108 standaard zijn gecombineerd.

Een element van type *TM\_Position* heeft onder het kwaliteitsregime IMBRO als
domein:

-   Datum en tijd

-   Of een datum

Onder het kwaliteitsregime IMBRO/A is het domein:

-   Datum en tijd

-   Of een datum

-   Of jaartal en maand

-   Of jaartal

-   Of onbekend

Binnen de BRO geldt als conventie dat een element met een naam met een suffix
*Time* als domein datum en tijd of minder nauwkeurig heeft en een element met
een naam met een suffix *Date* als domein datum of minder nauwkeurig heeft.

Binnen de BRO geldt voor een datum de codering ISO-8601 en de kalender
Gregoriaans. Formaat: YYYY-MM-DD.

Binnen de BRO bestaat een tijd uit uren, minuten en secondes conform UTC;
milliseconden worden niet gebruikt. Formaat: YYYY-MM-DDThh:mm:ss.

Voorbeelden:

| \<resultTime\>2013-07-12T10:04:38+02:00\</resultTime\> \<resultTime\>2013-07-12T10:04:38Z\</resultTime\> \<resultTime\>2013-07-12T10:04:38\</resultTime\> \<resultTime\>2013-07-12\</resultTime\> \<resultTime\>2013-07\</resultTime\> \<resultTime\>2013\</resultTime\> \<resultTime indeterminatePosition=*"unknown"*/\> \<reportDate\>2015-01-01+01:00\</reportDate\> \<reportDate\>2015-01-01Z\</reportDate\> \<reportDate\>2015-01-01\</reportDate\> \<reportDate\>2015-01\</reportDate\> \<reportDate\>2015\</reportDate\> \<reportDate indeterminatePosition=*"unknown"*/\> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


Package xlink-profile
=====================

De package xlink-profile bevat het XLINK-profiel, oftewel die concepten uit de
XLINK-standaard van de OGC die gebruikt worden in de BRO.

Href
----

Het datatype *href* definieert een XML-attribuut (niet een XML-element) van het
datatype *hrefType*.

![](media/37fcc5a90efcff8888831c4974c7c096.emf)

HrefType
--------

Het datatype *hrefType* definieert een *simpleType* als afgeleide van anyURI.

![](media/a5b8c411f5bbaad14e079a9ad6702981.emf)

SimpleAttrs
-----------

Het datatype *simpleAttrs* definieert een XML attributeGroup met twee
XML-attributen (geen XML-elementen).

![](media/46a42adc10d87b32f4dd08309bb947f7.emf)

Type
----

Het datatype *type* definieert een XML-attribuut (niet een XML-element) van het
datatype *TypeType*.

![](media/2455bf0e9505dfc80be9e420611663ff.emf)

TypeType
--------

Het datatype *TypeType* definieert een enumeratie met één toegestane waarde.

![](media/35d19094f347cc0f67a7e198671c1527.emf)

Bijlagen
========

Bijlage A: Vertaalslag Engels – Nederlands
------------------------------------------

### A1: dsgmw-messages

| Engels                          | Nederlands                             |
|---------------------------------|----------------------------------------|
| Characteristics                 | Kengegevens                            |
| constructionStandard            | Kwaliteitsnorm inrichting              |
| groundLevelPosition             | Maaiveld positie                       |
| initialFunction                 | Initiële functie                       |
| localVerticalReferencePoint     | Lokaal verticaal referentiepunt        |
| NITGCode                        | NITG-code                              |
| numberOfMonitoringTubes         | Aantal monitoringbuizen                |
| offSet                          | Verschuiving                           |
| owner                           | Eigenaar                               |
| removed                         | Opgeruimd                              |
| verticalDatum                   | Verticaal referentievlak               |
| wellCode                        | Putcode                                |
| wellConstructionDate            | Inrichtingsdatum put                   |
| wellHeadProtector               | Beschermconstructie                    |
| wellRemovalDate                 | Opruimingsdatum put                    |
| withPrehistory                  | Met voorgeschiedenis                   |
| CriteriaSet                     | Kenmerkenverzameling                   |
| constructionPeriod              | Periode van inrichting                 |
| constructionStandard            | Kwaliteitsnorm inrichting              |
| geoOhmCablePresent              | Geo-ohmkabel aanwezig                  |
| initialFunction                 | Initiële functie                       |
| maximumTubeTopDiameter          | Maximale diameter bovenkant buis       |
| minimumNumberOfTubes            | Minimum aantal buizen                  |
| minimumTubeTopDiameter          | Minimale diameter bovenkant buis       |
| owner                           | Eigenaar                               |
| removalPeriod                   | Periode van opruiming                  |
| removed                         | Opgeruimd                              |
| screenPositionRange             | Verticaal interval                     |
| tubeStatus                      | Buisstatus                             |
| wellHeadProtector               | Beschermconstructie                    |
| withPrehistory                  | Met voorgeschiedenis                   |
| DiameterRange                   | Diameterbereik                         |
| largestTubeTopDiameter          | Grootste diameter bovenkant buis       |
| smallestTubeTopDiameter         | Kleinste diameter bovenkant buis       |
| DispatchCharacteristics         | Uitgiftedocument (kengegevens)         |
| Characteristics                 | Kengegevens                            |
| DeregisteredObject              | Object uit registratie genomen         |
| DispatchCharacteristicsRequest  | Verzoek tot verzending kengegevens     |
| criteria                        | Kenmerken                              |
| requestReference                | Verzoekkenmerk                         |
| DispatchCharacteristicsResponse | Bericht van verzending kengegevens     |
| dispatchDocument                | Uitgiftedocument                       |
| dispatchTime                    | Tijdstip van uitgifte                  |
| numberOfDocuments               | Aantal documenten                      |
| rejectionReason                 | Reden afwijzing                        |
| rejectionTime                   | Tijdstip van afwijzing                 |
| requestReference                | Verzoekkenmerk                         |
| responseType                    |                                        |
| DispatchData                    | Uitgiftedocument (gegevens)            |
| DeregisteredObject              | Object uit registratie genomen         |
| GroundwaterMonitoringWell       | Grondwatermonitoringput                |
| DispatchDataRequest             | Verzoek tot verzending gegevens        |
| broId                           | BRO-ID                                 |
| dataToBeDelivered               | Te leveren gegevens                    |
| requestReference                | Verzoekkenmerk                         |
| DispatchDataResponse            | Bericht van verzending gegevens        |
| DispatchDocument                | Uitgiftedocument                       |
| ElectrodeData                   | Elektrodegegevens                      |
| cableNumber                     | Kabelnummer                            |
| electrodeNumber                 | Elektrodenummer                        |
| electrodePosition               | Elektrodepositie                       |
| electrodeStatus                 | Elektrodestatus                        |
| tubeNumber                      | Buisnummer                             |
| eventData                       | Resultaat gebeurtenis                  |
| electrodeData                   | Elektrodegegevens                      |
| tubeData                        | Buisgegevens                           |
| wellData                        | Putgegevens                            |
| GeoOhmCable                     | Geo-ohmkabel                           |
| cableInUse                      | Kabel in gebruik                       |
| cableNumber                     | Kabelnummer                            |
| GroundwaterMonitoringWell       | Grondwatermonitoringput                |
| constructionStandard            | Kwaliteitsnorm inrichting              |
| deliveryContext                 | Kader aanlevering                      |
| groundLevelStable               | Maaiveld stabiel                       |
| initialFunction                 | Initiële functie                       |
| maintenanceResponsibleParty     | Onderhoudende instantie                |
| NITGCode                        | NITG-code                              |
| numberOfMonitoringTubes         | Aantal buizen                          |
| owner                           | Eigenaar                               |
| removed                         | Opgeruimd                              |
| wellCode                        | Putcode                                |
| wellHeadProtector               | Beschermconstructie                    |
| wellStability                   | Putstabiliteit                         |
| withPrehistory                  | Met voorgeschiedenis                   |
| IntermediateEvent               | Tussentijdse gebeurtenis               |
| eventDate                       | Datum gebeurtenis                      |
| eventName                       | Naam gebeurtenis                       |
| MonitoringTube                  | Monitoringbuis                         |
| artesianWellCapPresent          | Voorzien van drukdop                   |
| numberOfGeoOhmCables            | Aantal geo-ohmkabels                   |
| sedimentSumpPresent             | Voorzien van zandvang                  |
| tubeInUse                       | Buis in gebruik                        |
| tubeNumber                      | Buisnummer                             |
| tubePartInserted                | Buisdeel geplaatst                     |
| tubeTopDiameter                 | Diameter bovenkant buis                |
| tubeTopPosition                 | Positie bovenkant buis                 |
| tubeTopPositioningMethod        | Methode positiebepaling bovenkant buis |
| tubeStatus                      | Buisstatus                             |
| tubeType                        | Buistype                               |
| variableDiameter                | Variabele diameter                     |
| Screen                          | Filter                                 |
| screenBottomPosition            | Positie onderkant filter               |
| screenLength                    | Filterlengte                           |
| screenTopPosition               | Positie bovenkant filter               |
| sockMaterial                    | Kousmateriaal                          |
| ScreenPositionRange             | Filterbereik                           |
| deepestScreenTopPosition        | Positie bovenkant diepste filter       |
| shallowestScreenTopPosition     | Positie bovenkant ondiepste filter     |
| StatusOverview                  | Statusoverzicht                        |
| tubeStatus                      | Buisstatus                             |
| TubeData                        | Buisgegevens                           |
| glue                            | Lijm                                   |
| insertedPartDiameter            | Diameter bovenkant ingeplaatst deel    |
| insertedPartLength              | Lengte ingeplaatst deel                |
| insertedPartMaterial            | Materiaal ingeplaatst deel             |
| plainTubePartLength             | Lengte stijgbuisdeel                   |
| screenBottomPosition            | Positie onderkant filter               |
| screenTopPosition               | Positie bovenkant filter               |
| tubeMaterial                    | Buismateriaal                          |
| tubeNumber                      | Buisnummer                             |
| tubePartInserted                | Buisdeel ingeplaatst                   |
| tubeStatus                      | Buisstatus                             |
| tubeTopDiameter                 | Diameter bovenkant buis                |
| tubeTopPosition                 | Positie bovenkant buis                 |
| tubeTopPositioningMethod        | Methode positiebepaling bovenkant buis |
| variableDiameter                | Variabele diameter                     |
| VerticalPositionRange           | Verticaal interval                     |
| endDepth                        | Einddiepte                             |
| startDepth                      | Begindiepte                            |
| WellData                        | Putgegevens                            |
| groundLevelPosition             | Maaiveldpositie                        |
| groundLevelPositioningMethod    | Methode positiebepaling maaiveld       |
| maintenanceResponsibleParty     | Onderhoudende instantie                |
| owner                           | Eigenaar                               |
| wellHeadProtector               | Beschermconstructie                    |
| wellHistory                     | Putgeschiedenis                        |
| wellConstructionDate            | Inrichtingsdatum put                   |
| wellRemovalDate                 | Opruimingsdatum put                    |

### A2: gmwcommon

| Engels                       | Nederlands                          |
|------------------------------|-------------------------------------|
| DeliveredLocation            | Aangeleverde locatie                |
| coordinates                  | Coördinaten                         |
| CRS                          | Referentiestelsel                   |
| horizontalPositioningMethod  | Methode locatiebepaling             |
| DeliveredVerticalPosition    | Aangeleverde verticale positie      |
| groundLevelPosition          | Maaiveldpositie                     |
| groundLevelPositioningMethod | Methode positiebepaling maaiveld    |
| localVerticalReferencePoint  | Lokaal verticaal referentiepunt     |
| offset                       | Verschuiving                        |
| verticalDatum                | Verticaal referentievlak            |
| Electrode                    | Elektrode                           |
| electrodeNumber              | Elektrodenummer                     |
| electrodePackingMaterial     | Aanvulmateriaal elektrode           |
| electrodePosition            | Elektrodepositie                    |
| electrodeStatus              | Elektrodestatus                     |
| InsertedPart                 | Ingeplaatst deel                    |
| insertedPartDiameter         | Diameter bovenkant ingeplaatst deel |
| insertedPartLength           | Lengte ingeplaatst deel             |
| insertedPartMaterial         | Materiaal ingeplaatst deel          |
| MaterialUsed                 | Toegepast materiaal                 |
| glue                         | Lijm                                |
| tubeMaterial                 | Buismateriaal                       |
| tubePackingMaterial          | Aanvulmateriaal buis                |
| PlaintubePart                | Stijgbuisdeel                       |
| plainTubePartLength          | stijgbuisdeellengte                 |
| SedimentSump                 | Zandvang                            |
| sedimentSumpLength           | Zandvanglengte                      |

### A3: brocommon

| Engels                     | Nederlands                           |
|----------------------------|--------------------------------------|
| AbortReason                | Reden afbreken                       |
| sequenceNumber             | Volgnummer                           |
| specification              | Foutmelding                          |
| Area                       | Gebied                               |
| boundingBox                | Omsluitende rechthoek                |
| enclosingCircle            | Omsluitende cirkel                   |
| Characteristics            | Kengegevens                          |
| broId                      | BRO-ID                               |
| deliveryAccountableParty   | Bronhouder                           |
| deregistered               | Uit registratie genomen              |
| latestCorrectionTime       | Tijdstip laatste correctie           |
| objectRegistrationTime     | Tijdstip registratie object          |
| qualityRegime              | Kwaliteitsregime                     |
| underReview                | In onderzoek                         |
| Circle                     | Cirkel                               |
| center                     | Middelpunt                           |
| radius                     | Straal                               |
| srsName                    | Referentiestelsel                    |
| CorrectionRequest          | Correctieverzoek                     |
| broId                      | BRO-ID                               |
| deliveryAccountableParty   | Bronhouder                           |
| qualityRegime              | Kwaliteitsregime                     |
| requestReference           | Verzoekkenmerk                       |
| underPrivilege             | Onder voorrecht                      |
| CriteriaSet                | Kenmerkenverzameling                 |
| correctionPeriod           | Periode van correctie                |
| deliveryAccountableParty   | Bronhouder                           |
| qualityRegime              | Kwaliteitsregime                     |
| registrationPeriod         | Periode van registratie              |
| underReview                | In onderzoek                         |
| CriterionError             | Kenmerkfout                          |
| sequenceNumber             | Volgnummer                           |
| specification              | Foutmelding                          |
| DatePeriod                 | Datuminterval                        |
| beginDate                  | Begindatum                           |
| endDate                    | Einddatum                            |
| DeregisteredObject         | Object uit registratie genomen       |
| broId                      | BRO-ID                               |
| deregistered               | Uit registratie genomen              |
| deregistrationTime         | Tijdstip uit registratie genomen     |
| DispatchDataRequest        | Verzoek tot verzending gegevens      |
| broId                      | BRO-ID                               |
| requestReference           | Verzoekkenmerk                       |
| DispatchResponse           | Bericht van verzending               |
| dispatchTime               | Tijdstip van uitgifte                |
| rejectionReason            | Reden afwijzing                      |
| rejectionTime              | Tijdstip van afwijzing               |
| requestReference           | Verzoekkenmerk                       |
| responseType               |                                      |
| IntakeResponse             | Bericht van registratie              |
| acceptanceTime             | Tijdstip van acceptatie              |
| broId                      | BRO-ID                               |
| completionTime             | Tijdstip van verwerking              |
| objectIdAccountableParty   | Object-ID bronhouder                 |
| rejectionReason            | Reden afwijzing                      |
| rejectionTime              | Tijdstip van afwijzing               |
| requestReference           | Verzoekkenmerk                       |
| responseType               |                                      |
| transactionId              | Transactie-ID                        |
| ParseFault                 | Validatiefout                        |
| abortTime                  | Moment van afbreken                  |
| requestReference           | Verzoekkenmerk                       |
| transactionId              | Transactiecode                       |
| PartialDate                | Onvolledige datum                    |
| date                       | Datum tot op de dag nauwkeurig       |
| voidReason                 | Geen datum bekend                    |
| year                       | Datum tot op het jaar nauwkeurig     |
| yearMonth                  | Datum tot op de maand nauwkeurig     |
| Radius                     | Straal                               |
| uom (unit of measure)      | Eenheid                              |
| value                      | Waarde                               |
| RegistrationHistory        | Registratiegeschiedenis              |
| corrected                  | Gecorrigeerd                         |
| deregistered               | Uit registratie genomen              |
| deregistrationTime         | Tijdstip uit registratie genomen     |
| latestAdditionTime         | Tijdstip laatste aanvulling          |
| latestCorrectionTime       | Tijdstip laatste correctie           |
| objectRegistrationTime     | Tijdstip registratie object          |
| registrationCompletionTime | Tijdstip voltooiing registratie      |
| registrationStatus         | Registratiestatus                    |
| reregistered               | Weer in registratie genomen          |
| reregistrationTime         | Tijdstip weer in registratie genomen |
| underReview                | In onderzoek                         |
| underReviewTime            | In onderzoek sinds                   |
| RegistrationObject         | Registratieobject                    |
| broId                      | BRO-ID                               |
| deliveryAccountableParty   | Bronhouder                           |
| deliveryResponsibleParty   | Dataleverancier                      |
| objectIdAccountableParty   | Object-ID bronhouder                 |
| qualityRegime              | Kwaliteitsregime                     |
| RegistrationRequest        | Registratieverzoek                   |
| broId                      | BRO-ID                               |
| deliveryAccountableParty   | Bronhouder                           |
| requestReference           | Verzoekkenmerk                       |
| qualityRegime              | Kwaliteitsregime                     |
| underPrivilege             | Onder voorrecht                      |
| SourceDocumentError        | Brondocumentfout                     |
| sequenceNumber             | Volgnummer                           |
| specification              | Foutmelding                          |
| StandardizedLocation       | Gestandaardiseerde locatie           |
| coordinateTransformation   | Coördinaattransformatie              |
| CRS                        | Referentiestelsel                    |
| location                   | Coördinaten                          |
| srsName                    | Referentiestelsel                    |

### A4: Domeinen van het type codelijst

**GMW codelijsten**

Codespace URI: urn:bro:gmw:\<Engelse naam\>

| Engelse naam                 | Nederlandse naam                       |
|------------------------------|----------------------------------------|
| ConstructionStandard         | Kwaliteitsnorm inrichting              |
| CorrectionReason             | Correctie reden                        |
| DeliveryContext              | Kader aanlevering                      |
| ElectrodePackingMaterial     | Aanvulmateriaal elektrode              |
| ElectrodePositioningMethod   | Methode positiebepaling elektrode      |
| ElectrodeStatus              | Elektrodestatus                        |
| EventName                    | Naam gebeurtenis                       |
| Glue                         | Lijm                                   |
| GroundLevelPositioningMethod | Methode positiebepaling maaiveld       |
| HorizontalPositioningMethod  | Referentiestelsel                      |
| InitialFunction              | Initiële functie                       |
| LocalVerticalReferencePoint  | Lokaal verticaal referentiepunt        |
| SockMaterial                 | Kousmateriaal                          |
| TubeMaterial                 | Buismateriaal                          |
| TubePackingMaterial          | Aanvulmateriaal buis                   |
| TubeStatus                   | Buisstatus                             |
| TubeTopPositioningMethod     | Methode positiebepaling bovenkant buis |
| TubeType                     | Buistype                               |
| VerticalDatum                | Verticaal referentievlak               |
| WellHeadProtector            | Beschermconstructie                    |
| WellStability                | Putstabiliteit                         |

**BRO algemene codelijsten**

Codespace URI: urn:bro:\<Engelse term\>

| Engelse naam             | Nederlandse naam        |
|--------------------------|-------------------------|
| CoordinateTransformation | Coördinaattransformatie |
| CorrectionReason         | Correctie reden         |
| DeliveryContext          | Kader aanlevering       |
| RegistrationStatus       | Registratiestatus       |

Bijlage B: Voorbeeldberichten
-----------------------------

Deze bijlage bevat enkele voorbeeld XML berichten om een beeld te krijgen hoe
die eruit kunnen zien. Een digitale versie van deze en meer voorbeeld XML
berichten kunt u vinden op [www.broinfo.nl](http://www.broinfo.nl).

### DispatchCharacteristicsRequest

Met onderstaande voorbeeldbericht worden de kengegevens gevraagd van alle putten
binnen een bepaalde cirkel en met een bepaalde bronhouder.

| \<dispatchCharacteristicsRequest xmlns=*"http://www.broservices.nl/xsd/dsgmw/1.0"* xmlns:gmwcommon=*"http://www.broservices.nl/xsd/gmwcommon/1.0"* xmlns:brocom=*"http://www.broservices.nl/xsd/brocommon/3.0"* xmlns:gml=*"http://www.opengis.net/gml/3.2"* xmlns:xsi=*"http://www.w3.org/2001/XMLSchema-instance"* xsi:schemaLocation=*"http://www.broservices.nl/xsd/dsgmw/1.0 http://www.broservices.nl/xsd/dsgmw/1.0/dsgmw-messages.xsd"*\> \<requestReference\>levering1-20150728\</requestReference\> \<criteria\> \<brocom:deliveryAccountableParty\>B07F0076\</brocom:deliveryAccountableParty\> \<brocom:registrationPeriod\> \<brocom:beginDate\>2016-05-24\</brocom:beginDate\> \<brocom:endDate\>2017-12-31\</brocom:endDate\> \</brocom:registrationPeriod\> \<brocom:area\> \<brocom:enclosingCircle srsName=*"urn:ogc:def:crs:EPSG::4258"*\> \<brocom:center\>52.090653459 5.121301739\</brocom:center\> \<brocom:radius uom=*"km"*\>10.000\</brocom:radius\> \</brocom:enclosingCircle\> \</brocom:area\> \</criteria\> \</dispatchCharacteristicsRequest\> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


### DispatchDataRequest

Met onderstaande voorbeeldbericht worden de gegevens van een bepaalde put
opgevraagd.

| \<dispatchDataRequest xmlns=*"http://www.broservices.nl/xsd/dsgmw/1.0"* xmlns:gmwcommon=*"http://www.broservices.nl/xsd/gmwcommon/1.0"* xmlns:brocom=*"http://www.broservices.nl/xsd/brocommon/3.0"* xmlns:gml=*"http://www.opengis.net/gml/3.2"* xmlns:xsi=*"http://www.w3.org/2001/XMLSchema-instance"* xsi:schemaLocation=*"http://www.broservices.nl/xsd/dsgmw/1.0 http://www.broservices.nl/xsd/dsgmw/1.0/dsgmw-messages.xsd"*\> \<brocom:requestReference\>levering2-20150728\</brocom:requestReference\> \<brocom:broId\>GMW000000046027\</brocom:broId\> \<dataToBeDelivered\>actueelHistorisch\</dataToBeDelivered\> \</dispatchDataRequest\> |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


### DispatchDataResponse – gebruiksfout

Voorbeeld van een *response* als er een gebruiksfout in het request wordt
geconstateerd.

| \<dispatchDataResponse xmlns=*"http://www.broservices.nl/xsd/dsgmw/1.0"* xmlns:gmwcommon=*"http://www.broservices.nl/xsd/gmwcommon/1.0"* xmlns:brocom=*"http://www.broservices.nl/xsd/brocommon/3.0"* xmlns:gml=*"http://www.opengis.net/gml/3.2"* xmlns:xsi=*"http://www.w3.org/2001/XMLSchema-instance"* xsi:schemaLocation=*"http://www.broservices.nl/xsd/dsgmw/1.0 http://www.broservices.nl/xsd/dsgmw/1.0/dsgmw-messages.xsd"*\> \<brocom:responseType\>rejection\</brocom:responseType\> \<brocom:requestReference\>levering2-20150728\</brocom:requestReference\> \<brocom:rejectionTime\>2017-06-13T14:08:39+01:00\</brocom:rejectionTime\> \<brocom:rejectionReason\>*Dit registratieobject bestaat niet*.\</brocom:rejectionReason\> \</dispatchDataResponse\> |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


### Softwarefout

Voorbeeld van de situatie dat een softwarefout in het systeem van de
data-afnemer wordt geconstateerd.

| \<soap:Fault xmlns:soap=*"http://schemas.xmlsoap.org/soap/envelope/"*\> \<faultcode\>soap:Client\</faultcode\> \<faultstring\>*Het verzoek voldoet niet aan het* schema.\</faultstring\> \<detail\> \<parseFault xmlns:brocom=*"http://www.broservices.nl/xsd/brocommon/3.0"* xmlns=*"http://www.broservices.nl/xsd/dsgmw/1.0"*\> \<brocom:requestReference\>levering1-20150728\</brocom:requestReference\> \<brocom:transactionId\>GMW-000000142872\</brocom:transactionId\> \<brocom:abortTime\>2017-06-13T14:08:39+01:00\</brocom:abortTime\> \<brocom:abortReason\> \<brocom:sequenceNumber\>1\</brocom:sequenceNumber\> \<brocom:specification\>*regel*: 1, *kolom*: 2895, offset: -1, *boodschap*: 'null'\</brocom:specification\> \</brocom:abortReason\> \<brocom:abortReason\> \<brocom:sequenceNumber\>2\</brocom:sequenceNumber\> \<brocom:specification\>*regel*: 1, *kolom*: 2895, offset: -1, *boodschap*: '*cvc*-*datatype*-valid.1.2.1: '*abcd*' is not a valid value for 'date'.'\</brocom:specification\> \</brocom:abortReason\> \<brocom:abortReason\> \<brocom:sequenceNumber\>3\</brocom:sequenceNumber\> \<brocom:specification\>*regel*: 1, *kolom*: 2895, offset: -1, *boodschap*: '*cvc*-complex-type.2.2: Element 'ns:deliveryAccountableParty' must have no element [children], and the value must be valid.'\</brocom:specification\> \</brocom:abortReason\> \</parseFault\> \</detail\> \</soap:Fault\> |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


### Systeemfout

Voorbeeld van de situatie dat er een systeemfout optreedt in het BRO-systeem.

| \<soap:Fault xmlns:soap=*"http://schemas.xmlsoap.org/soap/envelope/"*\> \<faultcode\>soap:Client\</faultcode\> \<faultstring\>*Er* is *een fout* in *het* BRO-*systeem geconstateerd*.\</faultstring\> \<detail\> \<abortTime\>2017-06-13T14:08:39+01:00\</abortTime\> \</detail\> \</soap:Fault\> |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

