Basisregistratie Ondergrond (BRO) Innamehandboek

Grondwatermonitoringput

**Colofon**

|                  | Bestuurskern                         |
|------------------|--------------------------------------|
|                  | Dir. Ruimtelijke Ontwikkeling        |
|                  |                                      |
|                  | Rijnstraat 8 2515 XP Den Haag        |
|                  |                                      |
| Algemeen contact | Programmabureau BRO                  |
|                  | Directoraat-Generaal Ruimte en Water |
|                  | bro\@minienm.nl                      |
|                  |                                      |
|                  |                                      |
| Versie           |                                      |
|                  |                                      |
| Auteur           | TNO Geologische Dienst Nederland     |
|                  |                                      |

1.  Inleiding

    1.  Doel en doelgroep

In de basisregistratie ondergrond (BRO) wordt een aantal typen gegevens
geregistreerd, de *registratieobjecten*. Een van de registratieobjecten is de
*grondwatermonitoringput*.

Het innamehandboek richt zich op de partijen die grondwatermonitoringput aan de
registerbeheerder van de BRO aanbieden en beschrijft hoe het proces van
gegevensinname globaal verloopt.

Het doel is de leveranciers van gegevens, de dataleveranciers, in algemeen
begrijpelijke bewoordingen inzicht te geven in de stappen die in dit proces
worden doorlopen, in de begrippenwereld die wordt gehanteerd, in de vormen van
controle en in de berichten die tussen de leverancier en de registerbeheerder
worden uitgewisseld.

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

![](media/acb49344109773d4e205475f3cd7c396.png)

*Figuur 1: Samenhang van de documentatie.*

Leeswijzer
----------

Hoofdstuk 1 geeft het doel en de doelgroep, de samenhang met andere documenten
en de versiehistorie van dit innamehandboek.

Hoofdstuk 2 geeft een inleiding op de inname van gegevens van de
grondwatermonitoringput en gaat in op de verwerking van verzoeken.

Hoofdstuk 3 gaat in op de berichten die bij de inname van nieuwe gegevens, het
*registreren*, worden uitgewisseld. Het hoofdstuk vertelt onder meer welke
gegevens een dataleverancier moet meesturen met een brondocument en welke
gegevens hij terug kan verwachten als antwoord.

Hoofdstuk 4 gaat in op de berichten die bij de inname van verbeterde gegevens,
het *corrigeren*, worden uitgewisseld.

Hoofdstuk 5 geeft de specificatie van de berichten en brondocumenten.

Versiehistorie 
---------------

| Versie    | Datum           | Omschrijving                                                                                                                                                                     |
|-----------|-----------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| concepten | September 2016  | Interne versies                                                                                                                                                                  |
| 0.7       | 17 oktober 2016 | Versie voor de eerste ketentest.                                                                                                                                                 |
| 0.9       | 13 juni 2017    | Versie met verwerking van het commentaar uit de ketentest en de gevolgen van de consolidatie van het systeem, die aansluit op de catalogus Grondwater-monitoringput versie 0.91. |
| 1.0       | 28 juni 2017    | Versie vastgesteld door het Ministerie van Infrastructuur en Milieu.                                                                                                             |

Contactinformatie 
------------------

Voor vragen, suggesties of opmerkingen over de inhoud van dit document kunt u
contact opnemen met de servicedesk van de beheerder van de basisregistratie
ondergrond via <info@basisregistratieondergrond.nl>.

1.  Inname via de webservice

    1.  Gegevens aanbieden

De basisregistratie ondergrond is een systeem dat een schakel vormt in een
informatieketen. Aan het begin van de keten staan bestuursorganen die opdracht
geven tot de productie van gegevens, of zelf gegevens produceren. Die
bestuursorganen worden *bronhouders* genoemd. De geproduceerde gegevens worden
door een *dataleverancier* geleverd aan de beheerder van het systeem, de
*registerbeheerder*. De bronhouder is verantwoordelijk voor de levering van
gegevens. Hij kan besluiten zelf dataleverancier te zijn of andere partijen een
machtiging voor levering te verlenen. De beheerder van de BRO registreert de
aangeleverde gegevens en levert ze voor (her)gebruik door aan allerlei afnemers.

Een organisatie kan niet zomaar gegevens aan de BRO aanbieden. Een organisatie
moet zich eerst als *dataleverancier* bij de registerbeheerder hebben laten
registreren en de registratie is gekoppeld aan een bepaald type
registratieobject. Om de grondwatermonitoringput aan te mogen bieden moet een
organisatie zich als *dataleverancier van de grondwatermonitoringput* laten
registreren.

Wanneer het om een bronhouder gaat die zelf gegevens wil aanbieden, is er sprake
van een bilaterale overeenkomst en kan de bronhouder zich direct als
dataleverancier laten registreren. Wanneer een intermediaire partij namens een
bronhouder gegevens wil aanleveren, is sprake van een overeenkomst tussen drie
partijen.

De gegevens van de grondwatermonitoringput worden altijd via de
*innamewebservice* aangeboden. De dataleverancier die de innamewebservice wil
gebruiken moet over software beschikken die de webservice kan aanroepen. Met de
eigen software heeft hij dan direct toegang tot het systeem van de
basisregistratie ondergrond, het BRO-systeem, en kan hij snel en op betrouwbare
wijze gegevens aanbieden.

Om zich bij de registerbeheerder als gebruiker van de webservice te laten
registreren, moet de organisatie van de dataleverancier beschikken over een
*PKIoverheid services certificaat*.

De gegevens die via de innamewebservice aan de BRO worden overgedragen staan in
het IMBRO-XML formaat. Het IMBRO-XML formaat is de gegevensdefinitie omgezet
naar de technische taal die voor de uitwisseling van gegevens met het systeem
van de BRO gebruikt wordt. De technische uitwerking wordt toegelicht in de
koppelvlakbeschrijving van de innamewebservice.

Communicatie tussen twee systemen
---------------------------------

De dataleverancier die voor het aanbieden van gegevens van de
grondwatermonitoringput gebruik maakt van de innamewebservice, gebruikt via zijn
eigen systeem algemene BRO-software die via het internet voor iedereen te vinden
is.

Het adres van de BRO-webservices is te vinden op
[www.broinfo.nl](http://www.broinfo.nl).

De webservice zorgt ervoor dat het systeem van de data-leverancier een verzoek
tot het innemen van gegevens aan het BRO-systeem kan aanbieden, zorgt voor de
verwerking van het verzoek en geeft het resultaat daarvan als antwoord van de
BRO terug aan het systeem van de dataleverancier (Figuur 2).

![](media/910c23055508f9ca01607ee4870ec8bd.png)

*Figuur 2: De webservice zorgt voor communicatie tussen twee systemen.*

Innameverzoek 
--------------

De dataleverancier biedt gegevens aan met het doel de gegevens op te laten nemen
in de registratie ondergrond. Het proces van inname begint aan de kant van de
dataleverancier met een verzoek. Vervolgens beoordeelt de basisregistratie
ondergrond dat verzoek om, als alles goed is, de gegevens in het systeem op te
nemen. Gaat er iets onverhoopt fout, dan wijst de basisregistratie ondergrond
het verzoek af. In alle gevallen krijgt de dataleverancier een antwoord op het
verzoek terug.

De basisregistratie ondergrond handelt de verzoeken altijd per object af. Dat
wil zeggen één grondwatermonitoringput tegelijk. Het begrip *innameverzoek*
heeft in de context van de basisregistratie ondergrond altijd betrekking op één
grondwatermonitoringput.

De gegevens die onderwerp zijn van een innameverzoek, vormen een geheel en dat
wordt in de taal van de basisregistratie ondergrond een *brondocument* genoemd.
Een brondocument bevat de gegevens die de dataleverancier van een bepaald object
overdraagt aan de basisregistratie ondergrond.

Er bestaan twee categorieën innameverzoeken. Het hangt er namelijk vanaf wat de
dataleverancier precies beoogt.

Wil een leverancier nieuwe gegevens aan de BRO overdragen die net beschikbaar
zijn gekomen, of wil hij fouten verbeteren in de gegevens die al aanwezig zijn.
In de basisregistratie ondergrond spreekt men van *registratieverzoeken,* resp.
*correctieverzoeken*.

De verwerking van registratieverzoeken verloopt anders dan van
correctieverzoeken.

Via een innameverzoek kan een dataleverancier niet alle gegevens van een
registratieobject laten verwijderen. Verwijderen, of beter het *uit registratie
nemen* van een object is een ingrijpende verandering in de registratie
ondergrond, en daartoe kan pas worden besloten na zorgvuldig onderzoek. Het
onderzoek begint bij de registratiebeheerder en uiteindelijk kan een object
alleen na akkoord van de bronhouder uit registratie genomen worden. Het is
bovendien goed om te weten dat de gegevens niet uit de registratie verwijderd
worden. De gegevens blijven bestaan maar zijn niet langer voor gebruikers
toegankelijk.

Verwerking van een registratieverzoek 
--------------------------------------

De verwerking van een registratieverzoek verloopt geheel automatisch en volgens
een vaste opeenvolging van stappen. Dit is waar het in het kort op neerkomt:

1.  De dataleverancier stuurt vanuit zijn systeem een registratieverzoek met
    daarin een brondocument.

2.  Het systeem van de BRO voert een toegangscontrole uit.

3.  Wanneer toegang tot het systeem van de BRO is verkregen, begint de controle
    van het verzoek en wordt onder meer vastgesteld of het verzoek inhoudelijk
    aan de gestelde eisen voldoet.

    -   Wanneer de inhoudelijke controle fouten oplevert, wordt het verzoek
        afgewezen en ontvangt het systeem van de dataleverancier een bericht van
        afwijzing.

4.  Wanneer de inhoudelijke controle geen fouten oplevert en er geen technische
    problemen zijn, wordt het registratieverzoek door het systeem van de BRO
    geaccepteerd. De aangeboden gegevens worden met de gegevens die de BRO zelf
    genereert vastgelegd. Het BRO-systeem stuurt het systeem van de
    dataleverancier als antwoord het bericht dat diens registratieverzoek is
    verwerkt.

![](media/a955f2db86328655386bb4d9c9fa8a05.png)

De stappen en de bijbehorende berichten worden in het onderstaande plaatje
uitgebeeld.

*Figuur 3: Verwerking van een registratieverzoek.*

Het resultaat van de verwerking is dat het brondocument in het *register
brondocumenten ondergrond* is opgenomen, dat de gegevens eruit zijn gehaald en
vastgelegd zijn in de *registratie ondergrond*. De gegevens zijn dan voor
eenieder beschikbaar.

Het verzoek van de dataleverancier en het antwoord dat de BRO daarop normaliter
geeft worden *berichten* genoemd. In het geval zich technische problemen
voordoen wordt het antwoord een *melding* genoemd.

Verwerking van een correctieverzoek 
------------------------------------

De verwerking van een correctieverzoek verloopt iets anders dan dat van een
registratieverzoek. De eerste stappen in de verwerking zijn hetzelfde, maar
nadat het BRO-systeem heeft gecontroleerd of alles goed is, neemt de
registratiebeheerder de controle over.

Dit is waar het in het kort op neerkomt:

1.  De dataleverancier stuurt vanuit zijn systeem een correctieverzoek met
    daarin een brondocument.

2.  Het systeem van de BRO voert een toegangscontrole uit.

3.  Wanneer toegang tot het systeem van de BRO is verkregen, begint de controle
    van het verzoek en wordt onder meer vastgesteld of het verzoek inhoudelijk
    aan de gestelde eisen voldoet.

    -   Wanneer de inhoudelijke controle fouten oplevert, wordt het verzoek
        afgewezen en ontvangt het systeem van de dataleverancier een bericht van
        afwijzing.

4.  Wanneer de inhoudelijke controle geen fouten oplevert en er geen technische
    problemen zijn, wordt het correctieverzoek door het systeem van de BRO
    geaccepteerd. Vervolgens neemt de registratiebeheerder de verwerking over.
    Hij beoordeelt de reden van het correctieverzoek en de gevolgen die het
    heeft voor de informatie in de registratie ondergrond .

    -   Indien zijn beoordeling aangeeft dat er iets fout gaat, ontvangt de
        dataleverancier een e-mail waarin de registratiebeheerder toelicht
        waarom hij het verzoek heeft moeten afwijzen.

5.  Wanneer de registratiebeheerder geen problemen ziet, wordt het verzoek
    doorgeleid. De aangeboden gegevens worden, met de gegevens die de BRO zelf
    genereert, vastgelegd. Het BRO-systeem stuurt de dataleverancier per e-mail
    bericht dat het correctieverzoek is verwerkt.

Het resultaat van de verwerking is dat het brondocument in het register
brondocumenten ondergrond is opgenomen, dat de gegevens eruit zijn gehaald en
dat de onjuiste gegevens in de registratie ondergrond zijn verbeterd. De
gegevens zijn dan voor eenieder beschikbaar.

De stappen en de bijbehorende berichten worden in figuur 4 uitgebeeld.

![](media/698da30b1197275bc171354b7faf38c1.png)

*Figuur 4: Verwerking van een correctieverzoek.*

Object met een levensloop
-------------------------

De grondwatermonitoringput is een object dat voor langere tijd in de
werkelijkheid bestaat en tijdens zijn bestaan kunnen veranderingen optreden die
geregistreerd moeten worden in de basisregistratie ondergrond. In de taal van de
basisregistraties is een grondwatermonitoringput een object met een materiële
geschiedenis.

Registratie van de gegevens van een grondwatermonitoringput is dus geen
eenmalige gebeurtenis, maar een proces dat zo lang duurt als de put bestaat. Het
heeft een begin en een eind, en wanneer zich tussentijds een relevante
verandering voordoet, wordt de registratie weer opgepakt en worden de nieuwe
gegevens aangeboden.

De gegevens over de gebeurtenissen in het leven van een grondwatermonitoringput,
worden zo snel mogelijk in de registratie ondergrond geregistreerd. Welke
gegevens dat zijn hangt af van de gebeurtenis.

Zodra de constructie van de put voltooid is en de gegevens door of voor de
bronhouder zijn vastgelegd, kan het registreren van gegevens beginnen. Bij het
begin van de registratie biedt de dataleverancier een brondocument aan dat alle
gegevens bevat die de put beschrijven; dat brondocument heet *GMW-Inrichten*.
Wanneer het proces van registratie vervolgd wordt omdat zich in de werkelijkheid
een bepaalde gebeurtenis heeft voorgedaan, biedt de dataleverancier de nieuwe
gegevens ter registratie aan. Dit wordt zolang de put bestaat het aanvullen van
de registratie genoemd. Het registratieproces eindigt wanneer geregistreerd is
dat de put is opgeruimd, wat wil zeggen dat de put niet langer bestaat. Bij
aanvullen heeft de dataleverancier de keuze uit elf verschillende
brondocumenten. Het brondocument dat bij het opruimen van de put hoort heet
*GMW-Opruimen*.

De verschillende typen brondocumenten worden allemaal via dezelfde webservice
aangeboden, maar de gegevens verschillen en de controles die bij de verwerking
van de gegevens worden uitgevoerd ook. Na het beëindigen van de registratie
kunnen geen nieuwe gegevens meer worden aangeleverd. Wel kunnen er onjuistheden
worden hersteld.

Voor het verbeteren van onjuistheden in de geregistreerde gegevens van een
grondwatermonitoringput zijn verschillende typen verzoeken nodig. Dat komt
doordat de verschillende registratieverzoeken elkaar netjes moeten opvolgen in
de tijd om de materiële geschiedenis van de put in de registratie ondergrond
correct op te bouwen. Een dataleverancier kan zich op allerlei manieren
vergissen. Hij kan onjuiste gegevens aanleveren, maar ook vergeten een verzoek
op tijd aan te bieden of een fout maken in een datum die in het brondocument
staat.

Er worden vier typen correctieverzoeken onderscheiden en dat zijn:

-   het verzoek gegevens te vervangen,

-   het verzoek gegevens in te voegen,

-   het verzoek gegevens te verwijderen,

-   het verzoek gegevens te verplaatsen.

De verschillende typen correctieverzoeken worden net als de registratieverzoeken
via de innamewebservice aangeboden en de gegevens en controles verschillen per
type verzoek.

Twee kwaliteitsregimes
----------------------

De basisregistratie ondergrond stelt stringente eisen aan de gegevens van
registratieobjecten. Er zijn echter veel gegevens van vóór de datum waarop de
wet in werking is getreden. Die gegevens kunnen niet altijd aan dezelfde eisen
voldoen als gegevens die na de inwerkingtreding van de wet ontstaan. Omdat de al
bestaande gegevens waardevol zijn, heeft de wetgever besloten dat de
basisregistratie ook die gegevens moet bevatten. Zodoende kent de BRO twee
*kwaliteitsregimes* voor registratieobjecten:

1.  het kwaliteitsregime dat aangeeft dat een registratieobject aan de meest
    stringente eisen voldoet: IMBRO;

2.  het kwaliteitsregime dat aangeeft dat een registratieobject aan minder
    stringente eisen voldoet: IMBRO/A.

De objecten die zich naar de stringente regels voegen, zijn te herleiden tot een
brondocument met als kwaliteit IMBRO, en de andere tot een brondocument met als
kwaliteit IMBRO/A.

Om aansluiting op de BRO te vergemakkelijken is een periode van transitie
voorzien voor nieuw geconstrueerde putten. In de periode van transitie is de
aanlevering van het brondocument *GMW-Inrichten* in IMBRO en IMBRO/A toegestaan.
De duur van de transitie voor de grondwatermonitoringput is nog niet bepaald. Na
afloop van de transitieperiode mag alleen IMBRO worden aangeleverd.

Het kwaliteitsregime van het object grondwatermonitoringput wordt bepaald door
de kwaliteit van het brondocument dat bij het starten van registratie wordt
ingenomen.

Het kwaliteitsregime van een object kan veranderen, maar alleen na het
doorvoeren van een specifieke correctie. De noodzaak tot deze correctie zal zich
zeer zelden voordoen. Correctie van het kwaliteitsregime is namelijk alleen
mogelijk tijdens de periode van transitie en alleen voor nieuwe putten.

Conversie en putten met voorgeschiedenis
----------------------------------------

Het leven van een grondwatermonitoringput die ter registratie wordt aangeboden,
kan al ver voor het moment van aanbieden begonnen zijn. In sommige gevallen kan
de put in werkelijkheid al weer opgeruimd zijn. Een grondwatermonitoringput die
ver voor de datum van registratie is ingericht, wordt een *put met
voorgeschiedenis* genoemd.

Inname van putten met voorgeschiedenis verloopt eigenlijk hetzelfde als bij
nieuw geconstrueerde putten. De registratie start met het aanbieden van het
brondocument *GMW-Inrichten*, dan worden de gegevens aangevuld met zoveel
brondocumenten als nodig zijn, en ten slotte wordt de registratie beëindigd met
het aanbieden van het brondocument *GMW-Opruimen.*

De condities waaronder de inname verloopt zijn echter wel anders. Inname van
putten met voorgeschiedenis is nauw verbonden met conversie van gegevens uit
bestaande systemen. Zo zullen op het moment dat de wet basisregistratie
ondergrond in werking treedt de grondwatermonitoringputten uit het systeem DINO
in de BRO geregistreerd zijn als putten met voorgeschiedenis. Dat is een grote
conversie-operatie. Aan de DINO naar BRO-conversie gaat een proces van
zorgvuldige voorbereiding vooraf. De inname van putten met voorgeschiedenis is
opgezet vanuit de aanname dat soortgelijke conversieprojecten ook zullen worden
uitgevoerd met andere dataleveranciers.

De conversieprojecten worden zo opgezet dat de betreffende dataleverancier na
afloop geen historische gegevens voor de betreffende bronhouder meer kan
aanbieden. Andersom geldt dat er zolang de conversie niet voltooid is geen
gegevens van nieuwe putten kunnen worden aangeleverd.

Om de inname van putten met voorgeschiedenis gecontroleerd te kunnen laten
verlopen zullen heldere afspraken gemaakt worden tussen bronhouder,
dataleverancier en registerbeheerder. Die afspraken worden in de
basisregistratie vertaald naar een bijzonder recht. Het bijzondere recht geldt
voor bepaalde tijd en wordt *voorrecht* genoemd.

Bij het voorrecht hoort dat de dataleverancier brondocumenten

mag aanleveren die in een opzicht afwijken van het voor historische gegevens
algemeen geldende kwaliteitsregime IMBRO/A. De afwijking heeft betrekking op de
nauwkeurigheid waarmee de gebeurtenissen in het leven van de put wordt
vastgelegd. Voor putten met voorgeschiedenis gelden minder strikte regels en de
details worden later behandeld.

Registreren van gegevens
========================

Dit hoofdstuk behandelt eerst de berichten die bij de normale procesgang tussen
het systeem van de dataleverancier en het systeem van de basisregistratie
ondergrond worden uitgewisseld. De chronologie van het proces van registreren
wordt gevolgd door eerst het starten van de registratie te bespreken, dan het
aanvullen en daarna het beëindigen.

Aan het eind van het hoofdstuk worden de meldingen behandeld die de
dataleverancier krijgt, wanneer de normale procesgang wordt verstoord door
onvoorziene omstandigheden.

1.  Begin van het registratieproces

    1.  *Verzoek*

![cid:image001.png\@01D2EC00.8BF79760](media/4a3e388f166eb5b2e60c0c1fe3a428e5.png)

Zodra de constructie van de put voltooid is en alle gegevens door of voor de
bronhouder zijn vastgelegd, kan het registreren van gegevens beginnen. De
dataleverancier biedt dan een brondocument aan met de naam *GMW-Inrichten*.

Het brondocument is belangrijkste onderdeel van het registratieverzoek. Het
bevat alle gegevens die het object grondwatermonitoringput beschrijven op het
moment dat de constructie volledig is ingericht.

Met het brondocument moet de dataleverancier in zijn verzoek aangeven aan welk
*kwaliteitsregime* het brondocument voldoet, of hij het verzoek *onder
voorrecht* doet omdat het om een put met voorgeschiedenis gaat, en voor welke
*bronhouder* hij de gegevens aanbiedt. Dat laatste hoeft de dataleverancier
alleen op te geven als hij zelf niet de bronhouder van de gegevens is.

Tenslotte moet de dataleverancier het verzoek zelf een identificatie meegeven,
het *verzoekkenmerk*. Dat verzoekkenmerk is nodig in de communicatie,
bijvoorbeeld als er iets mis is gegaan en de dataleverancier daarover contact
wil zoeken met de servicedesk.

### *Bericht van afwijzing*

![](media/6f34fccad807b71ee59512aaf8c85eec.png)

In de verwerking van het verzoek zijn allerlei controles ingebouwd. Als er in
technische zin iets mis gaat, krijgt de dataleverancier geen bericht van
afwijzing maar een melding.

Een *bericht van afwijzing* krijgt de dataleverancier als antwoord, wanneer bij
de verwerking een fout wordt gevonden die het gevolg is van een invoerfout. Bij
het invoeren van de gegevens die met het brondocument worden meegegeven kan een
fout worden gemaakt, maar de in potentie grootste bron van fouten is het
brondocument zelf.

Het belangrijkste onderdeel van het bericht van afwijzing is de *reden
afwijzing*. Wanneer de reden van afwijzen in het brondocument ligt, wordt van
iedere fout vermeld:

-   bij welk gegeven de fout is geconstateerd,

-   soms ook wat de waarde van het gegeven is,

-   en wat de fout is.

Het bericht bevat verder het *tijdstip van afwijzing* en het *verzoekkenmerk*
van de dataleverancier, de eigen identificatie van het object die in het
brondocument is opgenomen (*object-ID bronhouder*) en het unieke kenmerk dat de
BRO zelf toekent (*transactie-ID*).

### [./media/image9.png](./media/image9.png)

*Bericht van registratie*

Wanneer de verwerking van het verzoek foutloos is verlopen, krijgt de
dataleverancier als antwoord een *bericht van registratie*.

Het belangrijkste gegeven in het bericht van registratie is het *BRO-ID*, de
identificatie van het object in de BRO die voortaan in het formele
berichtenverkeer moet worden gebruikt. De dataleverancier krijgt ook terug op
welk moment het object is geregistreerd.

Het bericht van registratie bevat verder, net als het bericht van afwijzing, het
*verzoekkenmerk* van de dataleverancier, het unieke kenmerk dat de BRO zelf
toekent en de eigen identificatie van het object.

Het belangrijkste resultaat van de verwerking is dat de grondwatermonitoringput
als object in de registratie ondergrond is opgenomen. Het object krijgt als
registratiestatus *geregistreerd*.

Gegevens aanvullen
------------------

Wanneer, na registratie van het brondocument *GMW-Inrichten*, er in de
werkelijkheid een gebeurtenis optreedt waarvan de gevolgen geregistreerd moeten
worden, wordt een verzoek aangeboden met een brondocument dat de nieuwe gegevens
bevat.

De aard van de gebeurtenis die in de werkelijkheid optreedt, kan verschillen. Er
zijn elf typen gebeurtenissen onderkend en bij iedere daarvan hoort een apart
type brondocument (tabel 1).

Eenzelfde type gebeurtenis kan meer keren optreden en een verzoek tot aanvullen
kan dan ook zo vaak als nodig worden aangeboden.

| Gebeurtenis                                                                                                                                        | Brondocument            |
|----------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------|
| De put is voorzien van een beschermconstructie of een al bestaande beschermconstructie is vervangen door een ander type.                           | GMW-Beschermconstructie |
| Van één of meer buizen is de toestand die aangeeft of zij gebruikt kan worden voor monitoring veranderd.                                           | GMW-Buisstatus          |
| Het eigendom van de grondwatermonitoringput is op een andere organisatie overgegaan.                                                               | GMW-Eigenaar            |
| Van één of meer elektrodes is toestand die aangeeft of zij gebruikt kan worden voor monitoring veranderd.                                          | GMW-Elektrodestatus     |
| Een of meer monitoringbuizen zijn korter gemaakt en dat kan gedaan zijn in combinatie met het aanbrengen of vervangen van een beschermconstructie. | GMW-Inkorten            |
| Er is een nieuw stijgbuisdeel in een bestaande monitoringbuis geplaatst.                                                                           | GMW-Inplaatsen          |
| De positie van het maaiveld is opnieuw vastgesteld.                                                                                                | GMW-Maaiveld            |
| Het uitvoeren van het onderhoud van de grondwatermonitoringput is op een andere partij overgegaan.                                                 | GMW-Onderhouder         |
| Een of meer monitoringbuizen zijn langer gemaakt en dat kan gedaan zijn in combinatie met het aanbrengen of vervangen van een beschermconstructie. | GMW-Oplengen            |
| De positie van het maaiveld en van de bovenkant van de buizen is opnieuw vastgesteld.                                                              | GMW-Posities            |
| De positie van het maaiveld is opnieuw vastgesteld omdat het terrein rond de put is opgehoogd of afgegraven.                                       | GMW-Verleggen           |

*Tabel 1: De gebeurtenissen die tussen het inrichten en opruimen in het leven
van een put kunnen optreden, met de naam van het bijbehorende brondocument.*

### [./media/image10.png](./media/image10.png)

*Verzoek*

Het registratieverzoek lijkt sterk op het verzoek dat bij het begin van de
registratie wordt aangeboden. De verschillen zijn dat de dataleverancier altijd
het *BRO-ID* meegeeft van het object waarvoor hij nieuwe gegevens aanbiedt bevat
en een ander type brondocument.

### [./media/image11.png](./media/image11.png)

*Bericht van afwijzing*

Het bericht van afwijzing dat de dataleverancier als antwoord krijgt wanneer bij
de verwerking een invoerfout in het verzoek wordt gevonden verschilt maar op een
punt van dat wat teruggegeven wordt bij het begin van de registratie. Het
verschil is dat het *BRO-ID* wordt teruggegeven in plaats van het *object-ID
bronhouder*.

De verwerking van het verzoek verloopt anders dan bij het starten van de
registratie in de zin dat er extra controles zijn ingebouwd. Die controles zijn
nodig omdat bij aanvulling beoordeeld moet worden of de gegevens passen bij wat
al van de put geregistreerd is. Dat betekent vooral dat bepaalde waarden
vergeleken moeten worden met al geregistreerde waarden. Enkele voorbeelden
moeten dat verduidelijken. Als de gebeurtenis inhoudt dat een bestaand gegeven
een andere waarde moet krijgen, dan moet de aangeboden waarde ook werkelijk
anders zijn: een nieuwe eigenaar is een andere eigenaar dan al geregistreerd is.
Een ander voorbeeld is dat de gebeurtenis ook moet passen in de tijdreeks die al
in de registratie ondergrond is opgebouwd. Gebeurtenissen moeten netjes in
volgorde worden aangeleverd. De registratie kan niet meer aangevuld worden als
de put is opgeruimd. Ten slotte moet ook in de registratie ondergrond gekeken
worden of dataleverancier als de leverancier van het betreffende object is
geregistreerd. De reden van afwijzing moet zo duidelijk verwoord zijn dat de
dataleverancier begrijpt wat er precies is fout gegaan.

### *Bericht van registratie*

![](media/dd3896ed998cb151c412458de46e597a.png)

Wanneer de verwerking van het verzoek foutloos is verlopen, krijgt de
dataleverancier weer als antwoord een *bericht van registratie*. Het enige
verschil met het antwoord dat hij helemaal aan het begin van de registratie
krijgt, is dat het *object-ID bronhouder* ontbreekt omdat het niet meer gebruikt
wordt in de communicatie.

Het belangrijkste resultaat van de verwerking is dat de gebeurtenis met de
bijbehorende gegevens in de registratie ondergrond is vastgelegd. De gebeurtenis
wordt als zodanig geregistreerd, daarbij krijgen een of meer attributen een
nieuwe waarde. Die waarde is geldig vanaf de datum van de gebeurtenis (datum
begin geldigheid). De eerder geregistreerde waarde blijft behouden, maar
verliest op de datum van de gebeurtenis zijn geldigheid (datum einde
geldigheid).

Na verwerking van het eerste vervolgverzoek krijgt het object de
registratiestatus *aangevuld*.

Eind van het registratieproces
------------------------------

Wanneer de put is opgeruimd, kan de registratie van het object beëindigd worden.
Het beëindigen van de registratie is eenmalig en het bijbehorende brondocument
heet *GMW-Opruimen*. Dat document vertelt eigenlijk alleen wanneer de put is
opgeruimd. In de verwerking zijn soortgelijke controles ingebouwd als bij
aanvullen en de berichten hebben dezelfde opbouw.

Wanneer de verwerking van het verzoek foutloos is verlopen, krijgt het object
als registratiestatus *voltooid*, en als gebeurtenis wordt geregistreerd dat de
put is opgeruimd. Vanaf dat moment kunnen er geen nieuwe gegevens meer worden
geregistreerd.

Meldingen
---------

Een melding is het antwoord dat de BRO stuurt wanneer er op technisch vlak iets
mis is gegaan. Meldingen zijn in eerste instantie bedoeld voor programmeurs. Om
die reden worden de meldingen uitgebreid behandeld in de koppelvlakbeschrijving;
hier wordt alleen wat achtergrondinformatie gegeven.

De oorzaak van een technisch probleem kan variëren en er worden drie categorieën
meldingen onderscheiden:

-   melding van een probleem bij de toegangscontrole,

-   melding van een probleem in de software van de dataleverancier,

-   melding van een systeemfout.

Toegangscontrole houdt in dat het systeem van de BRO controleert of de
dataleverancier daadwerkelijk is wie hij beweert te zijn en of hij het recht
heeft gebruik te maken van de innamewebservice. Het optreden van een probleem
bij de toegangscontrole is uitzonderlijk en het zal zich eigenlijk alleen
voordoen wanneer een dataleverancier voor het eerst gebruik wil maken van de
webservice.

Problemen in de software van de dataleverancier kunnen

vaker optreden, maar ook deze zullen zich in eerste instantie met name openbaren
in de fase waarin de dataleverancier bezig is zijn software geschikt te maken
voor aansluiting op de BRO.

Systeemfouten doen zich voor wanneer er problemen zijn met de software van de
BRO of wanneer zich onvoorziene omstandigheden voordoen, bijvoorbeeld wanneer de
stroomtoevoer hapert. Fouten in het systeem van de BRO kunnen verwacht worden in
de testfase. Wanneer het systeem in productie is genomen mogen ze eigenlijk niet
meer optreden. Gebeurt dat toch, dan alleen in de korte periode direct na
inproductiename. Onvoorziene omstandigheden kunnen zich daarentegen altijd
voordoen.

Corrigeren van gegevens
=======================

Dit hoofdstuk behandelt de verschillende typen van correctie die voor de
grondwatermonitoringput worden onderscheiden en de berichten die bij de normale
procesgang tussen het systeem van de dataleverancier en het de basisregistratie
ondergrond worden uitgewisseld. De meldingen die de dataleverancier krijgt,
wanneer de procesgang wordt verstoord door onvoorziene omstandigheden zijn
behandeld in paragraaf 3.4.

Vier typen correcties
---------------------

De registratie van de gegevens van een grondwatermonitoringput is zoals in de
voorgaande hoofdstukken verteld een proces dat op een bepaald moment begint en
op een bepaald moment eindigt. In de tussengelegen tijd kunnen zich in de
werkelijkheid allerlei gebeurtenissen voordoen, waarvan het resultaat moet
worden geregistreerd in de basisregistratie ondergrond. Iedere keer wanneer  
het resultaat van een gebeurtenis wordt geregistreerd, krijgen een of meer
gegevens in de registratie ondergrond een nieuwe waarde. De oude waarde blijft
behouden, maar die verliest zijn geldigheid op de datum waarop de gebeurtenis
heeft plaatsgevonden. Omdat een bepaald type gebeurtenis meermalen kan optreden,
kan een gegeven in de registratie ondergrond een reeks van waarden opbouwen,
waarbij iedere waarde gebonden is aan een bepaald tijdinterval. De geldigheid
van een waarde kent een begindatum en een einddatum.

Om de integriteit van de waardereeksen in de registratie ondergrond te kunnen
borgen, voert de basisregistratie ondergrond allerlei controles uit. Voor die
controles is het belangrijk te weten wat voor soort vergissing er in het
verleden is gemaakt. Daarom vraagt de basisregistratie ondergrond aan de
dataleveranciers in hun correctieverzoek te expliciteren wat de aard van de fout
is. Is de dataleverancier vergeten een bepaald brondocument op tijd aan te
leveren, en heeft hij inmiddels wel een andere gebeurtenis laten registreren,
dan spreekt de basisregistratie over een verzoek tot *invoegen*. Heeft de
dataleverancier een gebeurtenis laten registreren die nooit heeft
plaatsgevonden, dan spreekt de basisregistratie over een verzoek tot
*verwijderen*. Heeft de dataleverancier een gebeurtenis laten registreren met
een verkeerde datum dan spreekt de basisregistratie over een verzoek tot
*verplaatsen*. Heeft de dataleverancier een gebeurtenis laten registreren op de
juiste datum maar een fout gemaakt in een ander type gegeven, dan spreekt de
basisregistratie over een verzoek tot *vervangen.*

De verschillen tussen de berichten die worden uitgewisseld zijn klein. Het
belangrijkste verschil is dat de dataleveranciers moeten aangeven wat de aard
van de vergissing is. De inhoud van een brondocument wordt louter bepaald door
het type gebeurtenis en die is bij alle typen correcties precies hetzelfde als
bij registratie. In drie van de vier type correcties bevatten de berichten
dezelfde gegevens. Alleen een verzoek tot verwijderen bevat een extra gegeven.

Gezien de grote overeenkomst tussen de vier verschillende correcties, worden de
berichten die bij vervangen horen uitgebreid behandeld en worden van de drie
andere typen alleen de bijzonderheden besproken.

Vervangen
---------

Vervangen is een correctie die op geen enkele wijze iets verandert in de
materiële geschiedenis van een grondwatermonitoringput. Alle gebeurtenissen zijn
in de juiste volgorde en met de juiste datum geregistreerd. De dataleverancier
dient een verzoek tot vervangen in wanneer hij eerder een brondocument heeft
aangeleverd met daarin de goede datum van de gebeurtenis, maar met fouten in een
of meer van de andere gegevens.

### [./media/image13.png](./media/image13.png)

*Verzoek*

Het correctieverzoek bij vervangen heeft allereerst veel gegevens het gemeen met
een registratieverzoek dat nadat de registratie is begonnen worden aangeboden.
Dat zijn het verzoekkenmerk, de bronhouder, het brondocumenttype, het
kwaliteitsregime waaronder het brondocument valt, het BRO-ID van de put en het
gegeven dat aangeeft of het de correctie van een put met voorgeschiedenis
betreft (*onder voorrecht*). Naast deze gegevens bevat het correctieverzoek twee
nieuwe gegevens. Het eerste is de *correctiereden* het tweede het
*correctietype*. Dat laatste gegeven heeft in dit geval de waarde *vervangen*.
Het eerste geeft aan of de correctie op eigen initiatief wordt aangeboden of
omdat het object vanwege een terugmelding door de registerbeheerder in onderzoek
is geplaatst, of dat het kwaliteitsregime van de grondwatermonitoringput
verbeterd moet worden of de bronhouder van de gegevens.

Een verzoek tot vervangen kan alle brondocumenten bevatten, met uitzondering van
*GMW-Opruimen*. Dat document bevat namelijk alleen de datum van opruimen en die
vormt een element in de materiële geschiedenis.

### *Bericht van afwijzing*

Het bericht dat de dataleverancier als antwoord krijgt, wanneer bij de
verwerking een fout wordt gevonden die het gevolg is van een invoerfout, is
precies hetzelfde als bij een registratieverzoek dat bij het aanvullen van
gegevens wordt ingediend (zie 3.2.2). De controles zijn bijna hetzelfde als bij
het aanvullen van gegevens. Het verschil is dat er wat extra aspecten
gecontroleerd worden die met de reden van correctie samenhangen. Zo wordt
nagegaan of het object wel of niet in onderzoek is. Zolang een object in
onderzoek is kan een dataleverancier niet op eigen initiatief een
correctieverzoek aanbieden.

### *Bericht van acceptatie*

![](media/412cce1800421d5888740a467f78f793.png)

Het bericht van acceptatie bevat naast het verzoekkenmerk, het transactie-ID en
het BRO-ID, alleen het tijdstip van acceptatie.

### *Bericht van bezwaar*

![C:\\Users\\leeuwenrjwv\\AppData\\Local\\Microsoft\\Windows\\INetCache\\Content.Word\\Bericht van bezwaar (002).png](media/3cc6fb6b32ffce032a6ebc06a9cf16f7.png)

Het bericht van bezwaar ontvangt de dataleverancier per e-mail en komt van de
registratiebeheerder. In het e-mailbericht legt de registratiebeheerder uit
waarom hij het correctieverzoek heeft moeten afwijzen. Dat is de *reden
bezwaar*. De *reden bezwaar* kent geen vaste structuur. De registratiebeheerder
vult in wat nodig is om de dataleverancier goed te informeren voer wat er fout
is gegaan. De registratiebeheerder controleert onder meer of de tijdreeksen na
correctie de juiste opbouw houden vormen en of de correctie van een object in
onderzoek aansluit op de reden het onderzoek te starten.  
Naast de *reden bezwaar* bevat het bericht de gegevens die de basisregistratie
altijd in een antwoordbericht opneemt: het verzoekkenmerk, de transactie-ID, het
BRO-ID en een tijdstip, in dit geval het tijdstip waarop de registratiebeheerder
het verzoek heeft afgewezen.

### *Bericht van correctie*

![C:\\Users\\leeuwenrjwv\\AppData\\Local\\Microsoft\\Windows\\INetCache\\Content.Word\\Bericht van correctie (002).png](media/0a992cd3b749a4a5f12bd0c78b455e46.png)

Het bericht van correctie dat de dataleverancier krijgt bij succesvolle
verwerking van het verzoek is ook een e-mailbericht dat namens de
registratiebeheerder wordt verstuurd. De inhoud van zo’n bericht is
vergelijkbaar met het bericht van registratie dat verstuurd wordt bij
succesvolle verwerking van een registratieverzoek.

Invoegen
--------

Invoegen is een correctie die ingrijpt in de materiële geschiedenis van een
grondwatermonitoringput. Het gaat om de eenvoudigste variant, namelijk de
situatie waarin de dataleverancier vergeten was een gebeurtenis te registreren
terwijl hij intussen wel een andere gebeurtenis heeft laten registreren.

De berichten zijn hetzelfde als bij vervangen. Maar een verzoek tot invoegen kan
alleen de elf brondocumenten bevatten die betrekking hebben op een gebeurtenis
die tussen het inrichten en beëindigen van een grondwatermonitoringput ligt.

Verwijderen
-----------

Verwijderen is een correctie die ingrijpt in de materiële geschiedenis van een
grondwatermonitoringput. Het gaat om de situatie waarin de dataleverancier ten
onrechte een brondocument heeft aangeleverd. Om de fout te herstellen, levert de
dataleverancier het eerder aangeleverde brondocument nogmaals aan maar nu met
het verzoek de gegevens die erin staan uit de registratie te verwijderen.

De berichten zijn hetzelfde als bij vervangen. Een verzoek tot verwijderen kan
alle brondocumenten bevatten, met uitzondering van *GMW-Inrichten*. Verwijderen
van dat document zou betekenen dat het hele registratieobject wordt verwijderd
en dat is een transactie die niet via de webservice kan worden uitgevoerd.

Verplaatsen
-----------

Verplaatsen is een correctie die ingrijpt in de materiële geschiedenis van een
grondwatermonitoringput. Het gaat om de situatie waarin de dataleverancier de
juiste gegevens heeft aangeleverd maar met de verkeerde datum. Om de fout te
herstellen, levert de dataleverancier het brondocument nogmaals aan maar nu met
de juiste datum erin en met het verzoek de gegevens te verplaatsen. Om aan te
geven over welke gebeurtenis het precies gaat geeft hij de onjuiste datum mee in
zijn verzoek.

Een verzoek tot verplaatsen kan alle brondocumenten bevatten.

1.  Specificatie van berichten en brondocumenten

    1.  Inleiding

In dit hoofdstuk wordt de gegevensinhoud beschreven van de berichten die bij
inname worden uitgewisseld tussen de dataleverancier en de BRO. De systematiek
van de beschrijving is dezelfde als in de catalogus van de
grondwatermonitoringput.

Eerst worden de verzoeken en antwoorden beschreven die uitgewisseld worden
tussen het systeem van de dataleverancier en het BRO-systeem. Dat gebeurt op
basis van een model dat de vorm heeft van een UML-diagram. De modellen zijn zo
generiek mogelijk gemaakt omdat de specifieke aspecten al in het betreffende
hoofdstuk zijn behandeld.

Vervolgens worden voorbeelden gegeven van de e-mailberichten die de
basisregistratie ondergrond verstuurt. Dan wordt de inhoud van de codelijsten
behandeld en aan het eind van het hoofdstuk wordt het UML-diagram van het
brondocument gegeven.

Het handboek is een aanvulling op de catalogus. Een gegeven wordt hier alleen
gedefinieerd wanneer het daarin niet beschreven is of wanneer er bijzondere
regels gelden. Delen van de definitie van een gegeven die ongewijzigd zijn ten
opzichte van de catalogus zijn grijs gemaakt. Nieuwe gegevens die voorkomen bij
meerdere berichten worden eenmalig gedefinieerd. In lijn daarmee worden aan het
eind van het hoofdstuk de domeinen behandeld die specifiek zijn voor de
berichten.

1.  Berichten

    1.  *Registratieverzoek*

![](media/1871614364aa9b209c9b280c066d1a44.png)

| **verzoekkenmerk**   |                                                                                                                                                            |
|----------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Naam attribuut       | verzoekkenmerk                                                                                                                                             |
| Definitie            | Het kenmerk dat de gebruiker, in dit geval de dataleverancier, meegeeft om het verzoek te identificeren.                                                   |
| Kardinaliteit        | 1                                                                                                                                                          |
| Domein               | Tekst                                                                                                                                                      |
|   Maximale lengte    | 200                                                                                                                                                        |
|                      |                                                                                                                                                            |
| **bronhouder**       |                                                                                                                                                            |
| Naam attribuut       | bronhouder                                                                                                                                                 |
| Definitie            | De identificatie die het bestuursorgaan dat bronhouder is van de gegevens in de basisregistratie ondergrond als onderneming in het Handelsregister heeft.  |
| Kardinaliteit        | 0..1                                                                                                                                                       |
| Domein               | KvK-nummer                                                                                                                                                 |
|   Type               | Code                                                                                                                                                       |
|   Opbouw             | NNNNNNNN                                                                                                                                                   |
| Regels               | Het gegeven is aanwezig, tenzij de dataleverancier zelf bronhouder is en uit dien hoofde het verzoek indient.                                              |
|                      |                                                                                                                                                            |
| **brondocumenttype** |                                                                                                                                                            |
| Naam attribuut       | brondocumenttype                                                                                                                                           |
| Definitie            | De aanduiding van het type brondocument dat in het verzoek wordt aangeboden.                                                                               |
| Kardinaliteit        | 1                                                                                                                                                          |
| Domein               | Brondocumenttype                                                                                                                                           |
|   Type               | Codelijst                                                                                                                                                  |
|                      |                                                                                                                                                            |
| **kwaliteitsregime** |                                                                                                                                                            |
| Naam attribuut       | kwaliteitsregime                                                                                                                                           |
| Definitie            | De aanduiding van de kwaliteitseis waaraan de gegevens in het brondocument voldoen.                                                                        |
| Kardinaliteit        | 1                                                                                                                                                          |
| Domein               | Kwaliteitsregime                                                                                                                                           |
|   Type               | Enumeratie                                                                                                                                                 |
| Toelichting          | Het kwaliteitsregime van een registratieobject wordt vastgelegd bij de registratie van het brondocument *GMW-Inrichten*.                                   |
|                      |                                                                                                                                                            |
| **BRO-ID**           |                                                                                                                                                            |
| Naam attribuut       | BRO-ID                                                                                                                                                     |
| Definitie            | De identificatie van een object dat in de registratie ondergrond is opgenomen.                                                                             |
| Kardinaliteit        | 0..1                                                                                                                                                       |
| Domein               | Registratieobjectcode                                                                                                                                      |
|   Type               | Code                                                                                                                                                       |
|   Opbouw             | GMWNNNNNNNNNNNN                                                                                                                                            |
| Regels               | Het gegeven is aanwezig, tenzij het verzoek de registratie van het brondocument *GMW-Inrichten* betreft.                                                   |
|                      |                                                                                                                                                            |
| **onder voorrecht**  |                                                                                                                                                            |
| Naam attribuut       | onder voorrecht                                                                                                                                            |
| Definitie            | De aanduiding die aangeeft dat de dataleverancier het recht heeft gedurende een bepaalde tijd putten met voorgeschiedenis aan te leveren                   |
| Kardinaliteit        | 0..1                                                                                                                                                       |
| Domein               | IndicatieJaNee=ja                                                                                                                                          |
| Regels               | Het gegeven is aanwezig zolang het recht geldt.                                                                                                            |
| Toelichting          | Onder dit voorrecht mag een brondocument binnen bepaalde restricties een datum voor gebeurtenissen bevatten met een waarde uit het domein OnvolledigeDatum |

### *Correctieverzoek*

![](media/98e8682a7d0825bf428abe0414348275.png)

| **correctiereden**      |                                                                                                                                                                                                                                                                      |
|-------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Naam attribuut          | correctiereden                                                                                                                                                                                                                                                       |
| Definitie               | De reden voor de verbetering die de dataleverancier in de geregistreerde gegevens wil doorvoeren.                                                                                                                                                                    |
| Kardinaliteit           | 1                                                                                                                                                                                                                                                                    |
| Domein                  | Correctiereden                                                                                                                                                                                                                                                       |
| Type                    | Codelijst                                                                                                                                                                                                                                                            |
| Regels                  | De waarde *inOnderzoek* is alleen toegestaan wanneer het attribuut *in onderzoek* van de entiteit *Registratiegeschiedenis* in de registratie ondergrond de waarde *ja* heeft. De andere waarden zijn alleen toegestaan wanneer dat attribuut de waarde *nee* heeft. |
|                         |                                                                                                                                                                                                                                                                      |
| **correctietype**       |                                                                                                                                                                                                                                                                      |
| Naam attribuut          | correctietype                                                                                                                                                                                                                                                        |
| Definitie               | De aard van de verbetering die de dataleverancier wil doorvoeren in de geregistreerde gegevens.                                                                                                                                                                      |
| Kardinaliteit           | 1                                                                                                                                                                                                                                                                    |
| Domein                  | Correctietype                                                                                                                                                                                                                                                        |
| Type                    | Codelijst                                                                                                                                                                                                                                                            |
|                         |                                                                                                                                                                                                                                                                      |
| **te corrigeren datum** |                                                                                                                                                                                                                                                                      |
| Naam attribuut          | te corrigeren datum                                                                                                                                                                                                                                                  |
| Definitie               | De datum die moet worden verbeterd.                                                                                                                                                                                                                                  |
| Kardinaliteit           | 0..1                                                                                                                                                                                                                                                                 |
| Domein                  | Datum of OnvolledigeDatum                                                                                                                                                                                                                                            |
| Waardebereik            | 1 januari 1899 tot heden                                                                                                                                                                                                                                             |
| Regels                  | Het gegeven is alleen aanwezig wanneer de waarde van het attribuut correctietype gelijk is aan *Verplaatsen.*                                                                                                                                                        |
|                         |                                                                                                                                                                                                                                                                      |

### *Bericht van acceptatie*

![](media/fd8a4dcc7e74851c5b6ab847891474b1.png)

| **tijdstip van acceptatie** |                                                                                   |
|-----------------------------|-----------------------------------------------------------------------------------|
| Naam attribuut              | tijdstip van acceptatie                                                           |
| Definitie                   | De datum en het tijdstip waarop een correctieverzoek door de BRO is geaccepteerd. |
| Kardinaliteit               | 1                                                                                 |
| Domein                      | DatumTijd                                                                         |
| Toelichting                 | Het gegeven wordt door de BRO geproduceerd.                                       |
|                             |                                                                                   |

### *Bericht van afwijzing*

![](media/32c8db6f3bdc7dfe815c623938e62e91.png)

| **transactie-ID**          |                                                                                                                                                                                       |
|----------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Naam attribuut             | transactie-ID                                                                                                                                                                         |
| Definitie                  | De unieke identificatie die door de BRO wordt gebruikt voor het innameverzoek.                                                                                                        |
| Kardinaliteit              | 1                                                                                                                                                                                     |
| Domein                     | Transactiecode                                                                                                                                                                        |
|   Type                     | Code                                                                                                                                                                                  |
|   Opbouw                   | GMW-NNNNNNNNNNNN                                                                                                                                                                      |
| Toelichting                | Het gegeven wordt door de BRO geproduceerd.                                                                                                                                           |
|                            |                                                                                                                                                                                       |
| **object-ID bronhouder **  |                                                                                                                                                                                       |
| Naam attribuut             | object-ID bronhouder                                                                                                                                                                  |
| Definitie                  | De identificatie die door of voor de bronhouder is gebruikt om het object in de eigen administratie te kunnen vinden voordat het was geregistreerd in de basisregistratie ondergrond. |
| Kardinaliteit              | 0..1                                                                                                                                                                                  |
| Domein                     | Tekst                                                                                                                                                                                 |
|   Maximale lengte          | 200                                                                                                                                                                                   |
| Regels                     | Het gegeven is alleen aanwezig als het bericht een antwoord is op een verzoek het brondocument *GMW-Inrichten* te registreren.                                                        |
| Toelichting                | Het gegeven wordt door de BRO uit het brondocument gehaald.                                                                                                                           |
|                            |                                                                                                                                                                                       |
| **tijdstip van afwijzing** |                                                                                                                                                                                       |
| Naam attribuut             | tijdstip van afwijzing                                                                                                                                                                |
| Definitie                  | De datum en het tijdstip waarop een verzoek door de BRO is afgewezen.                                                                                                                 |
| Kardinaliteit              | 1                                                                                                                                                                                     |
| Domein                     | DatumTijd                                                                                                                                                                             |
| Toelichting                | Het gegeven wordt door de BRO geproduceerd.                                                                                                                                           |
|                            |                                                                                                                                                                                       |
| **reden afwijzing**        |                                                                                                                                                                                       |
| Naam attribuut             | reden afwijzing                                                                                                                                                                       |
| Definitie                  | De omschrijving van de reden waarom het verzoek door de BRO is afgewezen.                                                                                                             |
| Kardinaliteit              | 1                                                                                                                                                                                     |
| Domein                     | RedenAfwijzing                                                                                                                                                                        |
| Toelichting                | Het gegeven wordt door de BRO geproduceerd.                                                                                                                                           |
|                            |                                                                                                                                                                                       |
| **Foutenoverzicht**        |                                                                                                                                                                                       |
| Naam entiteit              | Foutenoverzicht                                                                                                                                                                       |
| Definitie                  | De omschrijving van alle fout(en) die in het brondocument zijn gevonden.                                                                                                              |
| Kardinaliteit              | 0..1                                                                                                                                                                                  |
| Regels                     | Het gegeven kan alleen voorkomen als de *reden afwijzing* de waarde heeft *er zijn 1 of meer fouten geconstateerd in het brondocument*.                                               |
| Toelichting                | Het gegeven wordt door de BRO geproduceerd.                                                                                                                                           |
|                            |                                                                                                                                                                                       |
| **volgnummer**             |                                                                                                                                                                                       |
| Naam attribuut             | volgnummer                                                                                                                                                                            |
| Definitie                  | Het volgnummer van een gevonden fout in het brondocument.                                                                                                                             |
| Kardinaliteit              | 1..99                                                                                                                                                                                 |
| Domein                     | Nummer                                                                                                                                                                                |
|   Maximale lengte          | 2                                                                                                                                                                                     |
|                            |                                                                                                                                                                                       |
| **brondocumentfout**       |                                                                                                                                                                                       |
| Naam attribuut             | brondocumentfout                                                                                                                                                                      |
| Definitie                  | De omschrijving van een fout in het brondocument.                                                                                                                                     |
| Kardinaliteit              | 1..99                                                                                                                                                                                 |
| Domein                     | Brondocumentfout                                                                                                                                                                      |
|   Type                     | Codelijst                                                                                                                                                                             |

### *Bericht van registratie*

![](media/438cd4915a6cadf55e9389aaf1edb1b2.png)

| **tijdstip van verwerking** |                                                                                 |
|-----------------------------|---------------------------------------------------------------------------------|
| Naam attribuut              | tijdstip van verwerking                                                         |
| Definitie                   | De datum en het tijdstip waarop het registratieverzoek door de BRO is verwerkt. |
| Domein                      | DatumTijd                                                                       |
| Toelichting                 | Het gegeven wordt door de BRO geproduceerd.                                     |

1.  Beschrijving van de codelijsten

    1.  *Brondocumentfout*

Een waarde in de lijst is een zin met een bepaalde opbouw en met zowel vaste als
variabele bestanddelen. De variabele bestanddelen gegeven aan waar de fout in
het brondocument zit en eventueel waarom het een fout is.

Een eerste variabele element is \<gegeven\>. Dat is altijd aanwezig en geeft aan
welk gegeven onjuist is. Een \<gegeven\> geeft de naam van het gegeven in het
Nederlands en in het Engels. Het kan een attribuut zijn, een entiteit of een
attribuut met zijn entiteit.

In sommige gevallen wordt met het gegeven ook de waarde van het gegeven
opgenomen (\<gegeven = waarde\>).

Een tweede variabel element is \<referentiegegeven\> en dat wordt opgenomen
wanneer er een tweede gegeven is dat bepaalt dat het \<gegeven\> fout is. Dat
kan een gegeven zijn in het brondocument, maar ook een gegeven in de registratie
ondergrond. Zo nodig wordt ook hier de waarde meegegeven (\<referentiegegeven =
waarde\>).

Een derde variabel element is \<referentiewaarde\> en dat wordt opgenomen
wanneer een waardebereik bepaalt dat het \<gegeven\> fout is.

| *GEGEVEN ONTBREEKT*                                                                                                                                                                                         |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| \<gegeven\> ontbreekt: \<referentiegegeven = waarde\> bepaalt dat het aanwezig moet zijn.                                                                                                                   |
| \<gegeven\> ontbreekt: \<referentiegegeven = waarde\> bepaalt het aantal keer dat het gegeven voorkomt.                                                                                                     |
| \<gegeven\> ontbreekt: het moet aanwezig zijn als \<referentiegegeven\> ontbreekt.                                                                                                                          |
| *GEGEVEN MAG NIET AANWEZIG ZIJN*                                                                                                                                                                            |
| \<gegeven\> mag niet aanwezig zijn: \<referentiegegeven = waarde\> bepaalt dat het moet ontbreken.                                                                                                          |
| \<gegeven\> mag niet aanwezig zijn: \<referentiegegeven = waarde\> bepaalt het aantal keer het dat gegeven voorkomt.                                                                                        |
| *WAARDE ONTBREEKT*                                                                                                                                                                                          |
| \<gegeven\> waarde ontbreekt.                                                                                                                                                                               |
| *WAARDE HEEFT GEEN CORRECT FORMAAT*                                                                                                                                                                         |
| \<gegeven = waarde\> waarde heeft geen correct formaat: moet zijn \<referentiewaarde\>.                                                                                                                     |
| \<gegeven = waarde\> waarde heeft geen correct formaat: voldoet niet aan de MES 1 karakterset.                                                                                                              |
| *WAARDE IS NIET CORRECT*                                                                                                                                                                                    |
| \<gegeven = waarde\> waarde is niet correct: komt niet voor in de codelijst.                                                                                                                                |
| \<gegeven = waarde\> waarde is niet correct: moet gelijk zijn aan \<referentiewaarde\>.                                                                                                                     |
| \<gegeven = waarde\> waarde is niet correct: is binnen de BRO niet bekend als \<referentiewaarde\> van dit registratieobjecttype. Neem contact op met de servicedesk (info\@basisregistratieondergrond.nl). |
| \<gegeven = waarde\> waarde is niet correct: ligt niet binnen Nederland of zijn EEZ.                                                                                                                        |
| \<gegeven = waarde\> waarde is niet correct: ligt niet binnen Nederland aan de landzijde van de UNCLOS-basislijn.                                                                                           |
| \<gegeven = waarde\> waarde is niet correct: op land moeten de coördinaten in RD of in ETRS89 aangeleverd worden.                                                                                           |
| \<gegeven = waarde\> waarde is niet correct: op land moet de verticale positie ten opzichte van NAP aangeleverd worden.                                                                                     |
| \<gegeven = waarde\> waarde is niet correct: mag niet kleiner zijn dan \<referentiewaarde\>.                                                                                                                |
| \<gegeven = waarde\> waarde is niet correct: mag niet groter zijn dan \<referentiewaarde\>.                                                                                                                 |
| \<gegeven = waarde\> waarde is niet correct: moet kleiner zijn dan \<referentiegegeven = waarde\>.                                                                                                          |
| \<gegeven = waarde\> waarde is niet correct: moet gelijk zijn aan \<referentiegegeven = waarde\>.                                                                                                           |
| \<gegeven = waarde\> waarde is niet correct: is niet toegestaan.                                                                                                                                            |
| \<gegeven = waarde\> waarde is niet correct: is niet toegestaan in combinatie met \<referentiegegeven = waarde\>.                                                                                           |
| \<gegeven = waarde\> waarde is niet correct: mag niet na \<referentiewaarde\> liggen.                                                                                                                       |
| \<gegeven = waarde\> waarde is niet correct: mag niet voor \<referentiewaarde\> liggen.                                                                                                                     |
| \<gegeven = waarde\> waarde is niet correct: mag niet na \<referentiegegeven = waarde\> liggen.                                                                                                             |
| \<gegeven = waarde\> waarde is niet correct: mag niet voor \<referentiegegeven = waarde\> liggen.                                                                                                           |
| \<gegeven = waarde\> waarde is niet correct: mag niet in de toekomst liggen.                                                                                                                                |
| \<gegeven = waarde\> waarde is niet correct: moet uniek zijn.                                                                                                                                               |
| \<gegeven = waarde\> waarde is niet correct: moet afwijken van de waarde in de registratie ondergrond.                                                                                                      |
| \<gegeven = waarde\> waarde is niet correct: ten minste één van de volgende gegevens \<referentiegegeven1, …, referentiegegevenN\> moet afwijken van de waarde in de registratie ondergrond.                |
| \<gegeven = waarde\> waarde is niet correct: komt niet overeen met de waarde in de registratie ondergrond \<referentiewaarde\>.                                                                             |
| \<gegeven = waarde\> waarde is niet correct: bestaat niet in de registratie ondergrond.                                                                                                                     |
| \<gegeven = waarde\> waarde is niet correct: gebeurtenis valt niet tussen twee reeds geregistreerde gebeurtenissen in.                                                                                      |
| \<gegeven = waarde\> waarde is niet correct: gebeurtenis mag niet voor de laatst geregistreerde gebeurtenis \<referentiegegeven = waarde\> liggen.                                                          |
| \<gegeven = waarde\> waarde is niet correct: gebeurtenis mag niet na de eerst geregistreerde aanvulling \<referentiegegeven = waarde\> liggen.                                                              |
| \<naam gebeurtenis = waarde\> op \<datum gebeurtenis = waarde\> is niet correct: bestaat reeds in de registratie ondergrond.                                                                                |
| \<naam gebeurtenis = waarde\> op \<datum gebeurtenis = waarde\> is niet correct: bestaat niet in de registratie ondergrond.                                                                                 |
| \<gegeven = waarde\> waarde is niet correct: moet kleiner zijn dan de waarde in de registratie ondergrond \<waarde\>.                                                                                       |
| \<gegeven = waarde\> waarde is niet correct: moet groter zijn dan de waarde in de registratie ondergrond \<waarde\>.                                                                                        |
| er zijn nog meer fouten geconstateerd in het brondocument.                                                                                                                                                  |

### *Brondocumenttype*

| Waarde                  | Omschrijving                                                                                                                  |
|-------------------------|-------------------------------------------------------------------------------------------------------------------------------|
| GMW-Beschermconstructie | Het brondocument voor verandering van beschermconstructie.                                                                    |
| GMW-Buisstatus          | Het brondocument voor verandering van buisstatus.                                                                             |
| GMW-Eigenaar            | Het brondocument voor verandering van eigenaar.                                                                               |
| GMW-Elektrodestatus     | Het brondocument voor verandering van elektrodestatus.                                                                        |
| GMW-Inkorten            | Het brondocument voor inkorting van een monitoringbuis.                                                                       |
| GMW-Inplaatsen          | Het brondocument voor inplaatsing van een stijgbuisdeel.                                                                      |
| GMW-Inrichten           | Het brondocument voor inrichting van een grondwatermonitoringput.                                                             |
| GMW-Maaiveld            | Het brondocument voor herbepaling van de positie van het maaiveld.                                                            |
| GMW-Onderhouder         | Het brondocument voor verandering van onderhoudende instantie.                                                                |
| GMW-Oplengen            | Het brondocument voor oplenging van een monitoringbuis.                                                                       |
| GMW-Opruimen            | Het brondocument voor opruiming van een grondwatermonitoringput.                                                              |
| GMW-Posities            | Het brondocument voor herbepaling van de posities van het maaiveld en de bovenkant van de monitoringbuizen.                   |
| GMW-Verleggen           | Het brondocument voor herbepaling van de positie van het maaiveld wanneer het terrein rond de put is opgehoogd of afgegraven. |

*Correctiereden*

| Waarde           | Omschrijving                                                                                                                                                                                                |
|------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| bronhouder       | De correctie die de dataleverancier op eigen initiatief aanbiedt omdat hij heeft geconstateerd dat de waarde van de *bronhouder* van de grondwatermonitoringput in de registratie ondergrond niet juist is. |
| eigen correctie  | De correctie die de dataleverancier op eigen initiatief aanbiedt omdat hij heeft geconstateerd dat er in de registratie ondergrond een fout zit die herleid kan worden tot een fout in een brondocument.    |
| kwaliteitsRegime | De correctie die de dataleverancier op eigen initiatief aanbiedt omdat de waarde van het *kwaliteitsregime* van de grondwatermonitoringput in de registratie ondergrond niet juist is.                      |
| inOnderzoek      | De correctie van een fout in de registratie ondergrond die wordt aangeboden in vervolg op een door de registratiebeheerder gestart onderzoek.                                                               |

### *RedenAfwijzing*

Een waarde in de lijst is net als bij het domein Brondocumentfout een zin met
een bepaalde opbouw die zowel vaste als variabele bestanddelen kan bevatten.

| **Waarde**                                                                                                                                                                                                  |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| \<gegeven\> ontbreekt.                                                                                                                                                                                      |
| \<gegeven\> mag niet aanwezig zijn.                                                                                                                                                                         |
| \<gegeven\> waarde ontbreekt.                                                                                                                                                                               |
| \<gegeven = waarde\> waarde heeft geen correct formaat: moet zijn \<referentiewaarde\>.                                                                                                                     |
| \<gegeven = waarde\> waarde heeft geen correct formaat: voldoet niet aan de MES 1 karakterset.                                                                                                              |
| \<gegeven = waarde\> waarde is niet correct: komt niet voor in de codelijst.                                                                                                                                |
| \<gegeven = waarde\> waarde is niet correct: is binnen de BRO niet bekend als \<referentiewaarde\> van dit registratieobjecttype. Neem contact op met de servicedesk (info\@basisregistratieondergrond.nl). |
| \<gegeven = waarde\> waarde is niet correct: is niet toegestaan in combinatie met \<referentiegegeven = waarde\>.                                                                                           |
| \<gegeven = waarde\> waarde is niet correct: komt niet overeen met de waarde in de registratie ondergrond \<referentiewaarde\>.                                                                             |
| dit registratieobject bestaat niet.                                                                                                                                                                         |
| dit registratieobject is uit registratie genomen.                                                                                                                                                           |
| dit registratieobject is in onderzoek.                                                                                                                                                                      |
| \<gegeven = waarde\> waarde is niet correct: is niet toegestaan, het registratieobject heeft kwaliteitsregime IMBRO.                                                                                        |
| \<gegeven = waarde\> waarde is niet correct: dit registratieobject heeft geen voorgeschiedenis.                                                                                                             |
| \<gegeven = waarde\> waarde is niet correct: dit registratieobject is niet in onderzoek.                                                                                                                    |
| \<gegeven = waarde\> waarde is niet correct: dit registratieobject is in onderzoek.                                                                                                                         |
| \<gegeven = waarde\> waarde is niet correct: is niet toegestaan voor dit (type) brondocument.                                                                                                               |
| \<gegeven = waarde\> waarde is niet correct: dit registratieobject heeft al het door u gewenste kwaliteitsregime.                                                                                           |
| \<gegeven = waarde\> waarde is niet correct: dit registratieobject heeft al de door u gewenste bronhouder.                                                                                                  |
| \<gegeven\> ontbreekt. U bent binnen de BRO niet bekend als bronhouder van dit registratieobjecttype. Neem contact op met de servicedesk (info\@basisregistratieondergrond.nl).                             |
| \<gegeven\> ontbreekt. U mag alleen registratieobjecten met voorgeschiedenis aanleveren.                                                                                                                    |
| \<gegeven\> mag niet aanwezig zijn. U bent als bronhouder van dit registratieobjecttype geregistreerd.                                                                                                      |
| u bent niet door de bronhouder gemachtigd voor dit registratieobjecttype.                                                                                                                                   |
| \<gegeven\> mag niet aanwezig zijn. U mag geen registratieobjecten met voorgeschiedenis aanleveren.                                                                                                         |
| u bent niet als dataleverancier van dit registratieobject geregistreerd.                                                                                                                                    |
| Dit registratieobject heeft de registratiestatus *voltooid.*                                                                                                                                                |
| er zijn 1 of meer fouten geconstateerd in het brondocument.                                                                                                                                                 |
| er zijn 1 of meer fouten geconstateerd in de kenmerkenverzameling.                                                                                                                                          |
| het aantal uitgiftedocumenten is groter dan 2000. Pas de kenmerken van uw verzoek tot verzending kengegevens aan.                                                                                           |

E-mailberichten 
----------------

De registratiebeheerder stuurt de dataleverancier naar aanleiding van een
correctieverzoek via e-mail een bericht van bezwaar of een bericht van
correctie. Van de twee berichten wordt hier een voorbeeld gegeven.

### *Bericht van bezwaar*

>   **Berichtkop**

>   Afzender: noreply\@bro.nl  
>   Geadresseerde: \<e-mailadres dataleverancier\>

>   Onderwerp: BRO, Bericht van bezwaar CPT kenmerk \<verzoekkenmerk\>

>   **Bericht**

>   Geachte mevrouw/heer,

>   Uw correctieverzoek met het bovenstaande kenmerk is afgewezen op \<tijdstip
>   van afwijzing\> omdat \<reden bezwaar\>. Hieronder vindt u de details van uw
>   verzoek.

>   Transactie-ID: \<transactie-ID\>  
>   Correctiereden: \<correctiereden\>  
>   Kwaliteitsregime: \<kwaliteitsregime\>

>   BRO-ID: \<BRO-ID\>

>   Naam bronhouder: \<naam bronhouder\>  
>   Tijdstip van acceptatie: \<tijdstip van acceptatie\>

>   Met vriendelijke groet,

>   BRO Registerbeheer

>   \<naam registratiebeheerder\>

*Bericht van correctie*

>   **Berichtkop**

>   Afzender: noreply\@bro.nl  
>   Geadresseerde: \<e-mailadres dataleverancier\>

>   Onderwerp: BRO, Bericht van correctie CPT verzoek \<verzoekkenmerk\>

>   **Bericht**

>   Geachte mevrouw/heer,

>   Uw correctieverzoek met het bovenstaande kenmerk is goedgekeurd en de
>   gegevens zijn opgenomen op \<tijdstip van verwerking\> in de registratie
>   ondergrond. Hieronder vindt u de details van uw verzoek.

>   Transactie ID: \<transactie-ID\>  
>   Correctie reden: \<correctiereden\>  
>   Kwaliteitsregime: \<kwaliteitsregime\>

>   BRO-ID: \<BRO-ID\>

>   Naam bronhouder: \<naam bronhouder\>  
>   Tijdstip van acceptatie: \<tijdstip van acceptatie\>

>   Met vriendelijke groet,

>   BRO Registerbeheer

>   \<naam registratiebeheerder\>

Brondocumenten
--------------

Er zijn in het totaal dertien verschillende *brondocumenten*. De brondocumenten
verschillen per definitie in inhoud, maar kunnen ook in opbouw verschillen.
Sommige documenten bevatten alleen nieuwe gegevens, terwijl andere naast nieuwe
gegevens ook gegevens bevatten die nodig zijn voor identificatie. Ten slotte
bevatten bepaalde berichten ook gegevens die bedoeld zijn om de integriteit van
het brondocument te garanderen. Die derde categorie is in de UML-modellen
zichtbaar gemaakt (\<\<*stuurgegeven*\>\>).

De algemene regels die bij inname gelden zijn voor ieder van de brondocumenten
geformuleerd, maar de meer specifieke regels die van het type verzoek en het
type correctie afhangen niet.

### *GMW-Inrichten*

Het brondocument dat wordt aangeboden wanneer een nieuwe put is ingericht en het
begin van het registratieproces markeert (figuur 5).

Alleen wanneer het document bij een verzoek hoort dat *onder voorrecht* wordt
aangeboden, mag de *inrichtingsdatum put* de waarden uit het domein
OnvolledigeDatum hebben.

### *GMW-Beschermconstructie*

Het brondocument dat wordt aangeboden wanneer de put na inrichting alsnog
voorzien is van een beschermconstructie of wanneer de bestaande
beschermconstructie is vervangen door een ander type.

![](media/80ac4fe8234f9a5bfe1f63735b70d5f9.png)

Alleen wanneer het document bij een verzoek hoort dat *onder voorrecht* wordt
aangeboden mag het gegeven *datum gebeurtenis* de waarden uit het domein
OnvolledigeDatum hebben met uitzondering van de waarde *onbekend*.

Het gegeven *beschermconstructie* mag nooit de IMBRO/A-waarde *onbekend* hebben.

### *GMW-Buisstatus*

![](media/14c34266a90fb71a714bc6d7c6efd908.png)

Het brondocument dat wordt aangeboden wanneer de toestand die aangeeft of een
monitoringbuis gebruikt kan worden voor grondwatermonitoring voor een of meer
buizen is veranderd.

>   [./media/image24.emf](./media/image24.emf)

>   *Figuur 5: GMW-Inrichten.*

| **aantal veranderde buizen** |                                                                                 |
|------------------------------|---------------------------------------------------------------------------------|
| Naam attribuut               | aantal veranderde buizen                                                        |
| Definitie                    | Het stuurgegeven dat aangeeft van hoeveel monitoringbuizen de status verandert. |
| Kardinaliteit                | 1                                                                               |
| Domein                       | Aantal                                                                          |
|   Maximale lengte            | 2                                                                               |
| Waardebereik                 | 1 tot 50                                                                        |

Alleen wanneer het document bij een verzoek hoort dat *onder voorrecht* wordt
aangeboden mag het kwaliteitsregime IMBRO/A zijn. Het gegeven *datum
gebeurtenis* mag dan de waarden uit het domein OnvolledigeDatum hebben met
uitzondering van de waarde *onbekend*. Het gegeven *buisstatus* mag nooit de
IMBRO/A-waarde *onbekend* hebben.

De buisnummers zijn uniek binnen het brondocument.

### *GMW-Eigenaar*

![](media/470b61878ff56a0e5aaa7f631221714b.png)

Het brondocument dat wordt aangeboden wanneer het eigendom van de
grondwatermonitoringput op een andere organisatie is overgegaan.

Alleen wanneer het document bij een verzoek hoort dat *onder voorrecht* wordt
aangeboden mag het kwaliteitsregime IMBRO/A zijn. Het gegeven *datum
gebeurtenis* mag dan de waarden uit het domein OnvolledigeDatum hebben met
uitzondering van de waarde *onbekend*.

De waarde van het gegeven *eigenaar* mag alleen ontbreken in het zeer
uitzonderlijke geval dat het eigendom is overgegaan van een onderneming die in
het Handelsregister is geregistreerd op een eigenaar die niet is geregistreerd.

### *GMW-Elektrodestatus*

Het brondocument dat wordt aangeboden wanneer de toestand die aangeeft of een
elektrode gebruikt kan worden voor grondwatermonitoring voor een of meer
elektroden is veranderd.

![](media/4ebf8b651c915e39eeea85631165b37f.png)

| **aantal veranderde elektrodes** |                                                                       |
|----------------------------------|-----------------------------------------------------------------------|
| Naam attribuut                   | aantal veranderde elektrodes                                          |
| Definitie                        | Stuurgegeven dat aangeeft van hoeveel elektrodes de status verandert. |
| Domein                           | Aantal                                                                |
|   Maximale lengte                | 2                                                                     |
| Waardebereik                     | 1 tot 50                                                              |

Alleen wanneer het document bij een verzoek hoort dat *onder voorrecht* wordt
aangeboden mag het kwaliteitsregime IMBRO/A zijn. Het gegeven *datum
gebeurtenis* mag dan de waarden uit het domein OnvolledigeDatum hebben met
uitzondering van de waarde *onbekend*. Het gegeven *elektrodestatus* mag nooit
de IMBRO/A-waarde *onbekend* hebben.

De elektrodenummers zijn uniek voor een kabel.

### *GMW-Inkorten*

Het brondocument dat wordt aangeboden wanneer één of meer buizen zijn ingekort.
Wanneer ook de beschermconstructie is veranderd bevat het brondocument het
gegeven *beschermconstructie* met de nieuwe waarde.

![](media/164b8b4aced810e27db28596279db89b.png)

| **aantal ingekorte buizen**  |                                                                         |
|------------------------------|-------------------------------------------------------------------------|
| Naam attribuut               | aantal ingekorte buizen                                                 |
| Definitie                    | Stuurgegeven dat aangeeft hoeveel monitoringbuizen korter zijn gemaakt. |
| Domein                       | Aantal                                                                  |
| Maximale lengte              | 2                                                                       |
| Waardebereik                 | 1 tot 50                                                                |

Alleen wanneer het document bij een verzoek hoort dat *onder voorrecht* wordt
aangeboden mag het gegeven *datum gebeurtenis* de waarden uit het domein
OnvolledigeDatum hebben met uitzondering van de waarde *onbekend*.

Het gegeven *beschermconstructie* mag nooit de IMBRO/A-waarde *onbekend* hebben.

De buisnummers zijn uniek binnen het brondocument.

Het gegeven *buisnummer* mag niet verwijzen naar een buis waarvan het *buistype*
de waarde *volledigFilter* of *filterlozeBuis* heeft.

De waarde van het gegeven *lengte stijgbuisdeel* moet kleiner zijn dan de waarde
die in de registratie ondergrond geldt voor de periode voorafgaand aan de *datum
gebeurtenis*.

### *GMW-Inplaatsen*

![](media/b69a9860eb8d35a938ff129417f3a45d.png)

Het brondocument dat wordt aangeboden wanneer in een monitoringbuis een
stijgbuisdeel is ingeplaatst.

Alleen wanneer het document bij een verzoek hoort dat *onder voorrecht* wordt
aangeboden mag het gegeven *datum gebeurtenis* de waarden uit het domein
OnvolledigeDatum hebben met uitzondering van de waarde *onbekend*.

De waarde van het gegeven *diameter bovenkant ingeplaatst deel* moet kleiner
zijn dan de waarde van het gegeven *diameter bovenkant buis* van de
monitoringbuis waarin het stijgbuisdeel is geplaatst.

### *GMW-Maaiveldpositie*

![](media/b72a2ee7a0077fd902f04b2e4c57de6a.png)

Het brondocument dat wordt aangeboden wanneer een nieuwe maaiveldpositie is
bepaald.

Alleen wanneer het document bij een verzoek hoort dat *onder voorrecht* wordt
aangeboden mag het gegeven *datum gebeurtenis* de waarden uit het domein
OnvolledigeDatum hebben met uitzondering van de waarde *onbekend*.

Het gegeven *maaiveldpositie* heeft altijd een waarde, ook wanneer het
kwaliteitsregime van het brondocument de waarde *IMBRO/A* heeft (en om die reden
kan het gegeven *methode positiebepaling maaiveld* nooit de waarde *geen*
hebben).

### *GMW-Onderhouder*

![](media/eb9b920047f60079f1e3bbc9de1942a0.png)

Het brondocument dat wordt aangeboden wanneer een andere organisatie
verantwoordelijk is geworden voor het onderhoud van een grondwatermonitoringput.

Alleen wanneer het document bij een verzoek hoort dat *onder voorrecht* wordt
aangeboden mag het kwaliteitsregime IMBRO/A zijn. Het gegeven *datum
gebeurtenis* mag dan de waarden uit het domein OnvolledigeDatum hebben met
uitzondering van de waarde *onbekend*. Het gegeven *onderhoudende instantie* mag
nooit de IMBRO/A-waarde *onbekend* hebben.

### *GMW-Oplengen*

![](media/f84cd2305e7ba756b4829dde22b4ede9.png)

Het brondocument dat wordt aangeboden wanneer van een grondwatermonitoringput
één of meer buizen langer zijn gemaakt.

| **aantal opgelengde buizen**  |                                                                         |
|-------------------------------|-------------------------------------------------------------------------|
| Naam attribuut                | aantal opgelengde buizen                                                |
| Definitie                     | Stuurgegeven dat aangeeft hoeveel monitoringbuizen langer zijn gemaakt. |
| Domein                        | Aantal                                                                  |
|   Maximale lengte             | 2                                                                       |
| Waardebereik                  | 1 tot 50                                                                |

Alleen wanneer het document bij een verzoek hoort dat *onder voorrecht* wordt
aangeboden mag het gegeven *datum gebeurtenis* de waarden uit het domein
OnvolledigeDatum hebben met uitzondering van de waarde *onbekend*.

Het gegeven *beschermconstructie* mag nooit de IMBRO/A-waarde *onbekend* hebben.

De gegevens *diameter bovenkant buis, variabele diameter, buismateriaal* en
*lijm* zijn alleen aanwezig als de waarde moet veranderen.

Het gegeven *lijm* mag nooit de waarde *onbekend* of *geen* hebben.

Het gegeven *variabele diameter* heeft altijd de waarde *Ja*.

De buisnummers zijn uniek binnen het brondocument.

Het gegeven *buisnummer* mag niet verwijzen naar een buis waarvan het gegeven
*buistype* de waarde *volledigFilter* of *filterlozeBuis* is.

De waarde van het gegeven *lengte stijgbuisdeel* moet groter zijn dan de waarde
die in de registratie ondergrond geldt voor de periode voorafgaand aan de datum
gebeurtenis.

### *GMW-Posities*

![](media/d51763be163ac95e9e92ea7f0439dcad.png)

Het brondocument dat wordt aangeboden wanneer de posities van het maaiveld en de
bovenkant van de monitoringbuizen opnieuw zijn vastgesteld.

Alleen wanneer het document bij een verzoek hoort dat *onder voorrecht* wordt
aangeboden mag het gegeven datum gebeurtenis de waarden uit het domein
OnvolledigeDatum hebben met uitzondering van de waarde *onbekend*.

Het gegeven *maaiveldpositie* heeft altijd een waarde, ook wanneer het
kwaliteitsregime van het brondocument de waarde IMBRO/A heeft.

Het gegeven *methode positiebepaling maaiveld* kan nooit de waarde *geen*
hebben.  
Het gegeven *methode positiebepaling bovenkant buis* kan nooit de waarde
*afgeleidSbl* hebben).

De buisnummers zijn uniek binnen het brondocument.

### *GMW-Verleggen*

![](media/1517d096bd00f129412af34d3f8bc7d8.png)

Het brondocument dat in een verzoek de registratie aan te vullen wordt
aangeboden wanneer het maaiveld bij een grondwatermonitoringput door menselijk
ingrijpen is veranderd.

Alleen wanneer het document bij een verzoek hoort dat *onder voorrecht* wordt
aangeboden mag het gegeven *datum gebeurtenis* de waarden uit het domein
OnvolledigeDatum hebben met uitzondering van de waarde *onbekend*.

Het gegeven *maaiveldpositie* heeft altijd een waarde, ook wanneer het
kwaliteitsregime van het brondocument de waarde IMBRO/A heeft.

Het gegeven *methode positiebepaling maaiveld* kan niet de waarde *geen* hebben.

### *GMW-Opruimen*

![](media/58a153c4bc47aed120d3697b9e0f0a17.png)

Het brondocument dat in een verzoek de registratie aan te vullen wordt
aangeboden wanneer een grondwatermonitoringput is opgeruimd.

Wanneer het document bij een verzoek hoort dat *onder voorrecht* wordt
aangeboden mag het gegeven *opruimingsdatum put* alle waarden uit het domein
OnvolledigeDatum hebben, ook waarde *onbekend.* Alleen in dat geval heeft het
kwaliteitsregime van het brondocument de waarde *IMBRO/A*.
