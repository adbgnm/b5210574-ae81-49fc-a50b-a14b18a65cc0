Basisregistratie Ondergrond (BRO) Uitgiftehandboek

Grondwatermonitoringput

**Colofon**

|                  | Bestuurskern                         |   |
|------------------|--------------------------------------|---|
|                  | Dir. Ruimtelijke Ontwikkeling        |   |
|                  |                                      |   |
|                  | Rijnstraat 8                         |   |
| 2515 XP Den Haag |                                      |   |
|                  |                                      |   |
|                  |                                      |   |
| Algemeen contact | Programmabureau BRO                  |   |
|                  | Directoraat-Generaal Ruimte en Water |   |
|                  | bro\@minienm.nl                      |   |
|                  |                                      |   |
| Versie           | 1.0                                  |   |
|                  |                                      |   |
| Auteur           | TNO Geologische Dienst Nederland     |   |
|                  |                                      |   |

Inhoudsopgave

[1 Inleiding 5](#inleiding)

[1.1 Doel en doelgroep uitgiftehandboek 5](#doel-en-doelgroep-uitgiftehandboek)

[1.2 Samenhang met andere documentatie 5](#samenhang-met-andere-documentatie)

[1.3 Versiehistorie 7](#versiehistorie)

[1.4 Contactinformatie 7](#contactinformatie)

[2 Uitgifte van gegevens 8](#uitgifte-van-gegevens)

[2.1 Twee manieren van uitgifte 8](#twee-manieren-van-uitgifte)

[2.2 DINOloket 8](#dinoloket)

[2.3 Uitgiftewebservice 9](#uitgiftewebservice)

[2.3.1 Communicatie tussen twee systemen 9](#communicatie-tussen-twee-systemen)

[2.3.2 Opties bij opvragen via de webservice
10](#opties-bij-opvragen-via-de-webservice)

[2.3.3 Opvragen van kengegevens 11](#opvragen-van-kengegevens)

[2.3.4 Opvragen van gegevens 12](#opvragen-van-gegevens)

[3 Opvragen via de webservice: de berichten
14](#opvragen-via-de-webservice-de-berichten)

[3.1 Opvragen van kengegevens 14](#opvragen-van-kengegevens-1)

[3.1.1 Verzoek tot verzending 14](#verzoek-tot-verzending)

[3.1.2 Bericht van afwijzing 15](#bericht-van-afwijzing)

[3.1.3 Bericht van verzending 16](#bericht-van-verzending)

[3.2 Opvragen van gegevens 16](#opvragen-van-gegevens-1)

[3.2.1 Verzoek tot verzending 17](#verzoek-tot-verzending-1)

[3.2.2 Bericht van afwijzing 17](#bericht-van-afwijzing-1)

[3.2.3 Bericht van verzending 17](#bericht-van-verzending-1)

[3.3 Meldingen 18](#meldingen)

[4 Opvragen via DINOloket 20](#opvragen-via-dinoloket)

[4.1 De kaart als interface 20](#de-kaart-als-interface)

[4.2 Zoeken op BRO-ID 21](#zoeken-op-bro-id)

[5 Specificatie van de berichten bij gebruik van de webservice
22](#specificatie-van-de-berichten-bij-gebruik-van-de-webservice)

[5.1 Inleiding 22](#inleiding-1)

[5.2 Berichten 22](#berichten)

[5.2.1 Verzoek tot verzending kengegevens
22](#verzoek-tot-verzending-kengegevens)

[5.2.2 Verzoek tot verzending gegevens 26](#verzoek-tot-verzending-gegevens)

[5.2.3 Bericht van afwijzing 27](#bericht-van-afwijzing-2)

[5.2.4 Bericht van verzending kengegevens
28](#bericht-van-verzending-kengegevens)

[5.2.5 Bericht van verzending gegevens 29](#bericht-van-verzending-gegevens)

[5.3 Specifieke domeinen voor uitgifte 29](#specifieke-domeinen-voor-uitgifte)

[5.3.1 Rechthoek 29](#rechthoek)

[5.3.2 Cirkel 30](#cirkel)

[5.3.3 Getalswaardeinterval 30](#getalswaardeinterval)

[5.3.4 Datuminterval 30](#datuminterval)

[5.3.5 Kenmerkfout 31](#kenmerkfout)

[5.3.6 RedenAfwijzing 32](#redenafwijzing)

[5.3.7 TeLeverenGegevens 32](#televerengegevens)

[5.3.8 Uitgiftedocumenttype 33](#uitgiftedocumenttype)

[5.4 Uitgiftedocumenten 33](#uitgiftedocumenten)

[5.4.1 BRO-DO 33](#bro-do)

[5.4.2 GMW-C 34](#gmw-c)

[5.4.3 GMW-PO 36](#gmw-po)

[5.4.4 GMW-PO-DP 36](#gmw-po-dp)

[5.4.5 GMW-PPO 36](#gmw-ppo)

[5.4.6 GMW-PPO-DP 37](#gmw-ppo-dp)

1.  Inleiding

    1.  Doel en doelgroep uitgiftehandboek

In de basisregistratie ondergrond (BRO) wordt een aantal typen gegevens
geregistreerd, de *registratieobjecten*. Een van de registratieobjecten is de
grondwatermonitoringput.

Het uitgiftehandboek richt zich op de partijen die de grondwatermonitoringput
van de BRO willen opvragen en beschrijft hoe het proces van gegevensuitgifte
globaal verloopt.

Het doel is de afnemers van gegevens, de data-afnemers, in algemeen
begrijpelijke bewoordingen inzicht te geven in de stappen die in dit proces
worden doorlopen, in de begrippenwereld die wordt gehanteerd, in de vormen van
controle en in de berichten die tussen de afnemer en de registerbeheerder worden
uitgewisseld.

Samenhang met andere documentatie 
----------------------------------

Voor ieder registratieobject in de BRO worden de volgende beschrijvende
documenten opgesteld:

-   een catalogus,

-   de handboeken voor inname en uitgifte;

-   de koppelvlakbeschrijvingen voor inname en uitgifte.

De *catalogus* beschrijft de gegevensinhoud van een registratieobject en vormt
de basis voor de andere beschrijvende documenten. In de catalogus staan de
definities van de gegevens en alle regels waaraan zij moeten voldoen.

Een *handboek* voor inname of uitgifte beschrijft het proces dat bij inname of
uitgifte van gegevens wordt doorlopen. Alle registratieobjecten kunnen
aangeboden worden via webservices, bepaalde registratieobjecten kunnen ook
aangeboden worden via het innameloket. Bij uitgifte kan de afnemer voor alle
objecten kiezen tussen webservices of DINO*loket*.

De *koppelvlakbeschrijvingen* zijn geschreven voor softwareontwikkelaars en zijn
bedoeld voor de partijen die de webservices gaan gebruiken. Op basis van de twee
vorige typen documenten staat hierin beschreven hoe het registratieobject en de
processen van inname of uitgifte worden vertaald naar het technische koppelvlak
dat is gerealiseerd door middel van webservices. De koppelvlakbeschrijving gaat
dus in op de technische kant van de overdracht van gegevens.

Deze documenten hangen samen zoals hieronder afgebeeld.

![](media/87444e32db59cc47e6661635b7f351e7.png)

*Figuur 1: Samenhang van de documentatie.*

Hoofdstuk 1 geeft het doel en de doelgroep, de samenhang met andere documenten
en de versiehistorie van dit uitgiftehandboek.

Hoofdstuk 2 geeft een inleiding op de uitgifte van gegevens uit de
basisregistratie ondergrond. Hierbij wordt ingegaan op de keuzen die een
gebruiker moet maken als hij gegevens wil opvragen.

Hoofdstuk 3 gaat in op de berichten die bij het gebruik van de webservice worden
uitgewisseld. Het hoofdstuk vertelt welke gegevens een data-afnemer moet
meesturen met zijn verzoek en welke gegevens hij terug kan verwachten als
antwoord.

Hoofdstuk 4 legt globaal uit hoe het opvragen via DINO*loket* verloopt.

Hoofdstuk 5 geeft een specificatie van de berichten die worden uitgewisseld bij
gebruik van de webservice inclusief de gegevens die de afnemer krijgt.

Versiehistorie 
---------------

|           | Datum           | Omschrijving                                                                                                                                                                   |
| Versie    |                 |                                                                                                                                                                                |
|-----------|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| concepten | September 2016  | Interne versies.                                                                                                                                                               |
| 0.7       | 17 oktober 2016 | Versie voor de eerste ketentest.                                                                                                                                               |
| 0.9       | 21 juni 2017    | Versie met verwerking van het commentaar uit de ketentest en de gevolgen van de consolidatie van het systeem, die aansluit op de catalogus Grondwatermonitoringput versie 1.0. |
| 1.0       | 28 juni 2017    | Versie vastgesteld door het Ministerie van Infrastructuur en Milieu                                                                                                            |

Contactinformatie 
------------------

Voor vragen, suggesties of opmerkingen over de inhoud van dit document kunt u
contact opnemen met de servicedesk van de beheerder van de basisregistratie
ondergrond via <info@basisregistratieondergrond.nl>.

1.  Uitgifte van gegevens

    1.  Twee manieren van uitgifte

Iedereen mag gegevens opvragen uit de registratie ondergrond en men kan daarbij
kiezen uit twee mogelijkheden, via DINO*loket* of via een uitgiftewebservice. De
verschillen tussen de twee zijn groot en wat de gebruiker kiest hangt af van
zijn informatiebehoefte en de technische mogelijkheden waarover hij beschikt.  
DINO*loket* biedt een laagdrempelige manier voor het opvragen van gegevens die
door iedereen kan worden gebruikt. De webservice geeft meer direct toegang tot
de registratie, maar vraagt wel dat de gebruiker over geschikte software
beschikt.

DINO*loket* 
------------

DINO*loket* is een website die toegang geeft tot de gegevens van alle
registratieobjecten in de BRO. Het gebruik van de website stelt geen bijzondere
eisen. De gebruiker kan op de website bepalen in welke objecten hij
geïnteresseerd is, de belangrijkste gegevens daarvan bekijken en uiteindelijk
besluiten van welke objecten hij gegevens wil aanvragen. De opgevraagde gegevens
worden hem vervolgens per e-mail toegestuurd. Het enige wat van de data-afnemer
gevraagd wordt is dat hij bij het indienen van zijn aanvraag zijn e-mailadres
opgeeft.

DINO*loket* biedt niet alleen toegang tot de registratieobjecten in de BRO, maar
ook tot de gegevens in het systeem DINO. De keuzemogelijkheden zijn groot en de
gebruiker wordt door het selectieproces geleid zodat hij stapsgewijs kan bepalen
welke gegevens hij wil opvragen. Het loket biedt de gebruiker de mogelijkheid
gegevens uit DINO en de BRO te combineren.

Gegevens uit DINO worden uitgegeven in een formaat dat aansluit bij de bestaande
praktijk. De gegevens uit de BRO worden standaard uitgegeven in IMBRO-XML
formaat. Wanneer dat nodig is wordt naast het IMBRO-XML-formaat nog een ander
formaat ondersteund.

DINO*loket* is zo gebouwd dat de gebruiker eigenlijk geen fouten kan maken bij
het invoeren van zijn keuze zodat de gegevens die hij opvraagt ook zonder
problemen geleverd kunnen worden.

Uitgiftewebservice
------------------

Opvragen van gegevens via de uitgiftewebservice verloopt heel anders dan via het
loket. De gebruiker die via de webservice gegevens opvraagt krijgt de gegevens
onmiddellijk geleverd. Maar om de webservice te kunnen gebruiken moet hij wel
over software beschikken die de webservice kan aanroepen en moet hij zich als
data-afnemer bij de BRO laten registreren. De eis die daarbij wordt gesteld is
dat de organisatie waar hij werkt beschikt over een *PKIoverheid services
certificaat*. Dat certificaat is een soort digitaal paspoort, het
legitimatiebewijs van het softwaresysteem van de gebruiker.

Opvragen van gegevens via de uitgiftewebservice is snel, betrouwbaar en
elementair. Dat laatste betekent in de eerste plaats dat er voor ieder type
registratieobject een aparte webservice is. Wil men gegevens van meer dan een
type opvragen, dan moet men verschillende webservices gebruiken. Verder heeft de
gebruiker beperkte keuzevrijheid. Hij kan of alle gegevens van een enkel
registratieobject opvragen of een beperkte selectie van gegevens van een aantal
registratieobjecten tegelijk. De reden daarachter is dat een webservice alleen
in algemene gebruikerswensen voorziet. De eigen software van de data-afnemer
moet zo zijn ingericht dat de webservice wordt aangeroepen op een manier die
aansluit op de eigen bedrijfsprocessen.

Het proces van uitgifte is bij het gebruik van de webservice strikt
geformaliseerd. De webservice verzorgt de communicatie tussen twee
softwaresystemen en om te borgen dat de verwerking van een verzoek automatisch
kan verlopen zijn er allerlei controles ingebouwd. Een ander verschil is dat men
de gegevens altijd in het IMBRO-XML formaat krijgt.

### *Communicatie tussen twee systemen*

De data-afnemer die voor het opvragen van gegevens van
grondwatermonitoringputten gebruik maakt van de uitgiftewebservice, gebruikt via
zijn eigen systeem algemene BRO-software die via het internet voor iedereen te
vinden is. Het adres van de BRO-webservices is te vinden op
[www.broinfo.nl](http://www.broinfo.nl/).

De webservice zorgt ervoor dat het systeem van de data-afnemer een verzoek tot
verzending van een grondwatermonitoringput aan het BRO-systeem kan aanbieden,
zorgt voor de verwerking van het verzoek en geeft het antwoord van de BRO terug
aan het systeem van de data-afnemer (Figuur 2). Als alles goed is gegaan bevat
het antwoord de opgevraagde gegevens.

![](media/d0f7b009812bbfc470b6fc603b45a42d.png)

*Figuur 2: De webservice zorgt voor communicatie tussen twee systemen.*

### *Opties bij opvragen via de webservice*

De uitgiftewebservice voorziet in elementaire functionaliteit en die dekt drie
gebruikscasussen. De eerste is het geval waarin een gebruiker aanvankelijk niet
precies weet welke objecten hij wil hebben en daarom op zoek gaat naar de
objecten die aan bepaalde kenmerken voldoen.

De tweede casus is het geval waarin de gebruiker weet welke objecten aan zijn
kenmerken voldoen en hij alleen de actuele gegevens van een object wil opvragen.
Actueel wil zeggen de gegevens met de waarde die op het moment van opvragen
geldt. De grondwatermonitoringput is namelijk een registratieobject met een
*materiële geschiedenis* en dat betekent dat de waarde van bepaalde gegevens in
de loop van de tijd kan wijzigen.

De derde casus is het geval waarin de gebruiker weet welke objecten aan zijn
kenmerken voldoen en hij zowel de actuele als de historische waarden van de
gegevens van een object wil opvragen.

De drie opties zijn vertaald in twee verzoeken:

1.  Een verzoek tot verzending van de kengegevens van een aantal
    grondwatermonitoringputten.

>   De data-afnemer geeft in zijn verzoek de verzameling kenmerken mee waaraan
>   de grondwatermonitoringputten die hij zoekt moeten voldoen. In antwoord
>   daarop krijgt hij van ieder van de objecten die aan de kenmerken voldoen de
>   gegevens geleverd die het object karakteriseren, met ter identificatie het
>   BRO-ID.

1.  Een verzoek tot verzending van de gegevens van een bepaalde
    grondwatermonitoringput.

>   De data-afnemer geeft in zijn verzoek het BRO-ID van het
>   grondwatermonitoringput die hij wil hebben mee en specificeert of hij alleen
>   de actuele gegevens of de actuele en de historische gegevens wil hebben. In
>   antwoord daarop krijgt hij de gevraagde gegevens van de put geleverd.

In de volgende paragrafen wordt de verwerking in meer detail beschreven.

### *Opvragen van kengegevens*

Het opvragen van kengegevens verloopt volgens een vaste opeenvolging van
stappen.

Dit is waar het in het kort op neerkomt:

1.  De data-afnemer stuurt vanuit zijn systeem een verzoek tot verzending van
    kengegevens. Daarbij geeft hij de kenmerken mee van de
    grondwatermonitoringputten waarvan hij gegevens wil krijgen.

2.  Het systeem van de BRO voert een toegangscontrole uit.

3.  Wanneer toegang tot het systeem van de BRO is verkregen, begint de controle
    van het verzoek en wordt onder meer vastgesteld of het verzoek inhoudelijk
    aan de gestelde eisen voldoet.

    -   Wanneer de inhoudelijke controle fouten oplevert, wordt het verzoek
        afgewezen en ontvangt het systeem van de data-afnemer een bericht van
        afwijzing.

4.  Wanneer de inhoudelijke controle geen fouten oplevert en er ook geen
    technische problemen zijn, verzamelt het systeem van de BRO de kengegevens
    van de grondwatermonitoringputten die aan de meegegeven kenmerken voldoen.

    -   Wanneer de verzameling gegevens te groot is, wijst het BRO-systeem het
        verzoek tot verzending alsnog af en ontvangt het systeem van de
        data-afnemer een bericht van afwijzing.

    -   Wanneer de verzameling onder het gestelde maximum ligt stuurt het
        BRO-systeem de data-afnemer de opgevraagde gegevens in een bericht van
        verzending.

Het verzoek van de data-afnemer en het antwoord dat de BRO daarop normaliter
geeft worden *berichten* genoemd. In het geval zich technische problemen
voordoen, wordt het antwoord een *melding* genoemd.

De stappen en de bijbehorende berichten worden in het onderstaande plaatje
uitgebeeld.

![](media/d293a0656bbd4f9ec61a54d073607d78.png)

*Figuur 3: Verwerking van een verzoek tot verzending van kengegevens.*

### *Opvragen van gegevens* 

Het opvragen van de gegevens van een grondwatermonitoringput verloopt iets
anders dan het opvragen van kengegevens.

![](media/6743fad1c2b0fe9894d930dcd8d47cf6.png)

*Figuur 4: Verwerking van een verzoek tot verzending van gegevens van een
grondwatermonitoringput.*

De berichten die worden uitgewisseld zijn alleen qua inhoud anders dan berichten
bij een verzoek tot levering van kengegevens. Een bijzonderheid is dat
bronhouders en data-afnemers iets meer gegevens geleverd krijgen dan andere
afnemers.

1.  Opvragen via de webservice: de berichten

    1.  Opvragen van kengegevens

Het opvragen van de kengegevens van een aantal grondwatermonitoringputten
verloopt op basis van één of meer kenmerken.

### *Verzoek tot verzending* 

![](media/a8a2b5e5febfcb33a11ce8b65ee6d8af.png)

Het belangrijkste onderdeel van het *verzoek tot verzending* van kengegevens is
de *kenmerkenverzameling,* dat is het geheel van kenmerken waaraan de
grondwatermonitoringput die de afnemer wil krijgen moet voldoen. Door het
meegeven van kenmerken kan de data-afnemer de zoekvraag preciseren naar plaats,
tijd en aard van de constructie.

De kenmerken die de data-afnemer kan kiezen, worden in hoofdstuk 5
gespecificeerd. Het is een keuze uit de gegevens die in de catalogus voor de
grondwatermonitoringput zijn beschreven, met daarbij aangegeven hoe de waarde
moet worden gespecificeerd.

De data-afnemer moet als kenmerk in ieder geval opgeven in welk gebied de
locatie van de grondwatermonitoringput moet liggen. Dat kenmerk kan hij
combineren met een of meer andere kenmerken.

Naast deze kenmerken moet de data-afnemer een *verzoekkenmerk* meegeven. Dat
gegeven kan worden gebruikt in de communicatie met de servicedesk, bijvoorbeeld
als er iets mis is gegaan en de data-afnemer wil over het probleem contact
zoeken met de servicedesk.

### *Bericht van afwijzing*

![](media/e679756c8c5af5cc3ee223af5e2deb14.png)

In de verwerking van het verzoek zijn allerlei controles ingebouwd. Als er in
technische zin iets mis gaat, krijgt de data-afnemer een melding. Een *bericht
van afwijzing* krijgt hij als antwoord, wanneer bij de controles blijkt dat zich
een probleem voordoet dat bij het invoeren van gegevens moet worden opgelost.

![](media/ad93e1a229781ff74e5b612362f5b132.png)

Het bericht van afwijzing bevat het *tijdstip van afwijzing* en het
*verzoekkenmerk* van de data-afnemer, maar het belangrijkste onderdeel is de
*reden afwijzing*. De reden waarom het verzoek is afgewezen hangt af van de aard
van het probleem. Het probleem kan zijn dat er een fout zit in de gegevens die
de data-afnemer heeft meegegeven, maar het kan ook zijn dat bij het verzamelen
van gegevens blijkt dat het maximum aantal registratieobjecten wordt
overschreden.

*Figuur 5: Twee controles kunnen leiden tot een bericht van afwijzing.*

Fouten in de gegevens die de data-afnemer heeft meegegeven worden in het bericht
zo omschreven dat de afnemer direct kan zien waar de fout zit en wat de fout
inhoudt.

Het bericht van afwijzing dat gestuurd wordt na de tweede controle heeft een
eenvoudige boodschap. Het aantal objecten waarvan kengegevens worden geleverd is
beperkt tot 2000. De foutmelding geeft in dit geval alleen aan dat het maximum
is overschreden.

### *Bericht van verzending*

![](media/9ffe3dbeaa3e5b7f5f05a163632bfd62.png)

Het belangrijkste onderdeel van het *bericht van verzending* zijn de
uitgiftedocumenten. Ieder *uitgiftedocument* bevat de kengegevens van een
grondwatermonitoringput die de gewenste kenmerken heeft. Het bericht bevat
verder het *tijdstip van uitgifte*, het *verzoekkenmerk* van de data-afnemer en
de vermelding van het aantal uitgiftedocumenten. Er worden maximaal 2000
uitgiftedocumenten verzonden.

De lijst met kengegevens die standaard worden uitgegeven wordt gespecificeerd in
hoofdstuk 5.

Er is één uitzondering op de standaardlijst en dat is wanneer een
registratieobject door de registerbeheerder uit registratie is genomen. Dat
geval doet zich bijvoorbeeld voor wanneer een object ten onrechte is opgenomen
in de registratie en de registerbeheerder, na onderzoek en overleg met de
bronhouder, van die laatste het akkoord heeft gekregen het object uit
registratie te nemen. In dat uitzonderlijke geval ontvangt de data-afnemer een
bijzonder type uitgiftedocument dat enkel de volgende gegevens over het
betreffende registratieobject bevat:

| *Entiteit*              | *Attribuut*                      |
|-------------------------|----------------------------------|
| Grondwatermonitoringput | BRO-ID                           |
| Registratiegeschiedenis | uit registratie genomen          |
|                         | tijdstip uit registratie genomen |

Tot slot kan het voorkomen dat er geen enkel registratieobject bestaat dat aan
de kenmerken voldoet die zijn meegegeven. Dan ontvangt de data-afnemer wel een
bericht van verzending, maar worden er geen uitgiftedocumenten meegeleverd.

Opvragen van gegevens 
----------------------

Het opvragen van de gegevens van een grondwatermonitoringput verloopt op basis
van het BRO-ID.

### *Verzoek tot verzending*

![cid:image007.png\@01D2F029.FD9520E0](media/30710792593d26524ff348c9281d99b2.png)

Het *verzoek tot verzending* van de gegevens van een grondwatermonitoringput
bestaat uit drie gegevens. Het *verzoekkenmerk*, het *BRO-ID* van de
grondwatermonitoringput dat de data-afnemer wil krijgen en een aanduiding van de
te leveren gegevens. Met het laatste geeft de data-afnemer aan of hij alleen de
actuele gegevens of ook de historische gegevens van een grondwatermonitoringput
wil ontvangen.

### *Bericht van afwijzing*

![](media/706a33dae86da31ed3bc3eaf9962f8d7.png)

Een bericht van afwijzing wordt bij dit type verzoek alleen gestuurd als de BRO
een fout in het verzoek zelf heeft geconstateerd, dus wanneer er bij het
invoeren van het verzoekkenmerk of het BRO-ID iets mis is gegaan. De controle is
eenvoudig: de drie gegevens moeten aan de specificaties (zie hoofdstuk 5)
voldoen. Ook wanneer de data-afnemer per ongeluk een BRO-ID heeft opgegeven dat
niet bestaat, stuurt de BRO een bericht van afwijzing als antwoord.

### *Bericht van verzending* 

![](media/28afcbe0f08568400ade8a61ee24c2eb.png)

Het *bericht van verzending* bevat maar een uitgiftedocument en dat bevat de
gewenste gegevens van de opgevraagde grondwatermonitoringput. Verder bevat het
bericht de verwijzing naar het verzoek tot verzending en het tijdstip waarop de
gegevens zijn verzonden.

Welke gegevens er precies in het uitgiftedocument zitten hangt niet alleen af
van wat de data-afnemer heeft opgevraagd. Het wordt ook bepaald door de vraag of
de data-afnemer tevens de bronhouder of de data-afnemer van de betreffende
grondwatermonitoringput is. Die twee partijen krijgen alle gegevens van het
registratieobject geleverd. Dat geldt zelfs in het uitzonderlijke geval dat het
registratieobject door de registerbeheerder uit registratie is genomen.

De andere data-afnemers krijgen alle gegevens op drie na. De drie gegevens die
ze niet geleverd krijgen zijn:

| *Entiteit*              | *Attribuut*             |
|-------------------------|-------------------------|
| Grondwatermonitoringput | object-ID bronhouder    |
|                         | dataleverancier         |
|                         | onderhoudende instantie |

In het uitzonderlijke geval dat het registratieobject uit registratie is
genomen, krijgen de gewone data-afnemers een ander type uitgiftedocument dat
alleen de volgende gegevens bevat:

| *Entiteit*              | *Attribuut*                      |
|-------------------------|----------------------------------|
| Grondwatermonitoringput | BRO-ID                           |
| Registratiegeschiedenis | uit registratie genomen          |
|                         | tijdstip uit registratie genomen |

Meldingen
---------

Een melding is het antwoord dat de BRO stuurt wanneer er op technisch vlak iets
mis is gegaan. Meldingen zijn in eerste instantie bedoeld voor programmeurs. Om
die reden worden de meldingen uitgebreid behandeld in de koppelvlakbeschrijving;
hier wordt alleen achtergrondinformatie gegeven.

De oorzaak van een technisch probleem kan variëren en er worden drie categorieën
meldingen onderscheiden:

-   melding van een probleem bij de toegangscontrole,

-   melding van een probleem in de software van de data-afnemer,

-   melding van een systeemfout.

Toegangscontrole houdt in dat het systeem van de BRO controleert of de
data-afnemer daadwerkelijk is wie hij beweert te zijn en of hij het recht heeft
gebruik te maken van de uitgiftewebservice. Het optreden van een probleem bij de
toegangscontrole is uitzonderlijk en het zal zich eigenlijk alleen voordoen
wanneer een data-afnemer voor het eerst gebruik wil maken van de webservice.

Problemen in de software van de data-afnemer kunnen

vaker optreden, maar ook deze zullen zich in eerste instantie met name openbaren
in de fase waarin de data-afnemer bezig is zijn software geschikt te maken voor
aansluiting op de BRO.

Systeemfouten doen zich voor wanneer er problemen zijn met de software van de
BRO of wanneer zich onvoorziene omstandigheden voordoen, bijvoorbeeld wanneer de
stroomtoevoer hapert. Fouten in het systeem van de BRO kunnen verwacht worden in
de testfase. Wanneer het systeem in productie is genomen mogen ze eigenlijk niet
meer optreden. Gebeurt dat toch, dan alleen in de korte periode direct na
inproductiename. Onvoorziene omstandigheden kunnen zich daarentegen altijd
voordoen.

Opvragen via DINOloket
======================

De gebruiker die via DINO*loket* gegevens uit de basisregistratie ondergrond wil
opvragen, gaat naar [www.dinoloket.nl](http://www.dinoloket.nl) en kiest op de
eerste pagina van de website de module Ondergrondgegevens.

DINO*loket* biedt niet alleen toegang tot de registratieobjecten in de BRO, maar
ook tot de gegevens in het systeem DINO. In het geval van de
grondwatermonitoringput zitten de objecten alleen in de BRO, maar dat is pas het
geval wanneer de conversie van gegevens uit DINO voltooid is.

De kaart als interface
----------------------

DINO*loket* is ontworpen vanuit de gedachte dat de gegevens altijd in een
geografische context getoond en opgevraagd moeten worden en dat de gebruiker
niet precies weet welke objecten hij wil hebben. De gebruiker heeft daarom
altijd de beschikking over een kaart en hij kan kiezen wat hij daarop wil zien.

Eenmaal in de module Ondergrondgegevens, kiest de gebruiker de categorieën
gegevens hij wil zien. In het geval van de grondwatermonitoringput, selecteert
hij het domein *Grondwateronderzoek* en vinkt hij *grondwatermonitoringput* aan.
Hij krijgt dan op de kaart de locatie van alle registratieobjecten te zien. Door
de kenmerken op te geven waaraan de put moet voldoen, kan hij zijn opdracht
verfijnen. Dat is vergelijkbaar met het opvragen van kengegevens via de
webservice, maar het aantal kenmerken is beperkt tot de belangrijkste. Van ieder
object op de kaart kan hij de kengegevens bekijken door op het symbool op de
kaart te klikken.

Als hij zijn keuze globaal heeft bepaald, gaat hij door naar de volgende stap
waarin hij het gebied waarin hij geïnteresseerd is preciezer bepaalt. Hij heeft
de beschikking over een lijst waarin alle objecten die in het gebied liggen zijn
opgenomen en daarin is een aantal kenmerken opgenomen op basis waarvan hij zijn
selectie verder kan inperken. Ook in deze stap kan de gebruiker de kengegevens
van een bepaald object bekijken door op de kaart te klikken.

Heeft de gebruiker bepaald van welke grondwatermonitoringputten hij de gegevens
wil hebben, dan gaat hij naar de laatste stap en dat is dat hij wat gegevens
invult die voor verzending nodig zijn. Een daarvan is dat hij kiest in welke
formaat hij de bestanden wil krijgen. In het geval van de
grondwatermonitoringput heeft hij vooralsnog geen keuze en krijgt hij altijd
IMBRO-XML. Zijn alle gegevens ingevuld dan kan hij zijn verzoek indienen. Als
antwoord krijgt hij een link naar het zip-bestand, zodat hij de gegevens kan
downloaden.

Zoeken op BRO-ID
----------------

Hoewel DINOloket is ontworpen vanuit de gedachte de gebruiker niet precies weet
welke objecten hij wil hebben, is het ook mogelijk een bepaald object uit een
van de registraties direct op te vragen. In het geval van de
grondwatermonitoringput gebeurt dat door het BRO-ID in te voeren, zodra hij in
de module Ondergrondgegevens is terechtgekomen. De kaart zoomt vervolgens in op
dat object en de gebruiker kan de andere stappen snel doorlopen om de gegevens
op te vragen.

1.  Specificatie van de berichten bij gebruik van de webservice

    1.  Inleiding

In dit hoofdstuk worden de gegevensinhoud beschreven van de berichten die bij
uitgifte worden uitgewisseld tussen het systeem van de data-afnemer en het
BRO-systeem. De systematiek van de beschrijving is dezelfde als in de catalogus.

Eerst worden de berichten beschreven op basis van een model dat de vorm heeft
van een UML-diagram. Na de berichten worden de domeinen behandeld die specifiek
zijn voor de berichten. Aan het eind van het hoofdstuk worden de UML-modellen
van de verschillende typen uitgiftedocumenten gegeven.

Het handboek is een aanvulling op de catalogus en om die reden wordt een gegeven
hier alleen gedefinieerd wanneer het niet in de catalogus is opgenomen of
wanneer er bijzondere regels gelden. Wanneer alleen de kardinaliteit van een
gegeven afwijkt van die in de catalogus, is dat geen reden geweest het hier op
te nemen.

1.  Berichten

    1.  *Verzoek tot verzending kengegevens*

![](media/70b97b45adcd848d7f014fff2d9dddcf.emf)

| **verzoekkenmerk**                   |                                                                                                                                                                                        |
|--------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Naam attribuut                       | verzoekkenmerk                                                                                                                                                                         |
| Definitie                            | Het kenmerk dat de gebruiker, in dit geval de data-afnemer, meegeeft om het verzoek te identificeren.                                                                                  |
| Kardinaliteit                        | 1                                                                                                                                                                                      |
| Domein                               | Tekst                                                                                                                                                                                  |
| Maximale lengte                      | 200                                                                                                                                                                                    |
|                                      |                                                                                                                                                                                        |
| **Kenmerkenverzameling**             |                                                                                                                                                                                        |
| Naam entiteit                        | Kenmerkenverzameling                                                                                                                                                                   |
| Definitie                            | Het geheel van kenmerken waaraan een grondwatermonitoringput die de gebruiker opvraagt moet voldoen.                                                                                   |
| Kardinaliteit                        | 1                                                                                                                                                                                      |
| Toelichting                          | Bijna alle gegevens die als kenmerk gebruikt worden zijn gedefinieerd in de catalogus met als enige verschil dat de kardinaliteit 0..1 is omdat de gebruiker vrijheid van keuze heeft. |
|                                      |                                                                                                                                                                                        |
| **periode van registratie**          |                                                                                                                                                                                        |
| Naam attribuut                       | periode van registratie                                                                                                                                                                |
| Definitie                            | Het datuminterval waarbinnen de registratiedatum van de grondwatermonitoringput ligt                                                                                                   |
| Kardinaliteit                        | 0..1                                                                                                                                                                                   |
| Domein                               | Datuminterval                                                                                                                                                                          |
| Waardebereik                         | 1 juli 2017 tot datum van uitgifte                                                                                                                                                     |
|                                      |                                                                                                                                                                                        |
| **periode van correctie**            |                                                                                                                                                                                        |
| Naam attribuut                       | periode van correctie                                                                                                                                                                  |
| Definitie                            | Het datuminterval waarbinnen het laatste correctietijdstip van de grondwatermonitoringput ligt.                                                                                        |
| Kardinaliteit                        | 0..1                                                                                                                                                                                   |
| Domein                               | Datuminterval                                                                                                                                                                          |
| Waardebereik                         | 1 juli 2017 tot datum van uitgifte                                                                                                                                                     |
|                                      |                                                                                                                                                                                        |
| **minimum aantal buizen**            |                                                                                                                                                                                        |
| Naam attribuut                       | minimum aantal buizen                                                                                                                                                                  |
| Definitie                            | Het aantal buizen dat een grondwatermonitoringput ten minste heeft.                                                                                                                    |
| Kardinaliteit                        | 0..1                                                                                                                                                                                   |
| Domein                               | Aantal                                                                                                                                                                                 |
|  Maximale lengte                     | 2                                                                                                                                                                                      |
| Waardebereik                         | 1 tot 50                                                                                                                                                                               |
|                                      |                                                                                                                                                                                        |
| **periode van inrichting**           |                                                                                                                                                                                        |
| Naam attribuut                       | periode van inrichting                                                                                                                                                                 |
| Definitie                            | Het datuminterval waarbinnen de inrichtingsdatum van de grondwatermonitoringput ligt.                                                                                                  |
| Kardinaliteit                        | 0..1                                                                                                                                                                                   |
| Domein                               | Datuminterval                                                                                                                                                                          |
| Waardebereik                         | 1 januari 1889 tot datum van uitgifte                                                                                                                                                  |
|                                      |                                                                                                                                                                                        |
| **periode van opruiming**            |                                                                                                                                                                                        |
| Naam attribuut                       | periode van opruiming                                                                                                                                                                  |
| Definitie                            | Het datuminterval waarbinnen de opruimingsdatum van de grondwatermonitoringput ligt.                                                                                                   |
| Kardinaliteit                        | 0..1                                                                                                                                                                                   |
| Domein                               | Datuminterval                                                                                                                                                                          |
| Waardebereik                         | 1 januari 1889 tot datum van uitgifte                                                                                                                                                  |
| **geo-ohmkabel aanwezig**            |                                                                                                                                                                                        |
| Naam attribuut                       | geo-ohmkabel aanwezig                                                                                                                                                                  |
| Definitie                            | De aanduiding die aangeeft of de grondwatermonitoringput voorzien is van een of meer geo-ohmkabels.                                                                                    |
| Kardinaliteit                        | 0..1                                                                                                                                                                                   |
| Domein                               | IndicatieJaNee=ja                                                                                                                                                                      |
| Type                                 | Enumeratie                                                                                                                                                                             |
|                                      |                                                                                                                                                                                        |
| **minimale diameter bovenkant buis** |                                                                                                                                                                                        |
| Naam attribuut                       | minimale diameter bovenkant buis                                                                                                                                                       |
| Definitie                            | De ondergrens voor de diameter van de bovenkant van de monitoringbuizen van een grondwatermonitoringput.                                                                               |
| Kardinaliteit                        | 0..1                                                                                                                                                                                   |
| Domein                               | Rationaal getal                                                                                                                                                                        |
| Maximale lengte                      | 4                                                                                                                                                                                      |
| Eenheid                              | mm (millimeter)                                                                                                                                                                        |
| Waardebereik                         | 3 tot 1000                                                                                                                                                                             |
|                                      |                                                                                                                                                                                        |
| **maximale diameter bovenkant buis** |                                                                                                                                                                                        |
| Naam attribuut                       | maximale diameter bovenkant buis                                                                                                                                                       |
| Definitie                            | De bovengrens voor de diameter van de bovenkant van de monitoringbuizen van een grondwatermonitoringput.                                                                               |
| Kardinaliteit                        | 0..1                                                                                                                                                                                   |
| Domein                               | Rationaal getal                                                                                                                                                                        |
| Maximale lengte                      | 4                                                                                                                                                                                      |
| Eenheid                              | mm (millimeter)                                                                                                                                                                        |
| Waardebereik                         | 3 tot 1000                                                                                                                                                                             |
|                                      |                                                                                                                                                                                        |
| **verticaal interval**               |                                                                                                                                                                                        |
| Naam attribuut                       | verticaal interval                                                                                                                                                                     |
| Definitie                            | Het bereik dat gedeeltelijk of geheel overlapt met het filterbereik van een grondwatermonitoringput.                                                                                   |
| Kardinaliteit                        | 0..1                                                                                                                                                                                   |
| Domein                               | Getalswaardeinterval                                                                                                                                                                   |
| Maximale lengte                      | 3                                                                                                                                                                                      |
| Eenheid                              | m (meter)                                                                                                                                                                              |
| Waardebereik                         | \-750 tot 325                                                                                                                                                                          |
| Toelichting                          | De getalswaarden zijn gedefinieerd t.o.v. het verticaal referentievlak (NAP).                                                                                                          |
|                                      |                                                                                                                                                                                        |
| **Gebied  **                         |                                                                                                                                                                                        |
| Naam entiteit                        | Gebied                                                                                                                                                                                 |
| Definitie                            | De geografische begrenzing waarbinnen de locatie van een grondwatermonitoringput ligt.                                                                                                 |
| Kardinaliteit                        | 1                                                                                                                                                                                      |
| Regels                               | Een gebied bestaat uit een omsluitende rechthoek of een omsluitende cirkel.                                                                                                            |
|                                      |                                                                                                                                                                                        |
| **omsluitende rechthoek  **          |                                                                                                                                                                                        |
| Naam attribuut                       | omsluitende rechthoek                                                                                                                                                                  |
| Definitie                            | Een gebied dat omsloten wordt door een rechthoek.                                                                                                                                      |
| Kardinaliteit                        | 0..1                                                                                                                                                                                   |
| Domein                               | Rechthoek                                                                                                                                                                              |
| Zuidwestelijk hoekpunt               | Coördinatenpaar voor ETRS89 (φ,λ)                                                                                                                                                      |
| Noordoostelijk hoekpunt              | Coördinatenpaar voor ETRS89 (φ,λ)                                                                                                                                                      |
|                                      |                                                                                                                                                                                        |
| **omsluitende cirkel  **             |                                                                                                                                                                                        |
| Naam attribuut                       | omsluitende cirkel                                                                                                                                                                     |
| Definitie                            | Een gebied dat omsloten wordt door een cirkel.                                                                                                                                         |
| Kardinaliteit                        | 0..1                                                                                                                                                                                   |
| Domein                               | Cirkel                                                                                                                                                                                 |
| Middelpunt                           | Coördinatenpaar voor ETRS89 (φ,λ)                                                                                                                                                      |
| Straal                               | Rationaal getal                                                                                                                                                                        |
|                                      | Maximale lengte: 2.3                                                                                                                                                                   |
|                                      | Eenheid: km (kilometer)                                                                                                                                                                |
|                                      | Waardebereik: 0 tot 10                                                                                                                                                                 |

### *Verzoek tot verzending gegevens*

![](media/c9277246ff7fd533039fd65fe140d9c7.emf)

| **te leveren gegevens** |                                                                    |
|-------------------------|--------------------------------------------------------------------|
| Naam attribuut          | te leveren gegevens                                                |
| Definitie               | De categorie gegevens die de gebruiker van het object wil krijgen. |
| Kardinaliteit           | 1                                                                  |
| Domein                  | TeLeverenGegevens                                                  |
| Type                    | Codelijst                                                          |

### *Bericht van afwijzing*

![](media/85504e93c48d149ef56e5b06a0366a19.emf)

| **tijdstip van afwijzing**  |                                                                                                                                                    |
|-----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------|
| Naam attribuut              | tijdstip van afwijzing                                                                                                                             |
| Definitie                   | De datum en het tijdstip waarop een verzoek door de BRO is afgewezen.                                                                              |
| Kardinaliteit               | 1                                                                                                                                                  |
| Domein                      | DatumTijd                                                                                                                                          |
| Toelichting                 | Het tijdstip van afwijzing wordt door de BRO toegekend.                                                                                            |
|                             |                                                                                                                                                    |
| **reden afwijzing**         |                                                                                                                                                    |
| Naam attribuut              | reden afwijzing                                                                                                                                    |
| Definitie                   | De omschrijving van de reden waarom het verzoek door de BRO is afgewezen.                                                                          |
| Kardinaliteit               | 1                                                                                                                                                  |
| Domein                      | RedenAfwijzing                                                                                                                                     |
| Type                        | Codelijst                                                                                                                                          |
|                             |                                                                                                                                                    |
| **Foutenoverzicht**         |                                                                                                                                                    |
| Naam entiteit               | Foutenoverzicht                                                                                                                                    |
| Definitie                   | De omschrijving van alle fouten die in de kenmerkenverzameling zijn gevonden.                                                                      |
| Kardinaliteit               | 0..1                                                                                                                                               |
| Regels                      | Het gegeven kan alleen voorkomen als de *reden van afwijzing* de waarde *er zijn 1 of meer fouten geconstateerd in de kenmerkenverzameling* heeft. |
| Toelichting                 | Het gegeven wordt door de BRO geproduceerd.                                                                                                        |
|                             |                                                                                                                                                    |
| **volgnummer**              |                                                                                                                                                    |
| Naam attribuut              | volgnummer                                                                                                                                         |
| Definitie                   | Het volgnummer van een fout in de kenmerkenverzameling.                                                                                            |
| Kardinaliteit               | 1..99                                                                                                                                              |
| Domein                      | Nummer                                                                                                                                             |
| Maximale lengte             | 2                                                                                                                                                  |
|                             |                                                                                                                                                    |
| **kenmerkfout**             |                                                                                                                                                    |
| Naam attribuut              | kenmerkfout                                                                                                                                        |
| Definitie                   | De omschrijving van een fout in de kenmerkenverzameling.                                                                                           |
| Kardinaliteit               | 1..99                                                                                                                                              |
| Domein                      | Kenmerkfout                                                                                                                                        |
| Type                        | Codelijst                                                                                                                                          |

### *Bericht van verzending kengegevens*

![](media/d2bcf73b1887ddc9ec70ff01ac84cd39.emf)

| **tijdstip van uitgifte** |                                                                                                   |
|---------------------------|---------------------------------------------------------------------------------------------------|
| Naam attribuut            | tijdstip van uitgifte                                                                             |
| Definitie                 | De datum en het tijdstip waarop het bericht door de BRO is verstuurd.                             |
| Kardinaliteit             | 1                                                                                                 |
| Domein                    | DatumTijd                                                                                         |
|                           |                                                                                                   |
| **uitgiftedocumenttype**  |                                                                                                   |
| Naam attribuut            | uitgiftedocumenttype                                                                              |
| Definitie                 | De aanduiding van het type document dat de afnemer wordt toegezonden in antwoord op zijn verzoek. |
| Kardinaliteit             | 0..2                                                                                              |
| Domein                    | Uitgiftedocumenttype                                                                              |
| Type                      | Codelijst                                                                                         |
|                           |                                                                                                   |
| **aantal documenten**     |                                                                                                   |
| Naam attribuut            | aantal documenten                                                                                 |
| Definitie                 | Het aantal uitgiftedocumenten dat in het bericht zit.                                             |
| Kardinaliteit             | 1                                                                                                 |
| Domein                    | Aantal                                                                                            |
| Maximale lengte           | 1                                                                                                 |
| Waardebereik              | 0 tot 2000                                                                                        |
|                           |                                                                                                   |

### *Bericht van verzending gegevens*

![](media/a3341870653b0ecc1ceaad5384b6ced1.emf)

| **uitgiftedocumenttype**  |                                                                                                   |
|---------------------------|---------------------------------------------------------------------------------------------------|
| Naam attribuut            | uitgiftedocumenttype                                                                              |
| Definitie                 | De aanduiding van het type document dat de afnemer wordt toegezonden in antwoord op zijn verzoek. |
| Kardinaliteit             | 1                                                                                                 |
| Domein                    | Uitgiftedocumenttype                                                                              |
| Type                      | Codelijst                                                                                         |

1.  Specifieke domeinen voor uitgifte

    1.  *Rechthoek*

Het domein van het type *rechthoek* wordt gebruikt voor een gebied op aarde dat
als een rechthoek wordt voorgesteld. De rechthoek wordt gedefinieerd door twee
punten die op het aardoppervlak liggen. Dat zijn in deze volgorde het punt dat
de zuidwesthoek, resp. de noordoosthoek vertegenwoordigt. Ieder van de punten
wordt uitgedrukt in het domein Coördinatenpaar (zie de catalogus) met als
referentiestelsel ETRS89 (ongeprojecteerd).

Het coördinatenpaar voor ETRS89 (φ,λ) is als volgt gedefinieerd:

Getalswaarde 2.9

Eenheid ° (graden, decimaal)  
Bereik φ tussen 50.6 en 56

Bereik λ tussen 2.4 en 7.4

### *Cirkel*

Het domein van het type *cirkel* wordt gebruikt voor een gebied op aarde dat als
een cirkel wordt voorgesteld en wordt gedefinieerd door een middelpunt en een
straal.  
Het middelpunt is een punt op het aardoppervlak en wordt uitgedrukt in het
domein *Coördinatenpaar* (zie de catalogus) met als referentiestelsel ETRS89
(ongeprojecteerd).

De straal is de geodetische afstand van het middelpunt tot een punt op de cirkel
en wordt uitgedrukt als een *getalswaarde* (zie de catalogus).

### *Getalswaardeinterval*

Een domein van het type *getalswaardeinterval* omvat een bepaald deel van een
bepaalde verzameling getallen. Binnen de BRO zijn drie verzamelingen getallen
van belang de natuurlijke, de gehele, en de rationale getallen. Het
getalswaardeinterval kent een onder- en een bovengrens en ook de beide
grensgetallen maken deel uit van de verzameling.

Een domein van het type getalswaardeinterval wordt in de BRO gebruikt voor
gegevens die gemeten, berekend of anderszins bepaald zijn. Bij de getalswaarde
hoort daarom een eenheid. De BRO gebruikt voor de eenheden de codes uit het UCUM
(Unified Code for Units of Measure)-systeem. In bijzondere gevallen is de
eenheid dimensieloos.

Wanneer een attribuut een domein van het type getalswaardinterval heeft worden
de minimale waarde voor de ondergrens (minimum) en de maximale waarde voor de
bovengrens van het interval (maximum) opgegeven, wordt gespecificeerd of het
gehele of rationale getallen betreft, en wordt de eenheid waarop de
getalswaarden betrekking hebben opgegeven.

### *Datuminterval*

Het *datuminterval* is een van de drie domeinen die voor gegevens die over een
interval in de tijd, een periode, gaan. Het domein wordt gebruikt voor een
periode die tot op de dag nauwkeurig begrensd is. Het domein *datuminterval*
bestaat uit een begindatum en een einddatum, beide van het domeintype *Datum*
(JJJJ-MM-DD, zie de catalogus).

De basisregistratie ondergrond hanteert de volgende praktische regels:

-   Het begin ligt voor het einde of valt daarmee samen.

-   Het waardebereik is inclusief en omvat de begin- en de einddatum

-   Een aanvullende regel is nodig om aan te geven wanneer een temporeel gegeven
    uit het domein OnvolledigeDatum in het interval ligt, en wanneer niet. Om
    die regel te formuleren wordt een OnvolledigeDatum beschouwd als een
    interval.

    -   Een OnvolledigeDatum valt alleen binnen het bereik van een datuminterval
        wanneer het interval in zijn geheel binnen het datuminterval valt (of
        daarmee samenvalt).

    -   Gegevens met de waarde onbekend worden niet uitgegeven o.b.v. een
        datuminterval.

        1.  *Kenmerkfout*

Een waarde in de lijst is een zin met een bepaalde opbouw en met zowel vaste als
variabele bestanddelen. De variabele bestanddelen gegeven aan waar de fout in de
kenmerkenverzameling zit en eventueel waarom het een fout is.

Een eerste variabel element is \<gegeven\>. Dat geeft aan welk gegeven onjuist
is. Wanneer het gaat om een onjuiste waarde wordt met het gegeven ook de waarde
van het gegeven opgenomen (\<gegeven = waarde\>).

Een tweede variabel element is \<referentiegegeven\> en dat wordt opgenomen
wanneer er een tweede gegeven is dat bepaalt dat het \<gegeven\> fout is. Zo
nodig wordt ook hier de waarde meegegeven (\<referentiegegeven = waarde\>).

Een derde variabel element is \<referentiewaarde\> en dat wordt opgenomen
wanneer een waardebereik bepaalt dat het \<gegeven\> fout is.

| *GEGEVEN ONTBREEKT*                                                                                    |
|--------------------------------------------------------------------------------------------------------|
| \<gegeven\> ontbreekt: het moet aanwezig zijn als \<referentiegegeven\> ontbreekt.                     |
| *GEGEVEN MAG NIET AANWEZIG ZIJN*                                                                       |
| \<gegeven\> mag niet aanwezig zijn: als \<referentiegegeven\> aanwezig is.                             |
| *WAARDE ONTBREEKT*                                                                                     |
| \<gegeven\> waarde ontbreekt.                                                                          |
| *WAARDE HEEFT GEEN CORRECT FORMAAT*                                                                    |
| \<gegeven = waarde\> waarde heeft geen correct formaat: moet zijn \<referentiewaarde\>.                |
| *WAARDE IS NIET CORRECT*                                                                               |
| \<gegeven = waarde\> waarde is niet correct: komt niet voor in de codelijst.                           |
| \<gegeven = waarde\> waarde is niet correct: moet gelijk zijn aan \<referentiewaarde\>.                |
| \<gegeven = waarde\> waarde is niet correct: zuidwesthoek ligt niet goed t.o.v. de noordoosthoek.      |
| \<gegeven = waarde\> waarde is niet correct: mag niet kleiner zijn dan \<referentiewaarde\>.           |
| \<gegeven = waarde\> waarde is niet correct: mag niet groter zijn dan \<referentiewaarde\>.            |
| \<gegeven = waarde\> waarde is niet correct: mag niet kleiner zijn dan \<referentiegegeven = waarde\>. |
| \<gegeven = waarde\> waarde is niet correct: mag niet voor \<referentiewaarde\> liggen.                |
| \<gegeven = waarde\> waarde is niet correct: mag niet voor \<referentiegegeven = waarde\> liggen.      |
| \<gegeven = waarde\> waarde is niet correct: mag niet in de toekomst liggen.                           |

### *RedenAfwijzing*

Net als bij het domein Kenmerkfout is een waarde een zin met een bepaalde opbouw
die vaste en variabele bestanddelen heeft.

| Waarde                                                                                                            |
|-------------------------------------------------------------------------------------------------------------------|
| \<gegeven\> waarde ontbreekt.                                                                                     |
| \<gegeven = waarde\> waarde heeft geen correct formaat: moet zijn \<referentiewaarde\>.                           |
| \<gegeven = waarde\> waarde heeft geen correct formaat: voldoet niet aan de MES 1 karakterset.                    |
| \<gegeven = waarde\> waarde is niet correct: komt niet voor in de codelijst.                                      |
| dit registratieobject bestaat niet.                                                                               |
| er zijn 1 of meer fouten geconstateerd in de kenmerkenverzameling.                                                |
| het aantal uitgiftedocumenten is groter dan 2000. Pas de kenmerken van uw verzoek tot verzending kengegevens aan. |

### *TeLeverenGegevens*

| Waarde            | Omschrijving                                                                                                                    |
|-------------------|---------------------------------------------------------------------------------------------------------------------------------|
| actueel           | De actuele gegevens , d.w.z. de gegevens die de toestand van de grondwatermonitoringput beschrijven op het moment van uitgifte. |
| actueelHistorisch | De actuele en historische gegevens van de grondwatermonitoringput.                                                              |

### *Uitgiftedocumenttype*

| Waarde     | Omschrijving                                                                                                                                                                           |
|------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| BRO-DO     | Het uitgiftedocument dat de gegevens van een object dat uit registratie is genomen bevat.                                                                                              |
| GMW-C      | Het uitgiftedocument dat de kengegevens van een grondwatermonitoringput die niet uit registratie is genomen bevat.                                                                     |
| GMW-PO     | Het uitgiftedocument dat de actuele gegevens van een grondwatermonitoringput die niet uit registratie is genomen bevat die voor een standaard afnemer beschikbaar zijn.                |
| GMW-PO-DP  | Het uitgiftedocument dat de actuele gegevens van een grondwatermonitoringput bevat die voor dataleverancier en bronhouder beschikbaar zijn.                                            |
| GMW-PPO    | Het uitgiftedocument dat chronologisch geordend de gegevens van een grondwatermonitoringput die niet uit registratie is genomen bevat die voor een standaard afnemer beschikbaar zijn. |
| GMW-PPO-DP | Het uitgiftedocument dat chronologisch geordend de gegevens van een grondwatermonitoringput bevat die voor dataleverancier en bronhouder beschikbaar zijn.                             |

1.  Uitgiftedocumenten

    1.  *BRO-DO*

![](media/381f00927be076bf93b3b51daca4eced.emf)

### *GMW-C*

![](media/ca46ff2b4a48873750f3b81266e5046e.emf)

| **Diameterbereik**                      |                                                                                                               |
|-----------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Naam entiteit                           | Diameterbereik                                                                                                |
| Definitie                               | Het interval dat de grenzen aangeeft waarbinnen de diameters van de bovenkant van de monitoringbuizen liggen. |
| Kardinaliteit                           | 1                                                                                                             |
|                                         |                                                                                                               |
| **kleinste diameter bovenkant buis**    |                                                                                                               |
| Naam attribuut                          | kleinste diameter bovenkant buis                                                                              |
| Definitie                               | De diameter van de bovenkant van de dunste buis in de grondwatermonitoringput.                                |
| Domein                                  | Getalswaardeinterval                                                                                          |
| Maximale lengte                         | 4                                                                                                             |
| Eenheid                                 | mm (millimeter)                                                                                               |
| Waardebereik                            | 3 tot 1000                                                                                                    |
|                                         |                                                                                                               |
| **grootste diameter bovenkant buis**    |                                                                                                               |
| Naam attribuut                          | grootste diameter bovenkant buis                                                                              |
| Definitie                               | De diameter van de bovenkant van de dikste monitoringbuis in de grondwatermonitoringput.                      |
| Domein                                  | Getalswaardeinterval                                                                                          |
| Maximale lengte                         | 4                                                                                                             |
| Eenheid                                 | mm (millimeter)                                                                                               |
| Waardebereik                            | 3 tot 1000                                                                                                    |
|                                         |                                                                                                               |
| **Statusoverzicht**                     |                                                                                                               |
| Naam entiteit                           | Statusoverzicht                                                                                               |
| Definitie                               | De in een grondwatermonitoringput voorkomende buisstatussen                                                   |
| Toelichting                             | Elke voorkomende buisstatus in de grondwatermonitoringput wordt maximaal één keer uitgegeven.                 |
|                                         |                                                                                                               |
| **Filterbereik**                        |                                                                                                               |
| Naam entiteit                           | Filterbereik                                                                                                  |
| Definitie                               | Het interval dat de grenzen aangeeft waarbinnen de verticale posities van de filters liggen.                  |
|                                         |                                                                                                               |
| **positie bovenkant ondiepste filter**  |                                                                                                               |
| Naam attribuut                          | positie bovenkant ondiepste filter                                                                            |
| Definitie                               | De positie van de bovenkant van het meest ondiepe filter                                                      |
| Domein                                  | Getalswaarde                                                                                                  |
| Maximale lengte                         | 3.3                                                                                                           |
| Eenheid                                 | m (meter)                                                                                                     |
| Waardebereik                            | \-750 tot 325                                                                                                 |
|                                         |                                                                                                               |
| **positie onderkant diepste filter**    |                                                                                                               |
| Naam attribuut                          | positie onderkant diepste filter                                                                              |
| Definitie                               | De positie van de onderkant van het meest diepe filter                                                        |
| Domein                                  | Getalswaarde                                                                                                  |
| Maximale lengte                         | 3.3                                                                                                           |
| Eenheid                                 | m (meter)                                                                                                     |
| Waardebereik                            | \-750 tot 325                                                                                                 |
|                                         |                                                                                                               |
| **Elektrodebereik**                     |                                                                                                               |
| Naam entiteit                           | Elektrodebereik                                                                                               |
| Definitie                               | Het interval dat de grenzen aangeeft waarbinnen de verticale posities van de elektroden liggen.               |
|                                         |                                                                                                               |
| **positie ondiepste elektrode**         |                                                                                                               |
| Naam attribuut                          | positie ondiepste elektrode                                                                                   |
| Definitie                               | De positie van de meest ondiepe elektrode                                                                     |
| Domein                                  | Getalswaarde                                                                                                  |
| Maximale lengte                         | 3.3                                                                                                           |
| Eenheid                                 | m (meter)                                                                                                     |
| Waardebereik                            | \-200 tot 50                                                                                                  |
|                                         |                                                                                                               |
| **positie onderkant diepste elektrode** |                                                                                                               |
| Naam attribuut                          | positie diepste elektrode                                                                                     |
| Definitie                               | De positie van de meest diepe elektrode                                                                       |
| Domein                                  | Getalswaarde                                                                                                  |
| Maximale lengte                         | 3.3                                                                                                           |
| Eenheid                                 | m (meter)                                                                                                     |
| Waardebereik                            | \-200 tot 50                                                                                                  |

### *GMW-PO*

Zie figuur 6.

### *GMW-PO-DP*

Het verschil met *GMW-PO* is dat het uitgiftedocument ook de gegevens *object-ID
bronhouder, dataleverancier* en *onderhoudende instantie* bevat.

### *GMW-PPO*

Zie figuur 7.

| **Resultaat gebeurtenis** |                                                                                                                                       |
|---------------------------|---------------------------------------------------------------------------------------------------------------------------------------|
| Naam entiteit             | Resultaat gebeurtenis                                                                                                                 |
| Definitie                 | De gegevens die als gevolg van een bepaalde tussentijdse gebeurtenis een nieuwe waarde hebben gekregen.                               |
| Kardinaliteit             | 1                                                                                                                                     |
|                           |                                                                                                                                       |
| **Putgegevens**           |                                                                                                                                       |
| Naam entiteit             | Putgegevens                                                                                                                           |
| Definitie                 | De gegevens die als gevolg van een bepaalde tussentijdse gebeurtenis voor de put als geheel een nieuwe waarde hebben gekregen.        |
| Kardinaliteit             | 0..1                                                                                                                                  |
|                           |                                                                                                                                       |
| **Buisgegevens**          |                                                                                                                                       |
| Naam entiteit             | Buisgegevens                                                                                                                          |
| Definitie                 | De gegevens die als gevolg van een bepaalde tussentijdse gebeurtenis voor een specifieke buis een nieuwe waarde hebben gekregen.      |
| Kardinaliteit             | 0..1                                                                                                                                  |
|                           |                                                                                                                                       |
| **Elektrodegegevens**     |                                                                                                                                       |
| Naam entiteit             | Elektrodegegevens                                                                                                                     |
| Definitie                 | De gegevens die als gevolg van een bepaalde tussentijdse gebeurtenis voor een specifieke elektrode een nieuwe waarde hebben gekregen. |
| Kardinaliteit             | 0..1                                                                                                                                  |

### *GMW-PPO-DP*

Het verschil met *GMW-PPO* is dat het uitgiftedocument ook de gegevens
*object-ID bronhouder, dataleverancier* en *onderhoudende instantie* bevat.

![](media/b0152ba3da8b35488cc3e28136284f81.emf)

*Figuur 6: Uitgiftedocument GMW-PO.*

![](media/5c14e920fd79eec1b7e5e9c5a22641ab.emf)

*Figuur 7: Uitgiftedocument GMW-PPO.*
