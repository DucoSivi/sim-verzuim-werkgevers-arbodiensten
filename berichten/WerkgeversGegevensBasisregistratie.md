# WerkgeversGegevensBasisregistratie

Verzuimstandaard Werkgevers ↔ Arbodiensten, release 2026.

| | |
|---|---|
| Schema | [`xsd/WerkgeversGegevensBasisregistratie.xsd`](../xsd/WerkgeversGegevensBasisregistratie.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/WerkgeversGegevensBasisregistratie/2026` |
| Versie | 2026.0 |
| Elementen | 159 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`WerkgeversGegevensBasisregistratie`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | Bericht, code | 1..1 | an..5 | 00101 |
| &emsp;&emsp;`VnrBrCd` | Versienummer bericht, code | 1..1 | an..5 | 00009 |
| &emsp;&emsp;`AandatBr` | Aanmaakdatum bericht | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` | Aanmaaktijd bericht | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` | Identificatie inzender | 1..1 | an..40 |  |
| &emsp;&emsp;`GebrSwPakket` | Gebruikt softwarepakket | 1..1 | an..35 |  |
| &emsp;&emsp;`IdOntvngr` | Identificatie ontvanger | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` | Berichtreferentienummer | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` | Test J/N | 1..1 | an1 | J, N |
| &emsp;&emsp;`OntvngstbevJN` | Ontvangstbevestiging gewenst J/N | 1..1 | an1 | J, N |
| &emsp;**`AdmKantoor`** | Administratiekantoor | 0..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | Handelsnaam organisatie | 1..1 | an..100 |  |
| &emsp;&emsp;`InschrijvingsnrKvK` | Inschrijvingsnummer Kamer van Koophandel | 0..1 | n..8 |  |
| &emsp;&emsp;`VestigingsnrHandelsregister` | Vestigingsnummer | 0..1 | n..12 |  |
| &emsp;**`Wrkgvr`** | Werkgever | 1..* | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | Handelsnaam organisatie | 1..1 | an..100 |  |
| &emsp;&emsp;`InschrijvingsnrKvK` | Inschrijvingsnummer Kamer van Koophandel | 0..1 | n..8 |  |
| &emsp;&emsp;`VestigingsnrHandelsregister` | Vestigingsnummer | 0..1 | n..12 |  |
| &emsp;&emsp;`IdWrkgvrArbdnst` | Identificatie werkgever bij arbodienst | 1..1 | an..40 |  |
| &emsp;&emsp;`AansltnrGeguitwlngArbdnst` | Aansluitnummer gegevensuitwisseling Arbodienst | 1..1 | an..70 |  |
| &emsp;&emsp;`IdWrkgvrUWV` | Identificatie werkgever bij UWV | 0..1 | an..40 |  |
| &emsp;&emsp;`Lhnr` | Loonheffingennummer | 1..1 | an..12 |  |
| &emsp;&emsp;`OrgeenhCd` | Organisatie-eenheid, code | 1..1 | an..70 |  |
| &emsp;&emsp;`IndERDWGA` | Indicatie eigenrisicodrager voor de WGA | 0..1 | an1 | J, N |
| &emsp;&emsp;`IngdatERDWGA` | Ingangsdatum ERD WGA | 0..1 | datum |  |
| &emsp;&emsp;`EnddatERDWGA` | Einddatum ERD WGA | 0..1 | datum |  |
| &emsp;&emsp;`IndERDZW` | Indicatie eigenrisicodrager voor de ZW | 0..1 | an1 | J, N |
| &emsp;&emsp;`IngdatERDZW` | Ingangsdatum ERD ZW | 0..1 | datum |  |
| &emsp;&emsp;`EnddatERDZW` | Einddatum ERD ZW | 0..1 | datum |  |
| &emsp;&emsp;**`ArboCntrct`** | Arbocontract | 0..1 | groep |  |
| &emsp;&emsp;&emsp;`Cntrnr` | Contractnummer | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;**`Personeelssterkte`** | Personeelssterkte | 0..999 | groep |  |
| &emsp;&emsp;&emsp;`PeildatPersoneelssterkte` | Peildatum personeelssterkte | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`AantWrknmrs` | Aantal werknemers | 1..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantFTE` | Aantal FTE | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantVrouwelijkeWrknmrs` | Aantal vrouwelijke werknemers | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantVrouwelijkeFTE` | Aantal vrouwelijke FTE | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantMannelijkeWrknmrs` | Aantal mannelijke werknemers | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantMannelijkeFTE` | Aantal mannelijke FTE | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantUrenFTE` | Aantal uren FTE | 0..1 | n..3 |  |
| &emsp;&emsp;**`StrAdrNl`** | Straatadres nederland | 1..9 | groep |  |
| &emsp;&emsp;&emsp;`SrtAdrsCd` | Soort adres, code | 1..1 | an2 | 01, 02, 03, 05 |
| &emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Pc` | Postcode | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;`Wnpl` | Woonplaatsnaam | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;`StraatLang` | Straatnaam_ | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;`Huisnr` | Huisnummer | 1..1 | n..5 |  |
| &emsp;&emsp;&emsp;`HuisToev` | Huisnummertoevoeging | 0..1 | an..4 |  |
| &emsp;&emsp;**`PbadrsNl`** | Postbusadres nederland | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Pc` | Postcode | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;`Wnpl` | Woonplaatsnaam | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;`Pbnr` | Postbusnummer | 1..1 | n..5 |  |
| &emsp;&emsp;**`Com`** | Communicatie | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`SrtComCd` | Soort communicatie, code | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;`NrCom` | Nummer/adres communicatie | 1..1 | an..512 |  |
| &emsp;&emsp;**`Cntprsn`** | Contactpersoon | 1..9 | groep |  |
| &emsp;&emsp;&emsp;`IdWrknmr` | Identificatie Werknemer | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`Persnr` | Personeelsnummer | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`Achternaam` | Achternaam/Achternamen | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` | Voorletters | 1..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Roepnaam` | Roepnaam | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`GslchtCd` | Geslachtsaanduiding, code | 1..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;`RolCntprsnCd` | Rol contactpersoon, code | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;`IdCntctprsn` | Identificatie contactpersoon | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;**`Com`** | Communicatie | 1..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtComCd` | Soort communicatie, code | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;&emsp;`NrCom` | Nummer/adres communicatie | 1..1 | an..512 |  |
| &emsp;&emsp;**`OrgEenh`** | Organisatie eenheid | 0..9999 | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` | Verwerking, code | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`IngdatMut` | Ingangsdatum mutatie | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`NmOrgeenh` | Naam organisatie-eenheid | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;`OrgeenhCd` | Organisatie-eenheid, code | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;`OndOrgeenhCd` | Onderdeel van organisatieeenheid, code | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;`Lhnr` | Loonheffingennummer | 0..1 | an..12 |  |
| &emsp;&emsp;&emsp;**`ArboCntrct`** | Arbocontract | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`Cntrnr` | Contractnummer | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;**`Personeelssterkte`** | Personeelssterkte | 0..999 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`PeildatPersoneelssterkte` | Peildatum personeelssterkte | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`AantWrknmrs` | Aantal werknemers | 1..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantFTE` | Aantal FTE | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantVrouwelijkeWrknmrs` | Aantal vrouwelijke werknemers | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantVrouwelijkeFTE` | Aantal vrouwelijke FTE | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantMannelijkeWrknmrs` | Aantal mannelijke werknemers | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantMannelijkeFTE` | Aantal mannelijke FTE | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantUrenFTE` | Aantal uren FTE | 0..1 | n..3 |  |
| &emsp;&emsp;&emsp;**`StrAdrNl`** | Straatadres nederland | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtAdrsCd` | Soort adres, code | 1..1 | an2 | 01, 02, 03, 05 |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Pc` | Postcode | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;&emsp;`Wnpl` | Woonplaatsnaam | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;&emsp;`StraatLang` | Straatnaam_ | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;&emsp;`Huisnr` | Huisnummer | 1..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`HuisToev` | Huisnummertoevoeging | 0..1 | an..4 |  |
| &emsp;&emsp;&emsp;**`PbadrsNl`** | Postbusadres nederland | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Pc` | Postcode | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;&emsp;`Wnpl` | Woonplaatsnaam | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;&emsp;`Pbnr` | Postbusnummer | 1..1 | n..5 |  |
| &emsp;&emsp;&emsp;**`Cntprsn`** | Contactpersoon | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`IdWrknmr` | Identificatie Werknemer | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`Persnr` | Personeelsnummer | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`Achternaam` | Achternaam/Achternamen | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;&emsp;`Voorl` | Voorletters | 1..1 | an..6 |  |
| &emsp;&emsp;&emsp;&emsp;`Roepnaam` | Roepnaam | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`GslchtCd` | Geslachtsaanduiding, code | 1..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;&emsp;`RolCntprsnCd` | Rol contactpersoon, code | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;`IdCntctprsn` | Identificatie contactpersoon | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;**`Com`** | Communicatie | 1..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`SrtComCd` | Soort communicatie, code | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`NrCom` | Nummer/adres communicatie | 1..1 | an..512 |  |
| &emsp;&emsp;&emsp;**`Vrzkr`** | Verzekeraar/volmacht | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`HndlsnmOrg` | Handelsnaam organisatie | 1..1 | an..100 |  |
| &emsp;&emsp;&emsp;&emsp;`IdVrzkrVolmachtCd` | Identificatie verzekeraar/volmacht, code | 0..1 | an..4 |  |
| &emsp;&emsp;&emsp;&emsp;**`Cntrct`** | Contract | 1..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Cntrnr` | Contractnummer | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`CntrnrPakket` | Contractnummer pakket | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`SrtVrzmvrzCd` | Soort verzuimverzekering, code | 1..1 | an2 | 01, 02 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`AantVrzkrdn` | Aantal verzekerden | 0..1 | n..5 |  |
| &emsp;&emsp;**`Kostenplaats`** | Kostenplaats | 0..9999 | groep |  |
| &emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`IngdatMut` | Ingangsdatum mutatie | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`NmKostenplaats` | Naam kostenplaats | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;`KostenplaatsCd` | Kostenplaats, code | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;`OndKostenplaatsCd` | Onderdeel van kostenplaats, code | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;**`Personeelssterkte`** | Personeelssterkte | 0..999 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`PeildatPersoneelssterkte` | Peildatum personeelssterkte | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`AantWrknmrs` | Aantal werknemers | 1..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantFTE` | Aantal FTE | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantVrouwelijkeWrknmrs` | Aantal vrouwelijke werknemers | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantVrouwelijkeFTE` | Aantal vrouwelijke FTE | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantMannelijkeWrknmrs` | Aantal mannelijke werknemers | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantMannelijkeFTE` | Aantal mannelijke FTE | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantUrenFTE` | Aantal uren FTE | 0..1 | n..3 |  |
| &emsp;&emsp;**`Vrzkr`** | Verzekeraar/volmacht | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`HndlsnmOrg` | Handelsnaam organisatie | 1..1 | an..100 |  |
| &emsp;&emsp;&emsp;`IdVrzkrVolmachtCd` | Identificatie verzekeraar/volmacht, code | 0..1 | an..4 |  |
| &emsp;&emsp;&emsp;**`Cntrct`** | Contract | 1..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`Cntrnr` | Contractnummer | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`CntrnrPakket` | Contractnummer pakket | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`SrtVrzmvrzCd` | Soort verzuimverzekering, code | 1..1 | an2 | 01, 02 |
| &emsp;&emsp;&emsp;&emsp;`AantVrzkrdn` | Aantal verzekerden | 0..1 | n..5 |  |
