# Dienstverbanden

Verzuimstandaard Werkgevers ↔ Arbodiensten, release 2026.

| | |
|---|---|
| Schema | [`xsd/Dienstverbanden.xsd`](../xsd/Dienstverbanden.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/Dienstverbanden/2026` |
| Versie | 2026.0 |
| Elementen | 103 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`Dienstverbanden`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | Bericht, code | 1..1 | an..5 | 00106 |
| &emsp;&emsp;`VnrBrCd` | Versienummer bericht, code | 1..1 | an..5 | 00006 |
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
| &emsp;&emsp;**`Com`** | Communicatie | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`SrtComCd` | Soort communicatie, code | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;`NrCom` | Nummer/adres communicatie | 1..1 | an..512 |  |
| &emsp;&emsp;**`Cntprsn`** | Contactpersoon | 0..9 | groep |  |
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
| &emsp;&emsp;**`Wrknmr`** | Werknemer | 1..* | groep |  |
| &emsp;&emsp;&emsp;`IngdatMut` | Ingangsdatum mutatie | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Gebdat` | Geboortedatum | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`Overldat` | Overlijdensdatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`GslchtCd` | Geslachtsaanduiding, code | 1..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;`NivOpldngCd` | Niveau opleiding, code | 0..1 | an2 | 01, 02, 03, 04, 05, 06, 07, 99 |
| &emsp;&emsp;&emsp;`IdWrknmr` | Identificatie Werknemer | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;`IdWrknmrOud` | Identificatie werknemer oud | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;**`Dnstvbnd`** | Dienstverband | 1..999 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`IngdatMut` | Ingangsdatum mutatie | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`IdDnstvbnd` | Identificatie dienstverband | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`IdDnstvbndOud` | Identificatie dienstverband oud | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`RdEndDnstvbndCd` | Reden einde dienstverband, code | 0..1 | an2 | 01, 03, 05, 06, 08, 09, 10, 99 |
| &emsp;&emsp;&emsp;&emsp;`PersNr` | Personeelsnummer | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`PersNrOud` | Personeelsnummer oud | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`CntrnrArbdnst` | Contractnummer bij Arbo-dienst | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`SrtDnstvbndCd` | Soort dienstverband, code | 0..1 | an2 | 04, 05, 07, 20, 21, 22, 23, 24 |
| &emsp;&emsp;&emsp;&emsp;`Fnctcd` | Functiecode | 0..1 | an..15 |  |
| &emsp;&emsp;&emsp;&emsp;`NmFnct` | Naam functie | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`FsIndFZ` | Code fase indeling F&Z | 0..1 | an..2 | 1, 3, 4, 5, 6, 17, 18, 19, 38, 40, 41, 43 |
| &emsp;&emsp;&emsp;&emsp;`NmOrgeenh` | Naam organisatie-eenheid | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`OrgeenhCd` | Organisatie-eenheid, code | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`OndOrgeenhCd` | Onderdeel van organisatieeenheid, code | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`OndOrgeenhCdNm` | Onderdeel van organisatie-eenheid, naam | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`PcStandplts` | Postcode standplaats | 0..1 | an..9 |  |
| &emsp;&emsp;&emsp;&emsp;`OmsStandplts` | Omschrijving standplaats | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`VrdlngCd` | Verdeling, code | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`CdBepTd` | Code contract onbepaalde / bepaalde tijd | 0..1 | an1 | B, O |
| &emsp;&emsp;&emsp;&emsp;`AantCtrcturenPWk` | Aantal contracturen per week | 0..1 | n..5,2 |  |
| &emsp;&emsp;&emsp;&emsp;`AantUNormWk` | Normuren per week | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;&emsp;`SrtVarWrktdCd` | Soort variabele werktijden, code | 0..1 | an2 | 01, 02, 03, 04 |
| &emsp;&emsp;&emsp;&emsp;`AantLnwchtdgn` | Aantal loonwachtdagen | 0..1 | n..3 |  |
| &emsp;&emsp;&emsp;&emsp;`PrcLndrbtng` | Percentage loondoorbetaling | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;&emsp;**`Arbeidsrelatie`** | Arbeidsrelatie | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IdArbeidsrelatie` | Identificatie arbeidsrelatie | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IdArbeidsrelatieOud` | Identificatie arbeidsrelatie oud | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`PersNr` | Personeelsnummer | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`PersNrOud` | Personeelsnummer oud | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IngdatMut` | Ingangsdatum mutatie | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`AantCtrcturenPWk` | Aantal contracturen per week | 1..1 | n..5,2 |  |
| &emsp;&emsp;&emsp;&emsp;**`Kostenplaats`** | Kostenplaats | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IngdatMut` | Ingangsdatum mutatie | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`NmKostenplaats` | Naam kostenplaats | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`KostenplaatsCd` | Kostenplaats, code | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`OndKostenplaatsCd` | Onderdeel van kostenplaats, code | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`OndKostenplaatsNm` | Onderdeel van kostenplaats, naam | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;**`Cntprsn`** | Contactpersoon | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IdWrknmr` | Identificatie Werknemer | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Persnr` | Personeelsnummer | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Achternaam` | Achternaam/Achternamen | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Voorl` | Voorletters | 1..1 | an..6 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Roepnaam` | Roepnaam | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`GslchtCd` | Geslachtsaanduiding, code | 1..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;&emsp;&emsp;`RolCntprsnCd` | Rol contactpersoon, code | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IdCntctprsn` | Identificatie contactpersoon | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;**`Com`** | Communicatie | 1..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`SrtComCd` | Soort communicatie, code | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`NrCom` | Nummer/adres communicatie | 1..1 | an..512 |  |
