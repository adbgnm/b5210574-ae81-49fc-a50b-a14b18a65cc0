Basisregistratie Ondergrond (BRO) Koppelvlakbeschrijving

GMW Innamewebservice

Colofon

|                  | Bestuurskern Dir. Ruimtelijke Ontwikkeling Rijnstraat 8 2515 XP Den Haag  |
|------------------|---------------------------------------------------------------------------|
|                  |                                                                           |
| Algemeen Contact | Programmabureau BRO Directoraat-Generaal Ruimte en Water <bro@minienm.nl> |
|                  |                                                                           |
| Versie           | 1.0.3                                                                     |
|                  |                                                                           |
| Auteur           | TNO Geologische Dienst Nederland                                          |
|                  |                                                                           |

**Inhoudsopgave**

[1 Inleiding 8](#inleiding)

[1.1 Doel en doelgroep 8](#doel-en-doelgroep)

[1.2 Gebruik van dit document 8](#gebruik-van-dit-document)

[1.3 Samenhang met andere formele documentatie
8](#samenhang-met-andere-formele-documentatie)

[1.4 Leeswijzer 9](#leeswijzer)

[1.5 Referenties 9](#referenties)

[1.6 Versiehistorie 9](#versiehistorie)

[1.7 Contact 10](#contact)

[2 Aanbieden van grondwatermonitoringput
11](#aanbieden-van-grondwatermonitoringput)

[2.1 Inleiding 11](#inleiding-1)

[2.2 Communicatie tussen twee systemen 11](#communicatie-tussen-twee-systemen)

[2.3 Communicatiestandaarden 11](#communicatiestandaarden)

[2.3.1 Gegevens- en berichtenstandaarden 12](#gegevens--en-berichtenstandaarden)

[2.3.2 Logistieke standaard 12](#logistieke-standaard)

[2.3.3 Netwerkstandaard 13](#netwerkstandaard)

[2.4 Toegangscontrole 13](#toegangscontrole)

[3 API voor het aanbieden van grondwatermonitoringput
14](#api-voor-het-aanbieden-van-grondwatermonitoringput)

[3.1 Inleiding 14](#inleiding-2)

[3.2 Operaties 14](#operaties)

[3.2.1 Register 14](#register)

[3.2.2 Replace 14](#replace)

[3.2.3 Insert 15](#insert)

[3.2.4 Move 15](#move)

[3.2.5 Delete 15](#delete)

[3.3 Verwerking 16](#verwerking)

[3.3.1 Registratie 16](#registratie)

[3.3.2 Correctie 17](#correctie)

[3.4 Berichten bij registratie starten 18](#berichten-bij-registratie-starten)

[3.4.1 Request: registratieverzoek 18](#request-registratieverzoek)

[3.4.2 Response: bericht van afwijzing 19](#response-bericht-van-afwijzing)

[3.4.3 Response: bericht van registratie 20](#response-bericht-van-registratie)

[3.5 Berichten bij registratie aanvullen en beëindigen
20](#berichten-bij-registratie-aanvullen-en-beëindigen)

[3.5.1 Request: registratieverzoek 20](#request-registratieverzoek-1)

[3.5.2 Response: bericht van afwijzing 21](#response-bericht-van-afwijzing-1)

[3.5.3 Response: bericht van registratie
21](#response-bericht-van-registratie-1)

[3.6 Berichten bij correctie 22](#berichten-bij-correctie)

[3.6.1 Request: correctieverzoek 22](#request-correctieverzoek)

[3.6.2 Response: bericht van afwijzing 22](#response-bericht-van-afwijzing-2)

[3.6.3 Response: bericht van acceptatie 23](#response-bericht-van-acceptatie)

[3.7 Berichten bij technische fouten 24](#berichten-bij-technische-fouten)

[3.7.1 Softwarefout 24](#softwarefout)

[3.7.2 Systeemfouten 24](#systeemfouten)

[4 Modellering van het interface 25](#modellering-van-het-interface)

[4.1 Packagestructuur 25](#packagestructuur)

[4.2 Modelleerregels 26](#modelleerregels)

[4.2.1 CodeList 26](#codelist)

[4.2.2 DataType 26](#datatype)

[4.2.3 Enumeration 26](#enumeration)

[4.2.4 FeatureType 27](#featuretype)

[4.2.5 Type 27](#type)

[4.2.6 Union 27](#union)

[4.2.7 Voidable 27](#voidable)

[5 Package isgmw – de innamewebservice interface
28](#package-isgmw-de-innamewebservice-interface)

[5.1 De WSDL 28](#de-wsdl)

[5.1.1 Types 28](#types)

[5.1.2 Message 28](#message)

[5.1.3 PortType 29](#porttype)

[5.1.4 Binding 29](#binding)

[5.1.5 Service 29](#service)

[5.2 De XSD-bestanden 29](#de-xsd-bestanden)

[6 Package isgmw-messages – de berichten XSD
30](#package-isgmw-messages-de-berichten-xsd)

[6.1 RegistrationRequest 30](#registrationrequest)

[6.2 CorrectionRequest 31](#correctionrequest)

[6.3 MoveRequest 31](#moverequest)

[6.4 CorrectionReason 31](#correctionreason)

[6.5 SourceDocument 32](#sourcedocument)

[6.5.1 GMW\_Construction 33](#gmw_construction)

[6.5.2 GMW\_ElectrodeStatus 33](#gmw_electrodestatus)

[6.5.3 GMW\_GroundLevel 34](#gmw_groundlevel)

[6.5.4 GMW\_Insertion 34](#gmw_insertion)

[6.5.5 GMW\_Lengthening 34](#gmw_lengthening)

[6.5.6 GMW\_Maintainer 35](#gmw_maintainer)

[6.5.7 GMW\_Owner 35](#gmw_owner)

[6.5.8 GMW\_Positions 35](#gmw_positions)

[6.5.9 GMW\_Removal 35](#gmw_removal)

[6.5.10 GMW\_Shift 36](#gmw_shift)

[6.5.11 GMW\_Shortening 36](#gmw_shortening)

[6.5.12 GMW\_TubeStatus 36](#gmw_tubestatus)

[6.5.13 GMW\_WellHeadProtector 36](#gmw_wellheadprotector)

[6.5.14 GeoOhmCable 37](#geoohmcable)

[6.5.15 MonitoringTube 37](#monitoringtube)

[6.5.16 Screen 38](#screen)

[7 Package gmwcommon 39](#package-gmwcommon)

[7.1 Codelijsten 39](#codelijsten)

[7.2 DeliveredLocation 39](#deliveredlocation)

[7.3 DeliveredVerticalPosition 40](#deliveredverticalposition)

[7.4 Electrode 40](#electrode)

[7.5 InsertedPart 40](#insertedpart)

[7.6 MaterialUsed 40](#materialused)

[7.7 Meetwaarden 41](#meetwaarden)

[7.8 PlainTubePart 42](#plaintubepart)

[7.9 SedimentSump 42](#sedimentsump)

[8 Package brocommon 43](#package-brocommon)

[8.1 AbortReason 43](#abortreason)

[8.2 Area 43](#area)

[8.3 Characteristics 43](#characteristics)

[8.4 ChamberOfCommerceNumber 44](#chamberofcommercenumber)

[8.5 Circle 44](#circle)

[8.6 CoordinateTransformation 44](#coordinatetransformation)

[8.7 CorrectionRequest 45](#correctionrequest-1)

[8.8 CriteriaSet 45](#criteriaset)

[8.9 CriterionError 45](#criterionerror)

[8.10 DatePeriod 46](#dateperiod)

[8.11 DeregisteredObject 46](#deregisteredobject)

[8.12 DispatchDataRequest 46](#dispatchdatarequest)

[8.13 DispatchResponse 47](#dispatchresponse)

[8.14 Enumeraties 47](#enumeraties)

[8.15 IntakeResponse 48](#intakeresponse)

[8.16 ParseFault 49](#parsefault)

[8.17 PartialDate 50](#partialdate)

[8.18 Radius 51](#radius)

[8.19 RegistrationHistory 51](#registrationhistory)

[8.20 RegistrationObject 51](#registrationobject)

[8.21 RegistrationObjectCode 52](#registrationobjectcode)

[8.22 RegistrationRequest 52](#registrationrequest-1)

[8.23 RegistrationStatus 53](#registrationstatus)

[8.24 SOAP Fault 53](#soap-fault)

[8.25 SourceDocumentError 54](#sourcedocumenterror)

[8.26 StandardizedLocation 54](#standardizedlocation)

[9 Package gml-profile 56](#package-gml-profile)

[9.1 AbstractFeature 56](#abstractfeature)

[9.2 AbstractGML 56](#abstractgml)

[9.3 CodeWithAuthority 56](#codewithauthority)

[9.4 Doublelist 57](#doublelist)

[9.5 Envelope 58](#envelope)

[9.6 Measure 58](#measure)

[9.7 Point 59](#point)

[9.8 TM\_TimeInstant 60](#tm_timeinstant)

[9.9 TM\_Position 60](#tm_position)

[10 Package xlink-profile 62](#package-xlink-profile)

[10.1 Href 62](#href)

[10.2 HrefType 62](#hreftype)

[10.3 SimpleAttrs 62](#simpleattrs)

[10.4 Type 62](#type-1)

[10.5 TypeType 63](#typetype)

[11 Bijlagen 64](#bijlagen)

[11.1 Bijlage A: Vertaalslag Engels – Nederlands
64](#bijlage-a-vertaalslag-engels-nederlands)

[11.1.1 A1: isgmw-messages 64](#a1-isgmw-messages)

[11.1.2 A2: gmwcommon 67](#a2-gmwcommon)

[11.1.3 A3: brocommon 67](#a3-brocommon)

[11.1.4 A4: Domeinen van het type codelijst
69](#a4-domeinen-van-het-type-codelijst)

[11.2 Bijlage B: Voorbeeldberichten 70](#bijlage-b-voorbeeldberichten)

[11.2.1 RegistrationRequest – start registratie
70](#registrationrequest-start-registratie)

[11.2.2 RegistrationRequest – aanvullen nieuwe eigenaar
73](#registrationrequest-aanvullen-nieuwe-eigenaar)

[11.2.3 CorrectionRequest – eigenaar invoegen
73](#correctionrequest-eigenaar-invoegen)

[11.2.4 IntakeResponse – bericht van registratie
74](#intakeresponse-bericht-van-registratie)

[11.2.5 IntakeResponse – bericht van afwijzing
74](#intakeresponse-bericht-van-afwijzing)

[11.2.6 Softwarefout 74](#softwarefout-1)

[11.2.7 Systeemfout 75](#systeemfout)

Inleiding
=========

Dit document beschrijft het koppelvlak van de innamewebservice voor het
registratieobject grondwatermonitoringput (GMW) voor de Basisregistratie
Ondergrond (BRO). Deze koppelvlakbeschrijving gaat in op de technische werking
van het koppelvlak om GMW-gegevens uit te kunnen wisselen tussen het systeem van
de dataleverancier en het systeem van de BRO.

Doel en doelgroep
-----------------

Doel van dit document is inzicht bieden in de werking van de innamewebservice.
Het proces van gegevensinname zoals beschreven in het ‘Innamehandboek
Grondwatermonitoringput’ (zie [www.broninfo.nl](http://www.broninfo.nl)) is in
dit document vertaald naar het technische koppelvlak van de webservice: de
Application Programming Interface (API).

Dit document richt zich op de technisch specialisten die de aansluiting
realiseren tussen de systemen van de dataleveranciers en het systeem van de BRO.
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

![](media/3ade381ef6ecc8e316546bfbca8ce2bf.png)

Leeswijzer
----------

Hoofdstuk 2 beschrijft de algemene technische werking van het koppelvlak van de
innamewebservice. Dit hoofdstuk is bedoeld voor de lezer die een globaal idee
wil krijgen hoe de geautomatiseerde gegevensuitwisseling van de BRO werkt.

Hoofdstuk 3 beschrijft vervolgens het koppelvlak van de GMW innamewebservice in
technische termen: de Application Programming Interface (API). De
functionaliteit voor registratie en de functionaliteit voor correctie komen
daarbij aan bod.

De hoofdstukken 4 en verder beschrijven het UML-model van de innamewebservice.
Dezelfde structuur is van toepassing op de WSDL en XSD-bestanden van de
innamewebservice.

Bijlage A bevat de vertalingen van de berichten en de codelijsten van het Engels
naar het Nederlands. Deze bijlage is een praktisch hulpmiddel aangezien de
Engelstalige XML-berichten gebaseerd zijn op Nederlandse definities uit het
innamehandboek en de catalogus.

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

| Versie | Datum            | Omschrijving                                                                                                                                                                                                                           |
|--------|------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 0.7    | 17 oktober 2016  | Initiële versie                                                                                                                                                                                                                        |
| 0.7.2  | 2 december 2016  | Bijgewerkt n.a.v. profielen op OGC                                                                                                                                                                                                     |
| 0.7.3  | 27 januari 2017  | Bijgewerkt m.b.t. correctieverzoeken (correctie types invoegen en vervangen voor eigenaar, oplenging en inrichting).                                                                                                                   |
| 0.8.0  | 16 mei 2017      | Correctie types verplaatsen en verwijderen toegevoegd. Consolidatie met andere registratieobjecten.                                                                                                                                    |
| 1.0    | 21 juni 2017     | Bijgewerkt n.a.v. review commentaar.                                                                                                                                                                                                   |
| 1.0.1  | 25 juli 2017     | Stereotype FeatureType toegevoegd aan RegistrationObject                                                                                                                                                                               |
| 1.0.2  | 26 juli 2017     | Figuur in 6.5.1 vervangen i.v.m. toevoegen NITGCode en wellCode, tabel in 11.1.1 uitgebreid met details van GMW\_Constuction, tabel in 11.1.3 gecompleteerd i.r.t.. hoofdstuk 8 en voorbeeldbericht in 11.2.1 uitgebreid met NITGCode. |
| 1.0.3  | 8 september 2017 | Figuur in 6.3 vervangen en tekst bij dateToBeCorrected in paragrafen 3.6.1 en 6.3 aangevuld als mogelijkerwijs onvolledige datum.                                                                                                      |

Contact
-------

Algemene informatie, documentatie en voorbeeld XML berichten kunt u vinden op
www.broinfo.nl.

Als uw organisatie is aangemeld bij de BRO kunt u voor vragen, suggesties of
opmerkingen contact opnemen met de BRO Selfservicedesk via support.gdnnet.nl.

In alle andere gevallen kunt u contact opnemen met de BRO Servicedesk via
info\@basisregistratieondergrond.nl.

Aanbieden van grondwatermonitoringput
=====================================

Inleiding
---------

Dit hoofdstuk beschrijft hoe het aanbieden van gegevens van een
grondwatermonitoringput werkt. Hierbij wordt ingegaan op de algemene technische
werking van het koppelvlak van de GMW innamewebservice. Er wordt uitgelegd hoe
het systeem van de dataleverancier en het BRO-systeem communiceren en welke
standaarden worden gehanteerd. Dit geeft een beeld hoe de geautomatiseerde
gegevensuitwisseling met de BRO werkt.

Communicatie tussen twee systemen
---------------------------------

Een dataleverancier kan geautomatiseerd gegevens van een grondwatermonitoringput
aanbieden bij de BRO via de GMW innamewebservice. Het systeem van de
dataleverancier stuurt hiervoor een verzoek (*request*) aan de GMW
innamewebservice van de BRO. Het systeem van de BRO reageert op dit verzoek met
een antwoord (*response*). Deze *response* bevat het resultaat van de verwerking
van het *request*. Onderstaande afbeelding geeft dit schematisch weer.

![](media/30c4c4b3b78e65901b61feeca4de79ff.png)

Via het verzoek aan de GMW innamewebservice kunnen verschillende bewerkingen
(*operaties*) van GMW-gegevens worden gestart. Elke operatie heeft een eigen
*request* en een eigen *response*. De GMW innamewebservice is daarmee het
koppelvlak ofwel de Application Programming Interface (API) voor de inname van
GMW.

Communicatiestandaarden
-----------------------

De communicatie tussen het systeem van de dataleverancier en het BRO-systeem
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

![](media/f4991433370998432cd1e3f4fbd750ac.png)

Het WSDL-document (Web Service Definition Language) beschrijft in technische
termen de volledige API (Application Programming Interface) van de GMW
innamewebservice (zie hoofdstuk 3). Het beschrijft de operaties, inclusief
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

API voor het aanbieden van grondwatermonitoringput
==================================================

Inleiding
---------

In dit hoofdstuk wordt het koppelvlak in technische termen beschreven: de API
(Application Programming Interface). Hierbij staan de twee functionaliteiten van
de GMW innamewebservice centraal: functionaliteit voor het registreren van
gegevens en functionaliteit voor het corrigeren van gegevens.

Elke functionaliteit heeft verschillende operaties. Deze worden beschreven in
paragraaf 3.2. Paragraaf 3.3 beschrijft het patroon van verwerking van de
operaties. De daaropvolgende paragrafen beschrijven de mapping van de berichten
uit het innamehandboek op *requests* en *responses* in de API. De inhoud van de
*requests/responses* wordt beschreven in hoofdstuk 4 en verder.

Operaties
---------

De innamewebservice voor grondwatermonitoringputten biedt de dataleverancier
basale functionaliteit. De API van de BRO GMW innamewebservice definieert
hiervoor vijf operaties. Elke operatie heeft een eigen *request* en *response*
die de verschillende verzoeken en antwoorden realiseren die in het
innamehandboek zijn beschreven.

### Register

De aard van een grondwatermonitoringput brengt met zich mee dat er drie soorten
gebeurtenissen kunnen worden onderscheiden in de bestaansgeschiedenis van een
put (zie het innamehandboek):

-   Registratie starten  
    Nadat de constructie van een put is voltooid, kan de registratie van de put
    worden gestart. De initiële inrichting van de put wordt geregistreerd in de
    BRO.

-   Registratie aanvullen  
    Nadat een put is geconstrueerd, breekt de gebruiksperiode aan. Als in de
    werkelijkheid[^1] een verandering aan de put optreedt, nadat de put in de
    BRO is geregistreerd, dan moeten de putgegevens in de BRO worden aangevuld
    met de nieuwe informatie. Daarbij wordt over de putgegevens materiële
    geschiedenis (zie de catalogus) opgebouwd. Afhankelijk van de gebeurtenis
    wordt in het request van de register operatie een bepaald brondocument
    opgenomen, met daarin de nieuwe gegevens.

    [^1]: Merk op dat veranderingen in de putgegevens, die niet het gevolg zijn
    van een gebeurtenis in de werkelijkheid, worden verwerkt met een correctie
    operatie en leiden tot het opbouwen van formele geschiedenis (zie de
    catalogus en de volgende paragrafen).

-   Registratie beëindigen  
    Na de gebruiksperiode van de put kan deze worden opgeruimd. Dit wordt in de
    BRO geregistreerd en de put krijgt in de BRO de status voltooid. De
    geregistreerde putgegevens kunnen daarna niet meer worden aangevuld.

De putgegevens naar aanleiding van ieder van deze drie gebeurtenissen kunnen
worden aangeboden met een *register* operatie. Het brondocument in het *request*
geeft aan welke gebeurtenis er is opgetreden.

### Replace

Met deze operatie wordt een eerdere registratie of aanvulling gecorrigeerd door
de desbetreffende gegevens te vervangen door de gegevens in het *request*.

De correctie van het type vervangen is een correctie die **niet** ingrijpt in de
materiële geschiedenis van een put. Alle gebeurtenissen zijn netjes in volgorde
en met de juiste datum geregistreerd. Maar bij een van de transacties zijn een
of meer onjuiste waarden aangeleverd, of zijn niet alle nieuwe gegevens
aangeleverd.

In het eerste geval dient de dataleverancier een verzoek in om die onjuiste
waarde(n) te vervangen, en dat is ook letterlijk wat er in de registratie
ondergrond gebeurt: iedere waarde wordt vervangen. In het tweede geval dient de
dataleverancier een verzoek in waarin uitsluitend de ontbrekende gegevens zijn
opgenomen. In beide gevallen wordt er geen materiële geschiedenis maar
uitsluitend formele geschiedenis opgebouwd (zie innamehandboek).

### Insert

Met deze operatie wordt een ontbrekende aanvulling ingevoegd in de tijdlijn van
de putgeschiedenis.

De correctie van het type invoegen is een correctie die **wel** ingrijpt in de
materiële geschiedenis van een put. Het gaat om de eenvoudigste en meest
voorkomende variant. Namelijk het geval dat de dataleverancier de registratie
had moeten aanvullen, maar dat vergeten was terwijl hij intussen wel een andere
verandering heeft laten registreren.

Om de fout te herstellen, dient de dataleverancier een verzoek in met het doel
de ontbrekende gegevens in te voegen in de tijdlijn met geregistreerde gegevens.
De vergeten gebeurtenis wordt opgenomen in de putgeschiedenis, de betreffende
gegevens krijgen een nieuwe waarde met een begin geldigheid (zie innamehandboek)
en iedere reeds geregistreerde waarde die vanwege de gebeurtenis verandert
krijgt een datum einde geldigheid.

### Move

Met deze operatie wordt een eerdere registratie of aanvulling verplaatst in de
tijdlijn van de putgeschiedenis.

De correctie van het type verplaatsen is een correctie die **wel** ingrijpt in
de materiële geschiedenis van een put. Het gaat om een complexe variant, waarbij
een gebeurtenis is geregistreerd met een foute waarde voor de datum waarop de
gebeurtenis heeft plaatsgevonden.

Om de fout te herstellen, levert de dataleverancier de gegevens uit de eerdere
registratie of aanvulling opnieuw aan in een *move* operatie, nu met het
correcte moment waarop de gebeurtenis heeft plaats gevonden. De gebeurtenis
wordt opgezocht in de putgeschiedenis en verplaatst naar de juiste plek in de
tijdlijn van de putgeschiedenis. Van de betreffende gegevens (rondom de oude
plek in de tijdlijn en de gecorrigeerde plek in de tijdlijn) worden de waarden
voor begin geldigheid (zie innamehandboek) en einde geldigheid aangepast,
afhankelijk van het feit of een gegeven voor of na de verwerking van de *move*
operatie vanwege de verplaatste gebeurtenis van waarde is veranderd of juist
niet meer.

### Delete

Met deze operatie wordt een eerdere aanvulling verwijderd uit de tijdlijn van de
putgeschiedenis.

De correctie van het type verwijderen is een correctie die **wel** ingrijpt in
de materiële geschiedenis van een put. Het gaat om een eenvoudige variant,
waarbij een aanvulling ten onrechte is aangeboden.

Om de fout te herstellen, dient de dataleverancier een verzoek in met het doel
de betreffende gegevens te verwijderen uit de tijdlijn. De gebeurtenis wordt
opgezocht in de putgeschiedenis en verwijderd uit de tijdlijn van de
putgeschiedenis. Van de betreffende gegevens (rondom de verwijderde plek in de
tijdlijn) worden de waarden voor begin geldigheid (zie innamehandboek) en einde
geldigheid aangepast, afhankelijk van het feit of een gegeven voor of na de
verwerking van de *delete* operatie vanwege de verwijderde gebeurtenis van
waarde is veranderd of juist niet meer.

Verwerking
----------

De verwerking van een registratieverzoek of een correctieverzoek verloopt
volgens een vast patroon, maar er is wel een verschil tussen beide type
verzoeken.

### Registratie

De verwerking van een registratieverzoek (de *register* operatie) verloopt
volgens het hierna weergegeven patroon. Een registratie operatie van de GMW
innamewebservice begint bij het doen van een registratieverzoek door middel van
een *request* en eindigt met een *response*.

![](media/3c65661a692afb2df96cc3b619b97fdf.png)

Stap 1: Doen van een registratieverzoek

Het initiatief om een operatie te beginnen ligt bij het systeem van de
dataleverancier. Dat roept de *register* operatie van de GMW innamewebservice
aan met het *registrationRequest* als parameter.

Stap 2: Uitvoeren toegangscontrole

Dit bestaat uit identificatie, authenticatie, versleuteling en autorisatie.

Voor de beveiliging van de gegevensuitwisseling worden, conform de Digikoppeling
specificaties, PKIoverheid services server certificaten gebruikt. Zowel de
dataleverancier als de BRO beschikt over een dergelijk certificaat. In het
certificaat is een **identificatie** op basis van 20 cijfers opgenomen die uniek
is voor de houder van het certificaat.

Op het moment dat het systeem van een dataleverancier een operatie aanroept van
de webservice van het BRO-systeem wisselen beide systemen eerst hun PKIoverheid
services server certificaten uit. Aan de hand van de identificatie in de
certificaten weten beide partijen met wie gegevens­uitwisseling plaatsvindt. De
techniek van het PKIoverheid services server certificaat garandeert dat de
identificatie in het certificaat ook daadwerkelijk van die partij is
(**authenticatie**).

Als authenticatie succesvol is verlopen, worden beide certificaten vervolgens
gebruikt om al het dataverkeer tussen de systemen te **versleutelen**. Deze
versleuteling maakt het voor derden onmogelijk om de data te lezen of te
wijzigen.

Voor het aanbieden van gegevens aan het BRO-systeem zijn rechten nodig. Aan de
hand van de identificatie in het certificaat wordt bepaald of het systeem van de
dataleverancier **geautoriseerd** is de operatie uit te voeren. Als hierbij een
fout optreedt, ontvangt de dataleverancier een melding met een http-statuscode.

Als niet wordt voldaan aan de toegangscontrole, dan leidt dit tot:

-   Een http ‘401 Unauthorized’ foutmelding.

-   Of een ‘ssl error invalid certificate’ foutmelding.

-   Of een andere http-foutmelding met een http-statuscode anders dan ‘200 OK’.

Stap 3: Controleren verzoek

Als de toegangscontrole succesvol is verlopen, dan wordt het *request* technisch
en inhoudelijk gecontroleerd.

De technische controle vindt plaats door het *request* te valideren op basis van
de XSD. Als hierbij fouten gevonden worden, dan worden deze beschouwd als een
technische fout van het systeem van de dataleverancier en teruggegeven als een
*parseFault*.

De inhoudelijke controle vindt plaats door het *request* te controleren volgens
de regels die zijn gedefinieerd in de catalogus of het innamehandboek (*business
rules*). Deze regels zijn niet in de XSD vastgelegd, maar worden gecontroleerd
door de programmatuur van het BRO-systeem. Voorbeelden van controles zijn:

-   Is een waarde niet groter dan de toegestane maximale waarde?

-   Voldoet een waarde aan de toegestane waardes voor een gegeven?

Als hierbij fouten worden gevonden, dan worden deze beschouwd als een
gebruiksfout en teruggegeven in een *response* bericht.

Stap 4: Vastleggen van gegevens

Als alle controles succesvol zijn verlopen dan legt het BRO-systeem de
aangeboden gegevens vast en wordt het resultaat teruggegeven in een *response*
bericht.

### Correctie

De verwerking van een correctieverzoek (de operaties *replace*, *insert*, *move*
en *delete*) verloopt volgens het hieronder weergegeven patroon. In de
verwerking zijn vijf stappen te onderkennen; deze zijn in onderstaande
afbeelding weergegeven en worden vervolgens toegelicht.

![](media/b59551d47c87bc6be00d41ae585f4569.png)

De eerste drie stappen in de verwerking zijn hetzelfde als bij een
registratieverzoek, maar nadat het BRO-systeem heeft gecontroleerd of alles goed
is, neemt de registratiebeheerder de controle over.

Stap 1: Doen van een correctieverzoek

Het initiatief om een operatie te beginnen ligt bij het systeem van de
dataleverancier. Dat roept de desbetreffende operatie van de GMW
innamewebservice aan met het *correctionRequest* als parameter. In het
*correctionRequest* geeft hij aan waarom hij het correctieverzoek indient.

Stap 2: Uitvoeren toegangscontrole

Zie stap 2 bij de beschrijving van de verwerking van een registratieverzoek.

Stap 3: Controleren verzoek

Deze stap lijkt veel op stap 3 bij de beschrijving van de verwerking van een
registratieverzoek. Aanvullende controles, die de programmatuur van het
BRO-systeem uitvoert bij een correctieverzoek, zijn:

-   Bestaat het te corrigeren registratieobject in de BRO?

-   Voldoet het correctieverzoek aan procesmatige eisen? Bijvoorbeeld: mag de
    dataleverancier dit specifieke object corrigeren?

Als bij deze stap fouten worden gevonden, dan worden deze beschouwd als een
gebruiksfout en teruggegeven in een *response* bericht met daarin reden en
tijdstip van afwijzing.

Als hierbij geen fouten worden gevonden, dan wordt het correctieverzoek
geaccepteerd en vastgelegd, maar nog niet verwerkt in de basisregistratie.
Voordat het correctieverzoek wordt verwerkt in de basisregistratie wordt het
verzoek eerst nog beoordeeld door de registratie­beheerder zoals beschreven in
stap 4. Het BRO-systeem reageert met een *response* bericht met daarin het
tijdstip van acceptatie.

Stap 4: Beoordelen correctieverzoek

Nadat het correctieverzoek is vastgelegd neemt de registratiebeheerder de
verwerking over en voert een inhoudelijke controle uit of het correctieverzoek
verwerkt mag worden in de basisregistratie.

Als de registratiebeheerder een correctieverzoek afwijst, dan wordt een *email*
naar de dataleverancier verzonden met daarin reden en tijdstip van bezwaar. Een
beschrijving van de inhoud van deze email valt buiten de scope van deze
koppelvlakbeschrijving; zie het innamehandboek voor nadere informatie. Een
dataleverancier kan het emailadres kenbaar maken tijdens het aanmelden bij de
BRO.

Stap 5: Vastleggen van gegevens

Als alle controles succesvol zijn verlopen dan verwerkt het BRO-systeem de
correctie in de basisregistratie en wordt een *email* naar de dataleverancier
verzonden met daarin het tijdstip van correctie. Een dataleverancier kan het
emailadres kenbaar maken tijdens het aanmelden bij de BRO.

Berichten bij registratie starten
---------------------------------

Bij een *register* operatie zijn drie berichten van toepassing: een
registratieverzoek, een bericht van afwijzing en een bericht van registratie.
Deze paragraaf beschrijft de inhoud van deze berichten bij een ‘registratie
starten’ gebeurtenis.

### Request: registratieverzoek

Onderstaande figuur geeft de mapping weer van het registratieverzoek in het
innamehandboek op het datatype *RegistrationRequest* in dit document (zie
paragraaf 6.1), zoals gebruikt door de *register* operatie (zie hoofdstuk 5).

![](media/937a4f729f3fc0f04961828976b10e6a.png)

Het element brondocumenttype in het registratieverzoek komt niet voor in het
*RegistrationRequest*, omdat dit gegeven impliciet bekend is gegeven de inhoud
van het element *sourceDocument*.

Het element *sourceDocument* bevat alle gegevens die in de catalogus voor het
registratieobject grondwatermonitoringput zijn gespecificeerd, met uitzondering
van de gegevens die door het BRO-systeem worden gegenereerd of afgeleid uit het
*RegistrationRequest*.

### Response: bericht van afwijzing

Het innamehandboek benoemt als mogelijke reactie op een registratieverzoek een
bericht van afwijzing. De webservice gebruikt hiervoor een *response* van het
datatype *IntakeResponse*.

![](media/192610fbcafbbfeba82314df3162f055.png)

Het handboek definieert een aantal berichten als antwoord op een innameverzoek.
In de SOAP webservice definities mag elk *request* slechts een *response*
hebben. Daarom is het element *responseType* toegevoegd, om de betekenis van de
*response* te duiden. In dit geval heeft het element *responseType* de vaste
waarde *rejection*.

De waarde van de elementen *requestReference* en *objectIdAccountableParty*
wordt overgenomen uit het *request* c.q. het *sourceDocument* in het *request*.
De waarde van de overige elementen wordt toegekend door de webservice. Het
element *rejectionReason* bevat een waarde uit de tabel met gebruiksfouten; zie
het innamehandboek.

Als deze *response* wordt gegeven omdat er een of meer gebruiksfouten in het
*sourceDocument* zijn geconstateerd, dan is de waarde van *rejectionReason* “er
zijn 1 of meer fouten geconstateerd in het brondocument” en volgen er na dit
element een of meer *sourceDocumentErrors*.

Zie paragraaf 8.15 voor nadere details.

### Response: bericht van registratie

Het innamehandboek benoemt als mogelijke reactie op een registratieverzoek een
bericht van registratie. De webservice gebruikt hiervoor een *response* van het
datatype *IntakeResponse.*

![](media/293019b3d8123374b787d92d4c9305ae.png)

Het handboek definieert een aantal berichten als antwoord op een innameverzoek.
In de SOAP webservice definities mag elk *request* slechts een *response*
hebben. Daarom is het element *responseType* toegevoegd, om de betekenis van de
*response* te duiden. In dit geval heeft het element *responseType* de vaste
waarde *completion*.

De waarde van de elementen *requestReference* en *objectIdAccountableParty*
wordt overgenomen uit het request c.q. het *sourceDocument* in het *request*. De
waarde van de overige elementen wordt toegekend door de webservice. Het element
*broId* bevat de identificatie van het registratieobject in de BRO.

Zie paragraaf 8.15 voor nadere details.

Berichten bij registratie aanvullen en beëindigen
-------------------------------------------------

Bij een *register* operatie zijn drie berichten van toepassing: een
registratieverzoek, een bericht van afwijzing en een bericht van registratie.
Deze paragraaf beschrijft de inhoud van deze berichten bij de gebeurtenissen
‘registratie aanvullen’ en ‘registratie beëindigen’.

### Request: registratieverzoek

Onderstaande figuur geeft de mapping weer van het registratieverzoek in het
innamehandboek op het datatype *RegistrationRequest* in dit document (zie
paragraaf 6.1), zoals gebruikt door de *register* operatie (zie hoofdstuk 5).

![](media/ab84ece27abaf1425dc6c5cb94ed1ac3.png)

Het element brondocumenttype in het registratieverzoek komt niet voor in het
*RegistrationRequest*, omdat dit gegeven impliciet bekend is gegeven de inhoud
van het element *sourceDocument*.

Het element *broId* bevat de identificatie van het registratieobject in de BRO
dat moet worden aangevuld of beëindigd. Het element *sourceDocument* bevat de
aanvullende putgegevens c.q. gegevens met betrekking tot het feit dat de put is
opgeruimd.

### Response: bericht van afwijzing

Het innamehandboek benoemt als mogelijke reactie op een registratieverzoek een
bericht van afwijzing. De webservice gebruikt hiervoor een *response* van het
datatype *IntakeResponse*.

![](media/eabc4d5077cd0123969be461ed78f095.png)

Het handboek definieert een aantal berichten als antwoord op een innameverzoek.
In de SOAP webservice definities mag elk *request* slechts een *response*
hebben. Daarom is het element *responseType* toegevoegd, om de betekenis van de
*response* te duiden. In dit geval heeft het element *responseType* de vaste
waarde *rejection*.

De waarde van de elementen *requestReference* en *broId* wordt overgenomen uit
het *request*. De waarde van de overige elementen wordt toegekend door de
webservice. Het element *rejectionReason* bevat een waarde uit de tabel met
gebruiksfouten; zie het innamehandboek.

Als deze *response* wordt gegeven omdat er een of meer gebruiksfouten in het
*sourceDocument* zijn geconstateerd, dan is de waarde van *rejectionReason* “er
zijn 1 of meer fouten geconstateerd in het brondocument” en volgen er na dit
element een of meer *sourceDocumentErrors*.

Zie paragraaf 8.15 voor nadere details.

### Response: bericht van registratie

Het innamehandboek benoemt als mogelijke reactie op een registratieverzoek een
bericht van registratie. De webservice gebruikt hiervoor een *response* van het
datatype *IntakeResponse.*

![](media/8ba7493ad87e191eceb4115a03987c2b.png)

Het handboek definieert een aantal berichten als antwoord op een innameverzoek.
In de SOAP webservice definities mag elk *request* slechts een *response*
hebben. Daarom is het element *responseType* toegevoegd, om de betekenis van de
*response* te duiden. In dit geval heeft het element *responseType* de vaste
waarde *completion*.

De waarde van de elementen *requestReference* en *broId* wordt overgenomen uit
het *request*.

Zie paragraaf 8.15 voor nadere details.

Berichten bij correctie
-----------------------

Bij correctie operaties (de operaties *replace*, *insert*, *move* en *delete*)
zijn drie berichten van toepassing: een correctieverzoek, een bericht van
afwijzing en een bericht van acceptatie.

### Request: correctieverzoek

Onderstaande figuur geeft de mapping weer van het correctieverzoek in het
innamehandboek op het datatype *CorrectionRequest* in dit document (zie
paragraaf 6.2), zoals gebruikt door de *replace*, *insert* en *delete* operaties
(zie hoofdstuk 5).

![](media/a618bd5678df9cf73727b3cbfbbb74f9.png)

Het element brondocumenttype in het correctieverzoek komt niet voor in het
*correctionRequest*, omdat dit gegeven impliciet bekend is gegeven de inhoud van
het element *sourceDocument*.

Het elementen correctietype in het correctieverzoek komt niet voor in het
*correctionRequest*, omdat dit gegeven impliciet bekend is binnen de context van
de operatie waarmee het *correctionRequest* wordt aangeboden.

Het element *broId* bevat de identificatie van het te corrigeren
registratieobject.

Het element *dateToBeCorrected* komt alleen voor als het *correctionRequest*
wordt gebruikt in een *move* operatie. Dit element bevat de (mogelijkerwijs
onvolledige) datum van de momenteel geregistreerde gebeurtenis die verbeterd
moet worden.

Het element *sourceDocument* bevat dezelfde gegevens als het *sourceDocument*
van het dienovereenkomstige te corrigeren registratieverzoek maar nu met de
correcte waarden.

### Response: bericht van afwijzing

Het innamehandboek benoemt als mogelijke reactie op een registratieverzoek een
bericht van afwijzing. De webservice gebruikt hiervoor een *response* van het
datatype *IntakeResponse*.

![](media/eabc4d5077cd0123969be461ed78f095.png)

Het handboek definieert een aantal berichten als antwoord op een innameverzoek.
In de SOAP webservice definities mag elk *request* slechts een *response*
hebben. Daarom is het element *responseType* toegevoegd, om de betekenis van de
*response* te duiden. In dit geval heeft het element *responseType* de vaste
waarde *rejection*.

De waarde van de elementen *requestReference* en *broId* wordt overgenomen uit
het *request*. De waarde van de overige elementen wordt toegekend door de
webservice. Het element *rejectionReason* bevat een waarde uit de tabel met
gebruiksfouten; zie het innamehandboek.

Als deze *response* wordt gegeven omdat er een of meer gebruiksfouten in het
*sourceDocument* zijn geconstateerd, dan is de waarde van *rejectionReason* “er
zijn 1 of meer fouten geconstateerd in het brondocument” en volgen er na dit
element een of meer *sourceDocumentErrors*.

Zie paragraaf 8.15 voor nadere details.

### Response: bericht van acceptatie

Het innamehandboek benoemt als mogelijke reactie op een correctieverzoek een
bericht van acceptatie. De webservice gebruikt hiervoor een *response* van het
datatype *IntakeResponse*.

![](media/86960a586f005c9ed04b47c75283050d.png)

Het handboek definieert een aantal berichten als antwoord op een innameverzoek.
In de SOAP webservice definities mag elk *request* slechts een *response*
hebben. Daarom is het element *responseType* toegevoegd, om de betekenis van de
*response* te duiden. In dit geval heeft het element *responseType* de vaste
waarde *acceptance*.

De waarde van de elementen *requestReference* en *broId* wordt overgenomen uit
het *request*. De waarde van de overige elementen wordt toegekend door de
webservice. In *acceptanceTime* staat het (datum en) tijdstip waarop het
correctieverzoek is aangenomen.

Zie paragraaf 8.15 voor nadere details.

Berichten bij technische fouten
-------------------------------

Er zijn twee soorten berichten mogelijk bij een technische fout: een
softwarefout of een systeemfout. In de volgende paragrafen wordt dit toegelicht.

### Softwarefout

Als bij de technische controle van het *request* fouten in het verzoek en/of het
brondocument worden gevonden (bijvoorbeeld het *request* is niet een welgevormd
XML bericht of het *request* voldoet niet aan de schemavalidatie), dan worden
deze beschouwd als een softwarefout in het systeem van de dataleverancier. Het
BRO-systeem stuurt dan een melding in de vorm van een *parseFault*. Zie
paragraaf 8.16 voor nadere details.

![](media/d33439738863ed795352c0a0dc300aa5.png)

### Systeemfouten

Tijdens de uitvoering van een operatie kan er een onverwachte fout optreden in
het BRO-systeem. Hiervoor kunnen verschillende oorzaken zijn, zoals het falen
van bepaalde software of hardware. Deze onverwachte fouten worden beschouwd als
een systeemfout in het BRO-systeem. De BRO stuurt dan een bericht in de vorm van
een generieke, niet gemodelleerde *SOAP:Fault*. Zie paragraaf 8.24 voor nadere
details.

Modellering van het interface
=============================

Dit hoofdstuk en de volgende hoofdstukken beschrijven in detail de interface van
de GMW innamewebservice aan de hand van een UML-model.

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
innamewebservice. De packages *dsgmw* en *dsgmw-messages* worden buiten
beschouwing gelaten, aangezien deze de uitgiftewebservice betreffen.

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

Het stereotype *DataType* wordt in UML gebruikt om aan te geven dat een datatype
een niet-identificeerbaar, gestructureerd data type is. In de XSD leidt dit tot
een *complexType* zonder een *gml:id* attribuut.

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

Package isgmw – de innamewebservice interface
=============================================

De onderstaande figuur geeft het interface van de GMW innamewebservice weer:

![](media/27b22944ae1d8d2c01ff8a0d3d2af60c.emf)

Onderstaande tabel bevat een samenvatting van operaties met bijbehorende naam en
datatype van het request:

| Operatie | Request naam        | Request Datatype    |
|----------|---------------------|---------------------|
| Register | registrationRequest | RegistrationRequest |
| Replace  | replaceRequest      | CorrectionRequest   |
| Insert   | insertRequest       | CorrectionRequest   |
| Move     | moveRequest         | MoveRequest         |
| Delete   | deleteRequest       | CorrectionRequest   |

Zie paragraaf 6.1 voor het datatype *RegistrationRequest*, paragraaf 6.2 voor
het datatype *CorrectionRequest* en paragraaf 6.3 voor het datatype
*MoveRequest* uit de package *isgmw-messages*.

Alle operaties gebruiken de generieke response *IntakeResponse* uit de package
*brocommon* voor de functionele antwoordberichten. Zie paragraaf 3.7 voor de
afhandeling van technische fouten.

De WSDL 
--------

De GMW innamewebservice wordt technisch volledig beschreven door de WSDL van de
GMW innamewebservice (*isgmw.wsdl)*. De onderdelen van dit bestand worden
hieronder kort toegelicht.

### Types

Het onderdeel *types* in een WSDL definieert een XML-schema met daarbinnen
XML-types en XML-elementen. Voor de GMW innamewebservice zijn deze opgenomen in
een afzonderlijke berichten XSD (*isgmw-messages.xsd*) die in het *types*
element wordt geïmporteerd.

### Message

Het onderdeel *message* in een WSDL specificeert de berichten die per operatie
worden uitgewisseld, uitgedrukt in parts. In de parts worden XML-elementen uit
het types onderdeel van de WSDL gebruikt. Voor elke operatie wordt een *request*
message en een *response* message gespecificeerd.

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
worden in de WSDL voor de GMW innamewebservice. In alle XSD-bestanden van de BRO
wordt, conform de NEN3610 voorschriften, gebruik gemaakt van verschillende
XSD-bestanden van de internationale W3C en OGC-standaarden.

Deze schema’s worden in de navolgende hoofdstukken beschreven, elk schema in een
eigen hoofdstuk. De opbouw van een element of type uit een schema wordt
afgebeeld in een diagram en waar relevant worden bijzonderheden in de tekst
toegelicht. Voor de inhoudelijke betekenis van de afzonderlijke gegevens wordt
verwezen naar het innamehandboek en de catalogus van de GMW.

De XSD-bestanden zijn opgesteld in het Engels. De vertaling naar Nederlandse
termen die gebruikt worden in het innamehandboek en in de catalogus staat in
Bijlage A (zie paragraaf 11.1).

Package isgmw-messages – de berichten XSD
=========================================

De package isgmw-messages bevat de *requests* en brondocumenten voor de
registratieverzoeken en de correctieverzoeken.

RegistrationRequest
-------------------

Het *RegistrationRequest* in de GMW namespace is een specialisatie van de
abstract klasse *RegistrationRequest*, uit de package *brocommon*, waar het een
*sourceDocument* aan toevoegt.

![](media/26f0e75d2a68234e992449a5ba2bd212.emf)

*SourceDocument* heeft het stereotype *Union* (zie paragraaf 4.2.6), waarmee
wordt aangegeven dat het brondocument polymorf is en dat bij een gegeven request
een van de alternatieve datatypes gekozen moet worden.

In de XSD is dit gerealiseerd als een *choice* uit een lijst van paarsgewijs de
naam van het element en het bijbehorende datatype, zoals aangegeven in
bovenstaande figuur. Deze alternatieven worden toegelicht in de volgende
paragrafen. Merk op dat de naam van het alternatief opgenomen moet worden in het
element *sourceDocument*; daarmee wordt bij een gegeven *request* eenduidig
bekend welk alternatief gekozen is, voordat de feitelijke elementen van dat
alternatief aan bod komen. Voorbeeld:

| \<isgmw:registratonRequest xmlns:isgmw=*"http://www.broservices.nl/xsd/isgmw/1.0"* xmlns:gmwcommon=*"http://www.broservices.nl/xsd/gmwcommon/1.0"* xmlns:brocommon=*"http://www.broservices.nl/xsd/brocommon/3.0"* xmlns:gml=*"http://www.opengis.net/gml/3.2"* xmlns:xsi=*"http://www.w3.org/2001/XMLSchema-instance"* xsi:schemaLocation=*"http://www.broservices.nl/xsd/isgmw/1.0 http://www.broservices.nl/xsd/isgmw/1.0/isgmw-messages.xsd"*\> \<brocommon:requestReference\>levering1-object12\</brocommon:requestReference\> ... \<isgmw:sourceDocument\> \<isgmw:GMW\_Construction\> \<isgmw:objectIdAccountableParty\>object12\</isgmw:objectIdAccountableParty\> ... \</isgmw:GMW\_Construction\> \</isgmw:sourceDocument\> \</isgmw:registrationRequest\> |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


CorrectionRequest 
------------------

Het *CorrectionRequest* in de GMW namespace is een specialisatie van de abstract
klasse *CorrectionRequest* uit de package *brocommon*, waar het
*correctionReason* en een *sourceDocument* aan toevoegt.

![](media/7c5f509ca0826f60b2ed4f093e526f20.emf)

*SourceDocument* heeft het stereotype *Union* (zie ook paragraaf 4.2.6), waarmee
wordt aangegeven dat het brondocument polymorf is en dat bij een gegeven
*request* een van de alternatieve datatypes gekozen moet worden.

MoveRequest
-----------

Het *MoveRequest* is een specialisatie van *CorrectionRequest* uit de GMW
namespace, waar het een *dateToBeCorrected* aan toevoegt. De betekenis van
*dateToBeCorrected* is de (mogelijkerwijs onvolledige) datum gebeurtenis van de
oorspronkelijk geregistreerde gegevens die verbeterd moet worden. De juiste
datum is opgenomen in het *sourceDocument*.

![](media/aceb94cb46d09d8d919fb51793efb4d8.emf)

CorrectionReason
----------------

Het datatype *CorrectionReason* definieert het domein voor het element
*correctionReason*.

![](media/95093e8a95d40df0fb8e38f617e72e46.emf)

Het datatype *CorrectionReason* heeft het stereotype *CodeList* (zie paragraaf
4.2.1).

SourceDocument
--------------

Het datatype *SourceDocument* biedt een keuze uit een reeks alternatieve
brondocumenten datatypes.

![](media/aec5af704a086fa2afb963841f746c32.emf)

*SourceDocument* heeft het stereotype *Union* (zie paragraaf 4.2.6), waarmee
wordt aangegeven dat *SourceDocument* polymorf is en dat in een gegeven XML
bericht een van de alternatieve datatypes gebruikt is.

Niet elk type *sourceDocument* mag gebruikt worden in elke operatie.
Onderstaande tabel geeft weer in welke operatie welke type *sourceDocument*
opgenomen mag worden.

| sourceDocument         | register | replace | insert | move | delete |
|------------------------|----------|---------|--------|------|--------|
| GMW\_Construction      | X        | X       |        | X    |        |
| GMW\_Owner             | X        | X       | X      | X    | X      |
| GMW\_Lengthening       | X        | X       | X      | X    | X      |
| GMW\_GroundLevel       | X        | X       | X      | X    | X      |
| GMW\_Shortening        | X        | X       | X      | X    | X      |
| GMW\_Positions         | X        | X       | X      | X    | X      |
| GMW\_ElectrodeStatus   | X        | X       | X      | X    | X      |
| GMW\_Maintainer        | X        | X       | X      | X    | X      |
| GMW\_TubeStatus        | X        | X       | X      | X    | X      |
| GMW\_Insertion         | X        | X       | X      | X    | X      |
| GMW\_Shift             | X        | X       | X      | X    | X      |
| GMW\_Removal           | X        |         |        | X    | X      |
| GMW\_WellHeadProtector | X        | X       | X      | X    | X      |

Bovenstaande regel wordt niet afgedwongen door de XSD, maar softwarematig
gecontroleerd. Een *request* dat niet voldoet aan deze regels wordt gezien als
een gebruiksfout (zie paragraaf 3.4.2, 3.5.2 of paragraaf 3.6.2).

NB: Met *GMW\_Construction* wordt de initiële inrichting van een put
geregistreerd (*register* operatie), gecorrigeerd (*replace* operatie) of
verplaatst in de tijdlijn (*move* operatie). Met *GMW\_Removal* wordt de put
opgeruimd (*register* operatie), de opruiming verplaatst in de tijdlijn (*move*
operatie) of verwijderd uit de tijdlijn (*delete* operatie). Met de overige
brondocumenten wordt een aanvullingen geregistreerd (*register* operatie),
gecorrigeerd (*replace* operatie), toegevoegd in de tijdlijn (*insert*
operatie), verplaatst in de tijdlijn (*move* operatie) of verwijderd uit de
tijdlijn (*delete* operatie).

### GMW\_Construction

De variant *GMW\_Construction* van het element *sourceDocument* is van het
datatype *GroundwaterMonitoringWell*.

![](media/8c926d9b8fbabada2310759f169c0163.emf)

De elementen *NITGCode* en *mapSheetCode* zijn beiden optioneel, maar er moet
altijd een van beiden aanwezig zijn en een waarde hebben. Het element *NITGCode*
is alleen aanwezig wanneer de put geregistreerd was in de registratie DINO,
anders is het element *mapSheetCode* aanwezig.

De datatypes *DeliveredLocation* en *DeliveredVerticalPosition* zijn
gemodelleerd in de package *gmwcommon*, omdat zij veel overlap vertonen tussen
de innameservice en de uitgifteservice. De datatypes *GroundwaterMonitoringWell*
en *MonitoringTube* zijn gemodelleerd in de package *isgmw-messages*, omdat zij
(of een van hun kinderen) een andere structuur hebben dan de tegenhanger in de
uitgifteservice.

Enkele elementen hebben het GML-stereotype *Voidable*; zie paragraaf 4.2.7 voor
nadere uitleg.

### GMW\_ElectrodeStatus

Met de variant *GMW\_ElectrodeStatus* van het element *sourceDocument* kan de
verandering in de fysieke status van een of meer elektrodes van een reeds
geregistreerde put worden geregistreerd.

![](media/80720c604c698ee466bdd250cfcda1a9.emf)

### GMW\_GroundLevel

Met de variant *GMW\_GroundLevel* van het element *sourceDocument* kan een
nieuwe maaiveldpositie van een reeds geregistreerde put worden toegevoegd.

![](media/94844e8bdc0c4e547a74433f5d1440e5.emf)

### GMW\_Insertion

Met de variant *GMW\_Insertion* van het element *sourceDocument* kan het
repareren van een monitoringbuis, door het plaatsen van een stijgbuisdeel met
een kleinere diameter binnen een bestaande buis, van een reeds geregistreerde
put worden geregistreerd.

![](media/8a8083009b01a2b7949a2db6f6264fce.emf)

### GMW\_Lengthening

Met de variant *GMW\_Lengthening* van het element *sourceDocument* kan de
oplenging van het stijgbuisdeel van een of meer monitoringbuizen van een reeds
geregistreerde grondwatermonitoringput worden geregistreerd.

![](media/77b4ddebb2737c17b2eb45e903ba4a73.emf)

### GMW\_Maintainer

Met de variant *GMW\_Maintainer* van het element *sourceDocument* kan een nieuwe
onderhoudende instantie van een reeds geregistreerde put worden toegevoegd.

![](media/34125d767a26d2a7c0c66ea436e0ab78.emf)

### GMW\_Owner

Met de variant *GMW\_Owner* van het element *sourceDocument* kan een nieuwe
eigenaar worden toegevoegd aan een reeds geregistreerde put.

![](media/d4b6b68a6eadeea9466a507d2c64c6f7.emf)

### GMW\_Positions

Met de variant *GMW\_Positions* van het element *sourceDocument* kunnen een
nieuwe maaiveldpositie en de posities van een of meer monitoringbuizen van een
reeds geregistreerde put worden geregistreerd.

![](media/0082156b83ca4c8099ef7bd8d4b0f3d4.emf)

### GMW\_Removal

Met de variant *GMW\_Removal* van het element *sourceDocument* kan het opruimen
van een reeds geregistreerde put worden geregistreerd.

![](media/37b4f3e6e29d198b768e846964c29a0b.emf)

### GMW\_Shift

Met de variant *GMW\_Shift* van het element *sourceDocument* kan het verleggen
van het maaiveld bij een put door ophoging of afgraving van een reeds
geregistreerde put worden geregistreerd.

![](media/c7e36ba266ac18e8a108a4647f5a2146.emf)

### GMW\_Shortening

Met de variant *GMW\_Shortening* van het element *sourceDocument* kan het
inkorten van het stijgbuisdeel van een of meer monitoringbuizen van een reeds
geregistreerde put worden geregistreerd.

![](media/962c3d5cae0fb5cf493b46cee1d25f3d.emf)

### GMW\_TubeStatus

Met de variant *GMW\_TubeStatus* van het element *sourceDocument* kan de
verandering in de (fysieke) status van een of meer monitoringbuizen van een
reeds geregistreerde put worden geregistreerd.

![](media/974392008c088c2377e7bca5bbbd4306.emf)

### GMW\_WellHeadProtector

Met de variant *GMW\_WellHeadProtector* van het element *sourceDocument* kan het
plaatsen van een nieuwe beschermconstructie van een reeds geregistreerde put
worden geregistreerd.

![](media/7d0b4409be1c2847432187a223e887a9.emf)

### GeoOhmCable

Het datatype *GeoOhmCable* bevat de gegevens over een geo-ohmkabel bevestigd aan
een buis en voorzien van elektroden, die gebruikt wordt om bijvoorbeeld het
zoutgehalte van het water te kunnen bepalen.

![](media/406937907bded424fa82c1df60a3b767.emf)

Aan een buis kunnen meerdere geo-ohmkabels bevestigd zijn; het element
*cableNumber* geeft per buis iedere kabel een unieke aanduiding.

Een geo-ohmkabel is voorzien van twee of meer elektrodes. Het datatype
*Electrode* is gemodelleerd in de package *gmwcommon*, omdat zij veel overlap
vertoont tussen de innameservice en de uitgifteservice.

### MonitoringTube

Het datatype *MonitoringTube* bevat alle gegevens over een buis die is
aangebracht om het grondwater uit een specifiek deel van de ondergrond te
ontsluiten.

![](media/935f844a62d72c766f77e874f971d0de.emf)

De datatypes *MaterialUsed*, *PlainTubePart* en *SedimentSump* zijn gemodelleerd
in de package *gmwcommon*, omdat zij veel overlap vertonen tussen de
innameservice en de uitgifteservice. De datatypes *Screen* en *GeoOhmCable* zijn
gemodelleerd in de package *isgmw-messages*, omdat zij (of een van hun kinderen)
een andere structuur hebben dan de tegenhanger in de uitgifteservice.

Enkele elementen hebben het GML-stereotype *Voidable*; zie paragraaf 4.2.7 voor
nadere uitleg.

### Screen

Het datatype *Screen* bevat alle gegevens over het filter van een buis, namelijk
dat deel van de monitoringbuis dat voorzien is van openingen waardoor het
grondwater kan binnenstromen.

![](media/b01ef11c2cb969f8f133de0fb824acc6.emf)

Package gmwcommon
=================

De package *gmwcommon* bevat de entiteiten en relaties, die gemeenschappelijk
zijn voor zowel de GMW innamewebservice als de GMW uitgiftewebservice.

Codelijsten
-----------

De catalogus maakt een onderscheid in beheerde en niet-beheerde enumeraties. Het
stereotype *CodeList* wordt in UML gebruikt om aan te geven dat een datatype een
beheerde enumeratie is (zie paragraaf 4.2.1).

De package *gmwcommon* bevat een aantal codelijsten. Zie paragraaf 11.1.4 voor
een overzicht. Voorbeeld:

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
attributen gespecificeerd met getalswaarde.

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
daarom een stereotype *CodeList* (zie paragraaf 4.2.1). De waarde geeft aan
welke transformatiemethode is toegepast. Merk op dat de toegestane waarde anders
kan zijn voor IMBRO dan voor IMBRO/A.

![](media/d714d9e061e53e4c7e95864ebac33cfd.emf)

CorrectionRequest
-----------------

Het datatype *CorrectionRequest* bevat de gemeenschappelijke gegevens voor het
samenstellen van een request om de gegevens voor een bepaald registratieobject
te corrigeren.

![](media/e7dc4dda0747c0ad7d2ac437541ed948.emf)

Het element *requestReference* is een voor de dataleverancier unieke aanduiding
van het request.

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
alleen uitgegeven als de data-afnemer tevens bronhouder en/of dataleverancier is
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

Het element *requestReference* is een voor de dataleverancier unieke aanduiding
van het *request*.

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

Het datatype *RegistrationStatus* is een beheerde enumeratie en het heeft daarom
een stereotype *CodeList* (zie paragraaf 4.2.1). Zie de *catalogus* voor het
domein en de betekenis van de waarden.

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
verzoek niet is verwerkt. Deze fouten kunnen niet door de dataleverancier worden
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

| \<complexType name=*"DeliveryContext"*\> \<simpleContent\> \<restriction base=*"gml:CodeWithAuthorityType"*\> \<attribute name=*"codeSpace"* type=*"anyURI"* use=*"required"* fixed=*"urn:bro:gmw:DeliveryContext"*/\> \</restriction\> \</simpleContent\> \</complexType\> |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


Voorbeeld van een element, met als datatype een codelijst, in een XML bericht.
Zo’n element heeft een attribuut *codeSpace*, waarvan de waarde aangeeft in
welke tabel de toegestane waarden zijn vastgelegd, en als waarde een van de
waarden uit die tabel. Voorbeeld:

| \<deliveryContext codeSpace=*"urn:bro:gmw:DeliveryContext"*\>publiekeTaak\</deliveryContext\> |
|-----------------------------------------------------------------------------------------------|


Merk op dat in de catalogus en in het UML-diagram het domein expliciet wordt
benoemd. Het domein is niet opgenomen in het XSD-bestand. Als dat wel het geval
zou zijn, dan zou een wijziging in het domein leiden tot een wijziging van het
XSD-bestand. Het domein wordt niet afgedwongen door het XSD-bestand. In plaats
daarvan valideert het BRO-systeem de gebruikte waarde softwarematig via een
database tabel.

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

### A1: isgmw-messages

| Engels                       | Nederlands                             |
|------------------------------|----------------------------------------|
| CorrectionRequest            | Correctieverzoek                       |
| broId                        | BRO-ID                                 |
| correctionReason             | Correctie reden                        |
| deliveryAccountableParty     | Bronhouder                             |
| qualityRegime                | Kwaliteitsregime                       |
| requestReference             | Verzoekkenmerk                         |
| sourceDocument               | Brondocument                           |
| Underprivilege               | Onder voorrecht                        |
| Electrode                    | Elektrode                              |
| cableNumber                  | Kabelnummer                            |
| electrodeNumber              | Elektrodenummer                        |
| electrodeStatus              | Elektrodestatus                        |
| tubeNumber                   | Buisnummer                             |
| GeoOhmCable                  | Geo-ohmkabel                           |
| cableNumber                  | Kabelnummer                            |
| GMW\_Construction            | GMW-Inrichten                          |
| ConstructionStandard         | Kwaliteitsnorm inrichting              |
| DeliveredLocation            | Aangeleverde locatie                   |
| DeliveredVerticalPosition    | Aangeleverde verticale positie         |
| DeliveryContext              | Kader aanlevering                      |
| GroundLevelStable            | Maaiveld stabiel                       |
| GroundwaterMonitoringWell    | Grondwatermonitoringput                |
| InitialFunction              | Initiële functie                       |
| MaintenanceResponsibleParty  | Onderhoudende instantie                |
| MapSheetCode                 | Kaartbladnummer                        |
| MonitoringTube               | Monitoringbuis                         |
| NITGCode                     | NITG-code                              |
| NumberOfMonitoringTubes      | Aantal monitoringbuizen                |
| ObjectIdAccountableParty     | Object-ID bronhouder                   |
| Owner                        | Eigenaar                               |
| WellConstructionDate         | Inrichtingsdatum put                   |
| WellHeadProtector            | Beschermconstructie                    |
| WellStability                | Putstabiliteit                         |
| GMW\_ElectrodeStatus         | GMW-Elektrodestatus                    |
| Electrode                    | Elektrode                              |
| eventDate                    | Datum gebeurtenis                      |
| numberOfElectrodesChanged    | Aantal veranderde elektrodes           |
| GMW\_GroundLevel             | GMW-Maaiveldpositie                    |
| eventDate                    | Datum gebeurtenis                      |
| groundLevelPosition          | Maaiveldpositie                        |
| groundLevelPositioningMethod | Methode positiebepaling maaiveld       |
| groundLevelStable            | Maaiveld stabiel                       |
| wellStability                | Putstabiliteit                         |
| GMW\_Insertion               | GMW-Inplaatsen                         |
| eventDate                    | Datum gebeurtenis                      |
| insertedPartDiameter         | Diameter bovenkant ingeplaatst deel    |
| insertedPartLength           | Lengte ingeplaatst deel                |
| insertedPartMaterial         | Materiaal ingeplaatst deel             |
| tubeNumber                   | Buisnummer                             |
| tubeTopPosition              | Positie bovenkant buis                 |
| tubeTopPositioningMethod     | Methode positiebepaling bovenkant buis |
| GMW\_Lengthening             | GMW-Oplengen                           |
| eventDate                    | Datum gebeurtenis                      |
| monitoringTube               | Monitoringbuis                         |
| numberOfTubesLengthened      | Aantal opgelengde buizen               |
| wellHeadProtector            | Beschermconstructie                    |
| GMW\_Maintainer              | GMW-Onderhouder                        |
| eventDate                    | Datum gebeurtenis                      |
| maintenanceResponsibleParty  | Onderhoudende instantie                |
| GMW\_Owner                   | GMW-Eigenaar                           |
| eventDate                    | Datum gebeurtenis                      |
| owner                        | Eigenaar                               |
| GMW\_Positions               | GMW-Posities                           |
| eventDate                    | Datum gebeurtenis                      |
| groundLevelPosition          | Maaiveldpositie                        |
| groundLevelPositioningMethod | Methode positiebepaling maaiveld       |
| groundLevelStable            | Maaiveld stabiel                       |
| numberOfMonitoringTubes      | Aantal monitoringbuizen                |
| wellStability                | Putstabiliteit                         |
| GMW\_Removal                 | GMW-Opruimen                           |
| wellRemovalDate              | Opruimingsdatum                        |
| GMW\_Shift                   | GMW-Verleggen                          |
| eventDate                    | Datum gebeurtenis                      |
| groundLevelPosition          | Maaiveldpositie                        |
| groundLevelPositioningMethod | Methode positiebepaling maaiveld       |
| GMW\_Shortening              | GMW-Inkorten                           |
| eventDate                    | Datum gebeurtenis                      |
| numberOfTubesShortened       | Aantal ingekorte buizen                |
| wellHeadProtector            | Beschermconstructie                    |
| GMW\_TubeStatus              | GMW-Buisstatus                         |
| eventDate                    | Datum gebeurtenis                      |
| numberOfTubesChanged         | Aantal veranderde buizen               |
| GMW\_WellHeadProtector       | GMW-Beschermconstructie                |
| eventDate                    | Datum gebeurtenis                      |
| wellHeadProtector            | Beschermconstructie                    |
| MonitoringTube               |                                        |
| artesianWellCapPresent       | Voorzien van drukdop                   |
| sedimentSumpPresent          | Voorzien van zandvang                  |
| numberOfGeoOhmCables         | Aantal geo-ohmkabels                   |
| tubeNumber                   | Buisnummer                             |
| tubeTopDiameter              | Diameter bovenkant buis                |
| tubeTopPosition              | Positie bovenkant buis                 |
| tubeTopPositioningMethod     | Methode positiebepaling bovenkant buis |
| tubeStatus                   | Buisstatus                             |
| tubeType                     | Buistype                               |
| variableDiameter             | Variabele diameter                     |
| MonitoringTubeLengthening    |                                        |
| glue                         | Lijm                                   |
| plainTubePartLength          | Stijgbuisdeellengte                    |
| tubeMaterial                 | Buismateriaal                          |
| tubeNumber                   | Buisnummer                             |
| tubeTopDiameter              | Diameter bovenkant buis                |
| tubeTopPosition              | Positie bovenkant buis                 |
| tubeTopPositioningMethod     | Methode positiebepaling bovenkant buis |
| variableDiameter             | Variabele diameter                     |
| MonitoringTubePosition       |                                        |
| tubeNumber                   | Buisnummer                             |
| tubeTopPosition              | Positie bovenkant buis                 |
| tubeTopPositioningMethod     | Methode positiebepaling bovenkant buis |
| MonitoringTubeShortened      |                                        |
| plainTubePartLength          | Stijgbuisdeellengte                    |
| tubeNumber                   | Buisnummer                             |
| tubeTopPosition              | Positie bovenkant buis                 |
| tubeTopPositioningMethod     | Methode positiebepaling bovenkant buis |
| MonitoringTubeStatus         |                                        |
| tubeNumber                   | Buisnummer                             |
| tubeStatus                   | Buisstatus                             |
| MoveRequest                  | Verplaatsingsverzoek                   |
| broId                        | BRO-ID                                 |
| correctionReason             | Correctie reden                        |
| dateToBeCorrected            | Te corrigeren datum                    |
| deliveryAccountableParty     | Bronhouder                             |
| qualityRegime                | Kwaliteitsregime                       |
| requestReference             | Verzoekkenmerk                         |
| sourceDocument               | Brondocument                           |
| Underprivilege               | Onder voorrecht                        |
| RegistrationRequest          | Registratieverzoek                     |
| broId                        | BRO-ID                                 |
| deliveryAccountableParty     | Bronhouder                             |
| qualityRegime                | Kwaliteitsregime                       |
| requestReference             | Verzoekkenmerk                         |
| sourceDocument               | Brondocument                           |
| underprivilege               | Onder voorrecht                        |
| Screen                       | Filter                                 |
| screenLength                 | Filterlengte                           |
| sockMaterial                 | Kousmateriaal                          |
| SourceDocument               | Brondocument                           |
| GMW\_Construction            | GMW-Inrichten                          |
| GMW\_ElectrodeStatus         | GMW-Elektrodestatus                    |
| GMW\_GroundLevel             | GMW-Maaiveldpositie                    |
| GMW\_Insertion               | GMW-Inplaatsen                         |
| GMW\_Lengthening             | GMW-Oplengen                           |
| GMW\_Maintainer              | GMW-Onderhouder                        |
| GMW\_Owner                   | GMW-Eigenaar                           |
| GMW\_Positions               | GMW-Posities                           |
| GMW\_Removal                 | GMW-Opruimen                           |
| GMW\_Shift                   | GMW-Verleggen                          |
| GMW\_Shortening              | GMW-Inkorten                           |
| GMW\_TubeStatus              | GMW-Buisstatus                         |
| GMW\_WellHeadProtector       | GMW-Beschermconstructie                |

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
berichten kunt u vinden op www.broinfo.nl.

### RegistrationRequest – start registratie

Met onderstaande voorbeeldbericht *RegistrationRequest* in een *register*
operatie wordt een put geregistreerd, inclusief 2 buisdelen. De put is sinds 4
november 2014 in eigendom van het bedrijf met KvK nummer 52766111.

| \<isgmw:registrationRequest xmlns:isgmw=*"http://www.broservices.nl/xsd/isgmw/1.0"* xmlns:brocommon=*"http://www.broservices.nl/xsd/brocommon/3.0"* xmlns:gml=*"http://www.opengis.net/gml/3.2"* xmlns:gmwcommon=*"http://www.broservices.nl/xsd/gmwcommon/1.0"* xmlns:xsi=*"http://www.w3.org/2001/XMLSchema-instance"* xsi:schemaLocation=*"http://www.broservices.nl/xsd/isgmw/1.0 http://www.broservices.nl/xsd/isgmw/1.0/isgmw-messages.xsd"*\> \<brocommon:requestReference\>levering1-20150728\</brocommon:requestReference\> \<brocommon:qualityRegime\>IMBRO/A\</brocommon:qualityRegime\> \<isgmw:sourceDocument\> \<isgmw:GMW\_Construction\> \<isgmw:objectIdAccountableParty\>B07F0076\</isgmw:objectIdAccountableParty\> \<isgmw:deliveryContext codeSpace=*"urn:bro:gmw:DeliveryContext"*\> publiekeTaak \</isgmw:deliveryContext\> \<isgmw:constructionStandard codeSpace=*"urn:bro:gmw:ConstructionStandard"*\> RWSNormenGWMon \</isgmw:constructionStandard\> \<isgmw:initialFunction codeSpace=*"urn:bro:gmw:InitialFunction"*\> stand \</isgmw:initialFunction\> \<isgmw:numberOfMonitoringTubes\>2\</isgmw:numberOfMonitoringTubes\> \<isgmw:groundLevelStable\>nee\</isgmw:groundLevelStable\> \<isgmw:wellStability codeSpace=*"urn:bro:gmw:WellStability"*\> stabielTovNAP \</isgmw:wellStability\> \<isgmw:NITGCode\>B07F0076\</isgmw:NITGCode\> \<isgmw:owner\>52766111\</isgmw:owner\> \<isgmw:maintenanceResponsibleParty\> 27376655 \</isgmw:maintenanceResponsibleParty\> \<isgmw:wellHeadProtector codeSpace=*"urn:bro:gmw:WellHeadProtector"*\> kokerMetaal \</isgmw:wellHeadProtector\> \<isgmw:wellConstructionDate\> \<brocommon:date\>2014-11-04+01:00\</brocommon:date\> \</isgmw:wellConstructionDate\> \<isgmw:deliveredLocation\> \<gmwcommon:location gml:id=*"location0c28e3e4-f74e-4209-b9df-34224b92e0f8"* srsName=*"urn:ogc:def:crs:EPSG::28992"*\> \<gml:pos\>134750 477800\</gml:pos\> \</gmwcommon:location\> \<gmwcommon:horizontalPositioningMethod codeSpace=*"urn:bro:gmw:HorizontalPositioningMethod"*\> RTK\_GPS\_10\_50cm \</gmwcommon:horizontalPositioningMethod\> \</isgmw:deliveredLocation\> \<isgmw:deliveredVerticalPosition\> \<gmwcommon:localVerticalReferencePoint codeSpace=*"urn:bro:gmw:LocalVerticalReferencePoint"*\> NAP \</gmwcommon:localVerticalReferencePoint\> \<gmwcommon:offset uom=*"m"*\>0.000\</gmwcommon:offset\> \<gmwcommon:verticalDatum codeSpace=*"urn:bro:gmw:VerticalDatum"*\> NAP \</gmwcommon:verticalDatum\> \<gmwcommon:groundLevelPosition uom=*"m"*\> -0.98 \</gmwcommon:groundLevelPosition\> \<gmwcommon:groundLevelPositioningMethod codeSpace=*"urn:bro:gmw:GroundLevelPositioningMethod"*\> RTK\_GPS\_20\_100cm \</gmwcommon:groundLevelPositioningMethod\> \</isgmw:deliveredVerticalPosition\> \<isgmw:monitoringTube\> \<isgmw:tubeNumber\>1\</isgmw:tubeNumber\> \<isgmw:tubeType codeSpace=*"urn:bro:gmw:TubeType"*\> *buis* \</isgmw:tubeType\> \<isgmw:artesianWellCapPresent\>ja\</isgmw:artesianWellCapPresent\> \<isgmw:sedimentSumpPresent\>nee\</isgmw:sedimentSumpPresent\> \<isgmw:numberOfGeoOhmCables\>1\</isgmw:numberOfGeoOhmCables\> \<isgmw:tubeTopDiameter uom=*"mm"*\>36\</isgmw:tubeTopDiameter\> \<isgmw:variableDiameter\>nee\</isgmw:variableDiameter\> \<isgmw:tubeStatus codeSpace=*"urn:bro:gmw:TubeStatus"*\> klaarVoorGebruik \</isgmw:tubeStatus\> \<isgmw:tubeTopPosition uom=*"m"*\>-0.98\</isgmw:tubeTopPosition\> \<isgmw:tubeTopPositioningMethod codeSpace=*"urn:bro:gmw:TubeTopPositioningMethod"*\> RTK\_GPS\_20\_100cm \</isgmw:tubeTopPositioningMethod\> \<isgmw:materialUsed\> \<gmwcommon:tubePackingMaterial codeSpace=*"urn:bro:gmw:TubePackingMaterial"*\> *filtergrind* \</gmwcommon:tubePackingMaterial\> \<gmwcommon:tubeMaterial codeSpace=*"urn:bro:gmw:TubeMaterial"*\> *pvc* \</gmwcommon:tubeMaterial\> \<gmwcommon:glue codeSpace=*"urn:bro:gmw:Glue"*\>kit\</gmwcommon:glue\> \</isgmw:materialUsed\> \<isgmw:screen\> \<isgmw:screenLength uom=*"m"*\>0.00\</isgmw:screenLength\> \<isgmw:sockMaterial codeSpace=*"urn:bro:gmw:SockMaterial"*\> *geen* \</isgmw:sockMaterial\> \</isgmw:screen\> \<isgmw:plainTubePart\> \<gmwcommon:plainTubePartLength uom=*"m"*\> 10.000 \</gmwcommon:plainTubePartLength\> \</isgmw:plainTubePart\> \<isgmw:geoOhmCable\> \<isgmw:cableNumber\>1\</isgmw:cableNumber\> \<isgmw:electrode\> \<gmwcommon:electrodeNumber\>1\</gmwcommon:electrodeNumber\> \<gmwcommon:electrodePackingMaterial codeSpace=*"urn:bro:gmw:ElectrodePackingMaterial"*\> *zand* \</gmwcommon:electrodePackingMaterial\> \<gmwcommon:electrodeStatus codeSpace=*"urn:bro:gmw:ElectrodeStatus"*\> *Gebruiksklaar* \</gmwcommon:electrodeStatus\> \<gmwcommon:electrodePosition uom=*"m"*\>-7.000\</gmwcommon:electrodePosition\> \</isgmw:electrode\> \<isgmw:electrode\> \<gmwcommon:electrodeNumber\>2\</gmwcommon:electrodeNumber\> \<gmwcommon:electrodePackingMaterial codeSpace=*"urn:bro:gmw:ElectrodePackingMaterial"*\> *Zand* \</gmwcommon:electrodePackingMaterial\> \<gmwcommon:electrodeStatus codeSpace=*"urn:bro:gmw:ElectrodeStatus"*\> *gebruiksklaar* \</gmwcommon:electrodeStatus\> \<gmwcommon:electrodePosition uom=*"m"*\>-7.500\</gmwcommon:electrodePosition\> \</isgmw:electrode\> \</isgmw:geoOhmCable\> \</isgmw:monitoringTube\> \<isgmw:monitoringTube\> \<isgmw:tubeNumber\>2\</isgmw:tubeNumber\> \<isgmw:tubeType codeSpace=*"urn:bro:gmw:TubeType"*\> *buis* \</isgmw:tubeType\> \<isgmw:artesianWellCapPresent\>ja\</isgmw:artesianWellCapPresent\> \<isgmw:sedimentSumpPresent\>nee\</isgmw:sedimentSumpPresent\> \<isgmw:numberOfGeoOhmCables\>0\</isgmw:numberOfGeoOhmCables\> \<isgmw:tubeTopDiameter uom=*"mm"*\>36\</isgmw:tubeTopDiameter\> \<isgmw:variableDiameter\>nee\</isgmw:variableDiameter\> \<isgmw:tubeStatus codeSpace=*"urn:bro:gmw:TubeStatus"*\> klaarVoorGebruik \</isgmw:tubeStatus\> \<isgmw:tubeTopPosition uom=*"m"*\>-10.98\</isgmw:tubeTopPosition\> \<isgmw:tubeTopPositioningMethod codeSpace=*"urn:bro:gmw:TubeTopPositioningMethod"*\> RTK\_GPS\_20\_100cm \</isgmw:tubeTopPositioningMethod\> \<isgmw:materialUsed\> \<gmwcommon:tubePackingMaterial codeSpace=*"urn:bro:gmw:TubePackingMaterial"*\> *filtergrind* \</gmwcommon:tubePackingMaterial\> \<gmwcommon:tubeMaterial codeSpace=*"urn:bro:gmw:TubeMaterial"*\> *pvc* \</gmwcommon:tubeMaterial\> \<gmwcommon:glue codeSpace=*"urn:bro:gmw:Glue"*\> lijmOngespecificeerd \</gmwcommon:glue\> \</isgmw:materialUsed\> \<isgmw:screen\> \<isgmw:screenLength uom=*"m"*\>2.00\</isgmw:screenLength\> \<isgmw:sockMaterial codeSpace=*"urn:bro:gmw:SockMaterial"*\> *nylon* \</isgmw:sockMaterial\> \</isgmw:screen\> \<isgmw:plainTubePart\> \<gmwcommon:plainTubePartLength uom=*"m"*\> 8.00 \</gmwcommon:plainTubePartLength\> \</isgmw:plainTubePart\> \</isgmw:monitoringTube\> \</isgmw:GMW\_Construction\> \</isgmw:sourceDocument\> \</isgmw:registrationRequest\> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


### RegistrationRequest – aanvullen nieuwe eigenaar

Met onderstaande voorbeeldbericht *RegistrationRequest* in een *register*
operatie wordt een nieuwe huidige eigenaar van een put geregistreerd. Met ingang
van 1 februari 2017 is het bedrijf met KvK nummer 5276613 eigenaar van de put.

| \<isgmw:registrationRequest xmlns:isgmw=*"http://www.broservices.nl/xsd/isgmw/1.0"* xmlns:brocommon=*"http://www.broservices.nl/xsd/brocommon/3.0"* xmlns:gml=*"http://www.opengis.net/gml/3.2"* xmlns:gmwcommon=*"http://www.broservices.nl/xsd/gmwcommon/1.0"* xmlns:xsi=*"http://www.w3.org/2001/XMLSchema-instance"* xsi:schemaLocation=*"http://www.broservices.nl/xsd/isgmw/1.0 http://www.broservices.nl/xsd/isgmw/1.0/isgmw-messages.xsd"*\> \<brocommon:requestReference\>*aanv*-20170201-0001\</brocommon:requestReference\> \<brocommon:deliveryAccountableParty\>27376655\</brocommon:deliveryAccountableParty\> \<brocommon:broId\>GMW000000000001\</brocommon:broId\> \<brocommon:qualityRegime\>IMBRO/A\</brocommon:qualityRegime\> \<isgmw:sourceDocument\> \<isgmw:GMW\_Owner\> \<isgmw:eventDate\> \<brocommon:date\>2017-02-01+01:00\</brocommon:date\> \</isgmw:eventDate\> \<isgmw:owner\>52766133\</isgmw:owner\> \</isgmw:GMW\_Owner\> \</isgmw:sourceDocument\> \</isgmw:registrationRequest\> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


### CorrectionRequest – eigenaar invoegen

Nadat de aanvulling in de voorgaande paragraaf is uitgevoerd, ontdekt de
dataleverancier dat er iets fout is gegaan. Tussen de oorspronkelijke eigenaar
met KvK nummer 52766111 en de huidige eigenaar met KvK nummer 52766133 heeft de
put een andere eigenaar gehad.

Deze tussentijdse eigenaar kan niet met een *RegistrationRequest* worden
aangevuld, maar moet met een *insertRequest* in een *insert* operatie worden
ingevoegd. De naam van het request geeft aan dat het om een invoeging gaat. Merk
op dat de inhoud van het brondocument dezelfde structuur heeft als het
brondocument in het vorige voorbeeldbericht.

Het onderstaande voorbeeldbericht van een correctieverzoek voegt een eigenaar
in, in de periode vóór de huidige eigenaar: vanaf 1 mei 2016 was er een eigenaar
met KvK nummer 52766122.

| \<isgmw:insertRequest xmlns:isgmw=*"http://www.broservices.nl/xsd/isgmw/1.0"* xmlns:brocommon=*"http://www.broservices.nl/xsd/brocommon/3.0"* xmlns:gml=*"http://www.opengis.net/gml/3.2"* xmlns:gmwcommon=*"http://www.broservices.nl/xsd/gmwcommon/1.0"* xmlns:xsi=*"http://www.w3.org/2001/XMLSchema-instance"* xsi:schemaLocation=*"http://www.broservices.nl/xsd/isgmw/1.0 http://www.broservices.nl/xsd/isgmw/1.0/isgmw-messages.xsd"*\> \<brocommon:requestReference\>*corr*-20170214-0001\</brocommon:requestReference\> \<brocommon:deliveryAccountableParty\> 27376655 \</brocommon:deliveryAccountableParty\> \<brocommon:broId\>GMW000000000001\</brocommon:broId\> \<brocommon:qualityRegime\>IMBRO/A\</brocommon:qualityRegime\> \<isgmw:correctionReason codeSpace=*"urn:bro:gmw:CorrectionReason"*\> eigenCorrectie \</isgmw:correctionReason\> \<isgmw:sourceDocument\> \<isgmw:GMW\_Owner\> \<isgmw:eventDate\> \<brocommon:date\>2016-05-01+02:00\</brocommon:date\> \</isgmw:eventDate\> \<isgmw:owner\>52766122\</isgmw:owner\> \</isgmw:GMW\_Owner\> \</isgmw:sourceDocument\> \</isgmw:insertRequest\> |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


### IntakeResponse – bericht van registratie

Voorbeeld van een *response* op een registrationRequest dat het *request* is
verwerkt.

| \<isgmw:intakeResponse xmlns:isgmw=*"http://www.broservices.nl/xsd/isgmw/1.0"* xmlns:brocom=*"http://www.broservices.nl/xsd/brocommon/3.0"* xmlns:xsi=*"http://www.w3.org/2001/XMLSchema-instance"* xsi:schemaLocation=*"http://www.broservices.nl/xsd/isgmw/1.0 http://www.broservices.nl/xsd/isgmw/1.0/isgmw-messages.xsd"*\> \<brocom:responseType\>completion\</brocom:responseType\> \<brocom:requestReference\>*levering1-20150728*\</brocom:requestReference\> \<brocom:transactionId\>GMW-000000042845\</brocom:transactionId\> \<brocom:broId\>GMW000000046027\</brocom:broId\> \<brocom:objectIdAccountableParty\>object-0001\</brocom:objectIdAccountableParty\> \<brocom:completionTime\>2017-06-13T14:48:31+01:00\</brocom:completionTime\> \</isgmw:intakeResponse\> |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


### IntakeResponse – bericht van afwijzing

Voorbeeld van een *response* op een registrationRequest dat het *request* is
verwerkt.

| \<isgmw:intakeResponse xmlns:isgmw=*"http://www.broservices.nl/xsd/isgmw/1.0"* xmlns:brocom=*"http://www.broservices.nl/xsd/brocommon/3.0"* xmlns:xsi=*"http://www.w3.org/2001/XMLSchema-instance"* xsi:schemaLocation=*"http://www.broservices.nl/xsd/isgmw/1.0 http://www.broservices.nl/xsd/isgmw/1.0/isgmw-messages.xsd"*\> \<brocom:responseType\>rejection\</brocom:responseType\> \<brocom:requestReference\>*corr*-20170214-0001\</brocom:requestReference\> \<brocom:transactionId\>GMW-000000042846\</brocom:transactionId\> \<brocom:broId\>GMW000000000001\</brocom:broId\> \<brocom:rejectionTime\>2017-06-13T14:13:21+01:00\</brocom:rejectionTime\> \<brocom:rejectionReason\>*Er zijn* 1 of *meer fouten geconstateerd* in *het brondocument*.\</brocom:rejectionReason\> \<brocom:sourceDocumentError\> \<brocom:sequenceNumber\>1\</brocom:sequenceNumber\> \<brocom:specification\>GMW-Eigenaar.Datum *gebeurtenis* (GMW\_Owner.eventDate) = (2018-09-01, JJJJ-MM-DD) *waarde* is *niet* correct: *mag niet* in *de toekomst liggen*.\</brocom:specification\> \</brocom:sourceDocumentError\> \</isgmw:intakeResponse\> |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


### Softwarefout

Voorbeeld van de situatie dat een softwarefout in het systeem van de
dataleverancier wordt geconstateerd.

| \<soap:Fault xmlns:soap=*"http://schemas.xmlsoap.org/soap/envelope/"*\> \<faultcode\>soap:Client\</faultcode\> \<faultstring\>*Het verzoek voldoet niet aan het* schema.\</faultstring\> \<detail\> \<parseFault xmlns:brocom=<http://www.broservices.nl/xsd/brocommon/3.0> xmlns=*"http://www.broservices.nl/xsd/isgmw/1.0"*\> \<brocom:requestReference\>levering1-20150726\</brocom:requestReference\> \<brocom:transactionId\>GMW-000000042842\</brocom:transactionId\> \<brocom:abortTime\>2017-06-13T14:08:39+01:00\</brocom:abortTime\> \<brocom:abortReason\> \<brocom:sequenceNumber\>1\</brocom:sequenceNumber\> \<brocom:specification\>*regel*: 1, *kolom*: 2895, offset: -1, *boodschap*: 'null'\</brocom:specification\> \</brocom:abortReason\> \<brocom:abortReason\> \<brocom:sequenceNumber\>2\</brocom:sequenceNumber\> \<brocom:specification\>*regel*: 1, *kolom*: 2895, offset: -1, *boodschap*: '*cvc*-*datatype*-valid.1.2.1: '*abcd*' is not a valid value for 'double'.'\</brocom:specification\> \</brocom:abortReason\> \<brocom:abortReason\> \<brocom:sequenceNumber\>3\</brocom:sequenceNumber\> \<brocom:specification\>*regel*: 1, *kolom*: 2895, offset: -1, *boodschap*: '*cvc*-complex-type.2.2: Element 'ns:objectIdAccountableParty' must have no element [children], and the value must be valid.'\</brocom:specification\> \</brocom:abortReason\> \</parseFault\> \</detail\> \</soap:Fault\> |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|


### Systeemfout

Voorbeeld van de situatie dat er een systeemfout optreedt in het BRO-systeem.

| \<soap:Fault xmlns:soap=*"http://schemas.xmlsoap.org/soap/envelope/"*\> \<faultcode\>soap:Client\</faultcode\> \<faultstring\>*Er* is *een fout* in *het* BRO-*systeem geconstateerd*.\</faultstring\> \<detail\> \<abortTime\>2017-06-13T14:06:03+01:00\</abortTime\> \</detail\> \</soap:Fault\> |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

