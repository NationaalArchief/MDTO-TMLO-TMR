# Wijzigingen ten opzichte van TMLO en TMR

## Toepassingsgebied
MDTO is bedoeld voor toepassing door alle overheidsorganisaties.

## Terminologie
MDTO gebruikt zoveel mogelijk bestaande termen en definities. Een aantal termen is anders ten opzichte van TMLO/TMR. De voornaamste reden hiervoor is om beter aan te sluiten bij terminologie die wordt gebruikt in de architectuur en door ontwerpers van informatiesystemen. MDTO is daarmee beter toepasbaar door archiefvormers. Zo gebruikt MDTO de term ‘klasse’  in plaats van entiteit en ‘informatieobject’ in plaats van record. Veel bestaande definities zijn behouden (al dan niet in aangepaste vorm).

## Specificatie
De structuur van de specificatie van klassen en attributen is verbeterd. Hierdoor is de specificatie overzichtelijker en explicieter. Er zijn verder veel voorbeelden toegevoegd. Deze zijn gescheiden van de definities en de toelichting. Bij de definities, maar ook bij de teksten in MDTO in het algemeen, zijn veel onduidelijkheden of dubbelzinnigheden verwijderd.

## Onderdelen
TMLO en TMR bestaan uit één onderdeel: het metagegevensschema.
Ze voorzien niet in een machineleesbaar schema (XML) en een uitwisselingsprotocol.

In de praktijk hebben archiefinstellingen daar zelf invulling aan gegeven. Dit leidde tot onderlinge verschillen (in wat en hoe er uitgewisseld wordt). MDTO kent meerdere modules, waarvan een deel normerend is en een deel niet. Hiermee is ook de uitwisseling zelf gestandaardiseerd.

Modules van MDTO zijn:
| Normerend                                                                                            | Niet-normerend                                                                    |
| ---------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| [Metagegevensschema](https://nationaalarchief.github.io/MDTO-Metagegevensschema/)                    | RDF-ontologie                                                                     |
| [XML-schema](https://nationaalarchief.github.io/MDTO-XSD/)                                           | [Aanleverproces SIP](https://nationaalarchief.github.io/MDTO-SIP-aanleverproces/) |
| [Definitie van MDTO-conform](https://nationaalarchief.github.io/MDTO-Conform/)                       | [Mapping TMLO/TMR naar MDTO](#mapping-van-tmlo-tmr-naar-mdto)                     |
| [MDTO Begrippenlijsten](http://nationaalarchief.github.io/MDTO-Metagegevensschema/#begrippenlijsten) |                                                                                   |
| [Specificatie SIP](https://nationaalarchief.github.io/MDTO-SIP-specificatie/)                        |                                                                                   |

## Presentatie
Het Nationaal Archief presenteert MDTO als een set webpagina’s op de website.

Het gebruik van webpagina’s maakt MDTO toegankelijker en sluit beter aan bij de eisen voor van digitoegankelijkheid aan gepubliceerde overheidsinformatie. 

Daarnaast biedt het gebruik van webpagina’s het Nationaal Archief de mogelijkheid om delen van MDTO te (laten) reviewen. En aanpassingen door te voeren zonder MDTO in zijn geheel opnieuw te moeten publiceren. Denk aan kleine aanpassingen in de tekst en het toevoegen van extra toelichting of voorbeelden bij afzonderlijke attributen. Of aan grotere aanpassingen, zoals uitbreidingen van MDTO.

## Nummering attributen
Attributen in MDTO zijn niet voorzien van een nummer, zoals in TMLO/TMR.

MDTO kent ten opzichte van TMLO/TMR nogal wat wijzigingen in de attributen. Hierdoor was de bestaande nummering uit TMLO/TMR niet meer bruikbaar.

Door MDTO als een set van webpagina’s te presenteren, is er wel sprake van onderlinge relaties, maar niet van een bepaalde volgordelijkheid.  Gebruikers kunnen op iedere webpagina terecht komen. Er is een [mapping](#mapping-van-tmlo-tmr-naar-mdto) beschikbaar waarin de elementen uit TMLO/TMR worden gemapt naar attributen in MDTO (voor zover mogelijk).

## Verplichtingsniveaus aangepast
TMLO/TMR kennen vijf verplichtingsniveaus (van verplicht tot optioneel). Die niveaus zijn soms moeilijk van elkaar te onderscheiden. Ook is het niet altijd duidelijk wat ‘van toepassing’ zijn in de praktijk inhoudt. In MDTO worden de verplichtingen teruggebracht tot twee: ‘verplicht’ en ‘verplicht indien bekend’. Een uitleg hierover staat in de [Definitie van MDTO conform](https://nationaalarchief.github.io/MDTO-Conform/).

## Geen eigen toepassingsprofiel
Anders dan TMLO/TMR gaat MDTO niet uit van het maken van een eigen toepassingsprofiel (of metagegevensschema) op basis van MDTO. 

Door een metagegevensschema (zoals vermeld in de Archiefregeling) inhoudelijk te beperken tot wat alleen in TMLO/TMR is gespecificeerd, wordt geen recht gedaan aan andere metagegevens die voor andere doeleinden vastgelegd worden. Door de regels die werden gesteld in TMLO en TMR, was het ook omslachtig om extra, organisatiespecifieke gegevens toe te voegen aan een eigen profiel. Met als gevolg dat regelmatig werd geprobeerd om andere metagegevenselementen te mappen naar elementen in TMLO, die daar niet voor bedoeld waren. 

Elke organisatie zal nog steeds een eigen metagegevensschema moeten maken, zoals vermeld in de Archiefregeling. Maar dat hoeft geen profiel van MDTO te zijn. Zolang het eigen metagegevensschema maar wel te vertalen is naar MDTO (ook wel aangeduid als ‘mapping’). Het is daarbij niet noodzakelijk dat een organisatie één metagegevensschema voor de hele organisatie maakt. Dat kunnen er ook meerdere zijn, voor verschillende werkprocessen en informatiesystemen. De schema’s kunnen organisatie- of domeinspecifiek zijn. Voordeel van deze aanpak ten opzichte van TMLO/TMR is dat er recht wordt gedaan aan andere metagegevens die voor andere doeleinden vastgelegd worden. Ook zijn er geen omslachtige regels meer om extra, organisatiespecifieke gegevens toe te voegen aan een eigen profiel.

MDTO faciliteert de uitwisseling van organisatie- en domeinspecifieke metagegevens. In TMLO/TMR was hierin niet voorzien.

## Aggregatieniveaus
MDTO definieert wat een informatieobject is, maar niet wat een organisatie als een informatieobject kan of moet beschouwen. Ook onderkent MDTO dat informatieobjecten kunnen worden geaggregeerd, dus dat informatieobjecten tezamen ook een informatieobject kunnen vormen. Zoals een zaak/dossier met daarbinnen documenten over op de zaak of het dossier.

In tegenstelling tot TMLO/TMR schrijft MDTO geen aggregatieniveaus voor. Maar vermeldt alleen een aantal mogelijke waarden. Archiefvormers kunnen zelf aggregatieniveaus onderscheiden en benoemen, of kunnen gebruik maken van de voorbeelden uit MDTO. Of beide. Dit maakt het eenvoudiger om een eigen ordening te hanteren. 

## Beperking gebruik
TMLO/TMR kennen drie elementen die te maken hebben met beperkingen op het gebruik: Gebruiksrechten, Vertrouwelijkheid en Openbaarheid. In MDTO is hier de gegevensgroep ‘Beperking gebruik’ voor in de plaats gekomen. Hiermee kunnen meerdere typen beperkingen vastgelegd worden die voor informatieobjecten gelden (er kunnen meerdere beperkingen tegelijk van toepassing zijn). Zoals vanuit het Auteursrecht, de AVG, informatiebeveiliging (BIO) of de Archiefwet. In de praktijk zijn er veel verschillende beperkingen mogelijk, specifieke voorwaarden of meerdere betrokkenen die al dan niet toestemming kunnen geven voor gebruik van een informatieobject. Al deze mogelijkheden laten zich niet goed vatten in een schema. 

## Betrokkene
In TMLO/TMR is de mogelijkheid om gegevens over een actor vast te leggen. Dat is in de praktijk een overheidsorganisatie of een vertegenwoordiger daarvan, verantwoordelijk voor de creatie of ontvangst van een informatieobject als onderdeel van zijn of haar taak. In MDTO is daarnaast het attribuut ‘Betrokkene’ toegevoegd. Hiermee kunnen ook gegevens over andere organisaties of personen worden vastgelegd die een relatie hebben met een informatieobject (zoals een aanvrager van een vergunning).

## Bewaartermijn
Het attribuut *‘Bewaartermijn’* vervangt *Event plan* uit TMLO/TMR. Uit de bewaartermijn van een informatieobject kunnen toekomstige gebeurtenissen worden afgeleid (zoals vernietiging of overbrenging). Het apart vastleggen van die toekomstige gebeurtenissen gebeurt niet in MDTO.

Toekomstige gebeurtenissen zijn over het algemeen organisatie- en/of systeem specifiek. Dat maakt het lastig en weinig zinvol om gegevens hierover gestandaardiseerd uit te wisselen. De ontvangende partij bepaalt in de meeste gevallen zelf  welke toekomstige gebeurtenissen er  zijn. Met uitzondering van de bewaartermijn en de termijnen voor de beperkingen op het gebruikt. Daarom zijn hiervoor specifieke attributen in MDTO toegevoegd.

## Integriteit
In TMLO/TMR is *Integriteit* een element dat betrekking heeft op de inhoudelijke integriteit (als tegenhanger van de technische integriteit van een bestand). Inhoudelijke integriteit laat zich lastig definiëren (het is meer dan volledigheid). En is in de praktijk eigenlijk altijd te koppelen aan een gebeurtenis (zoals een migratie of conversie). In MDTO wordt een gebeurtenis die betrekking heeft op de inhoud van een informatieobject vastgelegd met de gegevensgroep ‘Event’. Hieraan is nu een attribuut toegevoegd waarmee het resultaat van een event ook kan worden vastgelegd. Zoals het resultaat van controles die onderdeel zijn van een migratie- of conversieproces.

## Vorm van informatieobjecten
In TMLO/TMR worden vormkenmerken vastgelegd met een eigen element. Dit biedt de mogelijkheid om informatie te categoriseren op basis van die kenmerken. Dit is een vorm van classificatie. In MDTO kunnen vormkenmerken vastgelegd worden met het attribuut *‘Classificatie’*. 