# Documenten

Verzuimstandaard Werkgevers ↔ Arbodiensten, release 2024.

| | |
|---|---|
| Schema | [`xsd/Documenten.xsd`](../xsd/Documenten.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/Documenten/2024` |
| Versie | 2024.0 |
| Elementen | 83 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`Documenten`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | Bericht, code | 1..1 | an..5 | 00500 |
| &emsp;&emsp;`VnrBrCd` | Versienummer bericht, code | 1..1 | an..5 | 00005 |
| &emsp;&emsp;`AandatBr` | Aanmaakdatum bericht | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` | Aanmaaktijd bericht | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` | Identificatie inzender | 1..1 | an..40 |  |
| &emsp;&emsp;`IdOntvngr` | Identificatie ontvanger | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` | Berichtreferentienummer | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` | Test J/N | 1..1 | an1 | J, N |
| &emsp;&emsp;`OntvngstbevJN` | Ontvangstbevestiging gewenst J/N | 1..1 | an1 | J, N |
| &emsp;**`Wrkgvr`** | Werkgever | 0..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | Handelsnaam organisatie | 1..1 | an..100 |  |
| &emsp;&emsp;`InschrijvingsnrKvK` | Inschrijvingsnummer Kamer van Koophandel | 0..1 | n..8 |  |
| &emsp;&emsp;`VestigingsnrHandelsregister` | Vestigingsnummer | 0..1 | n..12 |  |
| &emsp;&emsp;`IdWrkgvrArbdnst` | Identificatie werkgever bij arbodienst | 1..1 | an..40 |  |
| &emsp;&emsp;`AansltnrGeguitwlngArbdnst` | Aansluitnummer gegevensuitwisseling Arbodienst | 1..1 | an..70 |  |
| &emsp;&emsp;`Lhnr` | Loonheffingennummer | 0..1 | an..12 |  |
| &emsp;**`CntprsnOntvanger`** | Contactpersoon ontvanger | 0..1 | groep |  |
| &emsp;&emsp;`Achternaam` | Achternaam/Achternamen | 1..1 | an..200 |  |
| &emsp;&emsp;`Voorl` | Voorletters | 0..1 | an..6 |  |
| &emsp;&emsp;`Roepnaam` | Roepnaam | 0..1 | an..35 |  |
| &emsp;&emsp;`GslchtCd` | Geslachtsaanduiding, code | 0..1 | an1 | M, O, V |
| &emsp;&emsp;**`Com`** | Communicatie | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`SrtComCd` | Soort communicatie, code | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;`NrCom` | Nummer/adres communicatie | 1..1 | an..512 |  |
| &emsp;**`CntprsnZender`** | Contactpersoon zender | 0..1 | groep |  |
| &emsp;&emsp;`Achternaam` | Achternaam/Achternamen | 1..1 | an..200 |  |
| &emsp;&emsp;`Voorl` | Voorletters | 0..1 | an..6 |  |
| &emsp;&emsp;`Roepnaam` | Roepnaam | 0..1 | an..35 |  |
| &emsp;&emsp;`GslchtCd` | Geslachtsaanduiding, code | 0..1 | an1 | M, O, V |
| &emsp;&emsp;**`Com`** | Communicatie | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`SrtComCd` | Soort communicatie, code | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;`NrCom` | Nummer/adres communicatie | 1..1 | an..512 |  |
| &emsp;**`Document`** | Document | 1..9999 | groep |  |
| &emsp;&emsp;`IdDocument` | Identificatie document | 1..1 | an..40 |  |
| &emsp;&emsp;`IdDocumentOud` | Identificatie document oud | 0..1 | an..40 |  |
| &emsp;&emsp;`DatDocument` | Datum document | 1..1 | datum |  |
| &emsp;&emsp;`SrtDocumentCd` | Soort document, code | 1..1 | an3 | 23 waarden, o.a. 100, 104, 158, 208, 215 … |
| &emsp;&emsp;`SrtDocumentOms` | Soort document, omschrijving | 0..1 | an..70 |  |
| &emsp;&emsp;`StatDocumentCd` | Status document, code | 0..1 | an2 | 01, 02 |
| &emsp;&emsp;`KenmerkZendPartij` | Copyright SIVI | 1..1 | an..512 |  |
| &emsp;&emsp;`RdAanlevDocumentCd` | Reden aanlevering document, code | 0..1 | an2 | 01, 02, 03 |
| &emsp;&emsp;`PrioriteitCd` | Prioriteit, code | 0..1 | an2 | 01, 02, 03 |
| &emsp;&emsp;`BestandTypCd` | Bestand type, code | 0..1 | an2 | 14 waarden, o.a. 01, 02, 03, 04, 05 … |
| &emsp;&emsp;`Bestandsnm` | Bestandsnaam | 0..1 | an..70 |  |
| &emsp;&emsp;`AdresseringCd` | Adressering, code | 0..1 | an2 | 01, 02, 03 |
| &emsp;&emsp;`Datastring` | Datastring | 1..1 | string |  |
| &emsp;&emsp;**`Wrknmr`** | Werknemer | 1..1 | groep |  |
| &emsp;&emsp;&emsp;`SofiNr` | Burgerservicenummer | 0..1 | n..9 |  |
| &emsp;&emsp;&emsp;`Gebdat` | Geboortedatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Achternaam` | Achternaam/Achternamen | 0..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` | Voorletters | 0..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Roepnaam` | Roepnaam | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`GslchtCd` | Geslachtsaanduiding, code | 0..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;`IdWrknmr` | Identificatie werknemer | 1..1 | an..40 |  |
| &emsp;&emsp;**`Dnstvbnd`** | Dienstverband | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`IdDnstvbnd` | Identificatie dienstverband | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`PersNr` | Personeelsnummer | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;**`PrevDienst`** | Preventieve dienst | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`IdPrevDienst` | Identificatie preventieve dienst | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`PreventDienst` | Preventieve dienst, code | 1..1 | an2 | 22 waarden, o.a. 01, 02, 03, 04, 05 … |
| &emsp;&emsp;&emsp;&emsp;`PevDienstToev` | Preventieve dienst toevoeging | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`DatTotPrevD` | Datum uitvoering preventieve dienst | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`VerbPrevDCode` | Verbijzondering prev. dienst, code | 0..1 | an..10 |  |
| &emsp;&emsp;&emsp;&emsp;`VerbPrevDOms` | Verbijz. prev. dienst, omschrijving | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;**`Vrzm`** | Verzuim | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`VrzmgvlId` | Verzuimgeval identificatie | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`DatEerstVrzmdg` | Datum eerste verzuimdag | 1..1 | datum |  |
| &emsp;&emsp;**`Afspraak`** | Afspraak | 0..1 | groep |  |
| &emsp;&emsp;&emsp;`IdAfspraak` | Identificatie  afspraak | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`DatAfspraak` | Datum afspraak | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`TijdAfspraak` | Tijdstip afspraak | 0..1 | tijd |  |
| &emsp;&emsp;&emsp;`DuurAfspraak` | Duur afspraak | 0..1 | n..5,2 |  |
| &emsp;&emsp;&emsp;`StatusAfspraakCd` | Status afspraak, code | 0..1 | an2 | 01, 02, 03, 04, 05, 06 |
| &emsp;&emsp;&emsp;`OmsSrtAfspraak` | Omschrijving soort afspraak | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;**`UitvoerderAfspraak`** | Uitvoerder afspraak | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`Achternaam` | Achternaam/Achternamen | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;&emsp;`Voorl` | Voorletters | 0..1 | an..6 |  |
| &emsp;&emsp;&emsp;&emsp;`Roepnaam` | Roepnaam | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`GslchtCd` | Geslachtsaanduiding, code | 0..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;&emsp;`NmFnct` | Naam functie | 1..1 | an..35 |  |
