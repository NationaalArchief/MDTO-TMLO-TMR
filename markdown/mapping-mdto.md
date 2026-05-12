# Mapping van TMLO/TMR naar MDTO
Onderstaand overzicht geeft een vertaling van de bestaande TMLO- en TMR-elementen naar MDTO-attributen. Door onderlinge verschillen is het niet altijd mogelijk om een 1-op-1 vertaling te maken.

| Elementnr. In TMLO 1.1 | Elementnaam in TMLO 1.1        | Element nr. in TMR | Elementnaam in TMR                              | Naam attribuut in MDTO                                               |
| ---------------------- | ------------------------------ | ------------------ | ----------------------------------------------- | -------------------------------------------------------------------- |
| 1                      | Entiteittype                   | 1                  | Entiteittype                                    | Nvt                                                                  |
| 2                      | Identificatiekenmerk           | 2                  | Identificatiekenmerk                            | identificatieKenmerk (*)                                             |
| 3                      | Aggregatieniveau               | 3                  | Aggregatieniveau                                | aggregatieniveau                                                     |
| 4                      | Naam                           | 4                  | Naam                                            | naam                                                                 |
| 5                      | Classificatie                  | 5                  | Classificatie                                   | classificatie                                                        |
| 5.1                    | Code                           | 5.1                | Code                                            | begripCode                                                           |
| 5.2                    | Omschrijving                   | 5.2                | Omschrijving                                    | Nvt                                                                  |
| 5.3                    | Bron                           | 5.3                | Bron                                            | begripBegrippenlijst (*)                                             |
| 5.4                    | Datum                          | 5.4                | Datum                                           | Nvt                                                                  |
| 6                      | Omschrijving                   | 6                  | Omschrijving                                    | omschrijving                                                         |
| 7                      | Plaats                         | 7                  | Plaats                                          | raadpleeglocatieFysiek (*)                                           |
| 9                      | Dekking                        | 9                  | Dekking                                         | Nvt                                                                  |
| 9.1                    | In tijd                        | 9.1                | In tijd                                         | dekkingInTijd                                                        |
| 9.2                    | Geografisch gebied             | 9.2                | Geografisch gebied                              | dekkingInRuimte                                                      |
| 10                     | Externe identificatiekenmerken | 10                 | Externe identificatiekenmerken                  | identificatie                                                        |
| 10.1                   | Kenmerk systeem                | 10.1               | Naam of identificatiekenmerk van extern systeem | identificatieKenmerk                                                 |
| 10.2                   | Nummer binnen systeem          | 10.2               | Nummer/code binnen betreffende systeem          | identificatieBron                                                    |
| 11                     | Taal                           | 11                 | Taal                                            | taal                                                                 |
| 12                     | Event geschiedenis             | 12                 | Event geschiedenis                              | event                                                                |
| 12.1                   | Datum/periode                  | 12.1               | Datum/periode                                   | eventTijd                                                            |
| 12.2                   | Type                           | 12.2               | Type                                            | eventType                                                            |
| 12.3                   | Beschrijving                   | 12.3               | Beschrijving                                    | Nvt                                                                  |
| 12.4                   | Verantwoordelijke functionaris | 12.4               | Verantwoordelijke functionaris                  | eventVerantwoordelijkActor                                           |
| 13                     | Event plan                     | 13                 | Event plan                                      | bewaartermijn (**)                                                   |
| 13.1                   | Datum/periode                  | 13.1               | Datum                                           | termijnStartdatumLooptijd, termijnLooptijd, termijnEinddatum (*)     |
| 13.4                   | Aanleiding                     | 13.4               | Trigger                                         | termijnTriggerStartLooptijd (*)                                      |
| 15                     | Relatie                        | 15                 | Relatie                                         | gerelateerdInformatieobject                                          |
| 15.1                   | Relatie-ID                     | 15.1               | Relatie-ID                                      | identificatieKenmerk (*)                                             |
| 15.2                   | Type relatie                   | 15.2               | Type relatie                                    | gerelateerdInformatieobjectTypeRelatie                               |
| 15.3                   | Nvt                            | 15.3               | Datum/periode                                   | Nvt                                                                  |
| 15C                    | (Ontstaans)context             | 15C                | Context                                         | Nvt                                                                  |
| 15C.1                  | Actor                          | 15C-1              | Actor                                           | archiefvormer                                                        |
| 15C.1.2                | Identificatiekenmerk           | 15C-1-2            | Identificatiekenmerk                            | identificatieKenmerk (*)                                             |
| 15C.1.3                | Aggregatieniveau               | 15C-1-3            | Aggregatieniveau                                | Nvt                                                                  |
| 15C.1.4.2              | Geautoriseerde naam            | 15C-1-4.2          | Geautoriseerde naam                             | naam                                                                 |
| 15C.1.7                | Plaats                         | 15C-1-7            | Plaats                                          | Nvt                                                                  |
| 15C.1.8                | Jurisdictie                    | 15C-1-8            | Jurisdictie                                     | Nvt                                                                  |
| 15C.2                  | Activiteit (werkproces)        | 15C-2              | Activiteit                                      | activiteit                                                           |
| 15C.2.2                | Identificatiekenmerk           | 15C-2-2            | Identificatiekenmerk                            | identificatieKenmerk (*)                                             |
| 15C.2.3                | Aggregatieniveau               | 15C-2-3            | Aggregatieniveau                                | Nvt                                                                  |
| 15C.2.4                | Naam (van het werkproces)      | 15C-2-4            | Naam                                            | naam                                                                 |
| 16                     | Gebruiksrechten                | 16                 | Gebruiksrechten                                 | beperkingGebruik (*)                                                 |
| 16.1                   | Omschrijving voorwaarden       | 16.1               | Omschrijving voorwaarden                        | beperkingGebruikNadereBeschrijving, beperkingGebruikDocumentatie (*) |
| 16.2                   | Datum/periode                  | 16.2               | Datum/periode                                   | beperkingGebruikTermijn (*)                                          |
| 17                     | Vertrouwelijkheid              | 17                 | Vertrouwelijkheid                               | beperkingGebruik (*)                                                 |
| 17.1                   | Classificatie/niveau           | 17.1               | Classificatie/niveau                            | beperkingGebruikType (*)                                             |
| 17.2                   | Datum/periode                  | 17.2               | Datum/periode                                   | beperkingGebruikTermijn (*)                                          |
| 18                     | Openbaarheid                   | 18                 | Openbaarheid                                    | beperkingGebruik (*)                                                 |
| 18.1                   | Omschrijving beperkingen       | 18.1               | Omschrijving beperkingen                        | beperkingGebruikType (*)                                             |
| 18.2                   | Datum/periode                  | 18.2               | Datum/periode                                   | beperkingGebruikTermijn (*)                                          |
| 19                     | Vorm                           | 19                 | Vorm                                            | classificatie                                                        |
| 19.1                   | Redactie/genre                 | 19.1               | Redactie/genre                                  | Nvt                                                                  |
| 19.2                   | Verschijningsvorm              | 19.2               | Verschijningsvorm                               | Nvt                                                                  |
| 19.3                   | Structuur                      | 19.3               | Structuur                                       | Nvt                                                                  |
| 20                     | Integriteit                    | 20                 | Integriteit                                     | eventResultaat (*)                                                   |
| 21                     | Formaat                        | 21                 | Formaat                                         | Bestand (*)                                                          |
| 21.1                   | Identificatiekenmerk           | 21.1               | Identificatiekenmerk                            | identificatieKenmerk (*)                                             |
| 21.2                   | Bestandsnaam                   | 21.2               | Bestandsnaam                                    | naam                                                                 |
| 21.2.1                 | Naam                           | 21.2.1             | Naam                                            | Nvt                                                                  |
| 21.2.2                 | Extensie                       | 21.2.2             | Extensie                                        | Nvt                                                                  |
| 21.3                   | Type                           | 21.3               | Type                                            | Nvt                                                                  |
| 21.4                   | Omvang                         | 21.4               | Omvang                                          | omvang                                                               |
| 21.5                   | Bestandsformaat                | 21.5               | Bestandsformaat                                 | bestandsformaat                                                      |
| 21.6                   | Creatieapplicatie              | 21.6               | Creatieapplicatie                               | Nvt                                                                  |
| 21.6.1                 | Naam                           | 21.6.1             | Naam                                            | Nvt                                                                  |
| 21.6.2                 | Versie                         | 21.6.2             | Versie                                          | Nvt                                                                  |
| 21.6.3                 | Datum aanmaak                  | 21.6.3             | Datum aanmaak                                   | Nvt                                                                  |
| 21.7                   | Fysieke integriteit            | 21.7               | Integriteit                                     | checksum                                                             |
| 21.7.1                 | Algoritme (type)               | 21.7.1             | Algoritme (type)                                | checksumAlgoritme                                                    |
| 21.7.2                 | Waarde                         | 21.7.2             | Waarde                                          | checksumWaarde                                                       |
| 21.7.3                 | Datum                          | 21.7.3             | Datum                                           | checksumDatum                                                        |
| 21.8                   | Datum aanmaak                  | 21.8               | Datum aanmaak                                   | Nvt                                                                  |
| 21.9                   | Event plan formaat             | 21.9               | Event plan                                      | Nvt                                                                  |
| 21.9.1                 | Datum                          | 21.9.1             | Datum                                           | Nvt                                                                  |
| 21.9.2                 | Type                           | 21.9.2             | Type                                            | Nvt                                                                  |
| 21.9.3                 | Beschrijving                   | 21.9.3             | Beschrijving                                    | Nvt                                                                  |
| 21.9.4                 | Aanleiding                     | 21.9.4             | Trigger                                         | Nvt                                                                  |
| 21.10                  | Relatie                        | 21.10              | Relatie                                         | isRepresentatieVan (*)                                               |

(*) Geen 1-op-1 mapping. Structuur gewijzigd t.o.v. TMR / TMLO of er zijn aanvullende of andere regels gesteld. Zie het MDTO metagegevensschema voor meer toelichting.

(**) Dit geldt alleen voor bewaartermijnen die in Eventplan zijn vastgelegd. Eventplan is verder geen onderdeel van MDTO.