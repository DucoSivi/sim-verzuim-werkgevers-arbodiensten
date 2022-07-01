# WerkgeversGegevensBasisregistratie

Verzuimstandaard Werkgevers ↔ Arbodiensten, release 2022.

| | |
|---|---|
| Schema | [`xsd/WerkgeversGegevensBasisregistratie.xsd`](../xsd/WerkgeversGegevensBasisregistratie.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/WerkgeversGegevensBasisregistratie/2022` |
| Versie | 2022.0 |
| Elementen | 157 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`WerkgeversGegevensBasisregistratie`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | an..5 | 1..1 | an..5 | 00101 |
| &emsp;&emsp;`VnrBrCd` | an..5 | 1..1 | an..5 | 00008 |
| &emsp;&emsp;`AandatBr` | an10 | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` | an8 | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`GebrSwPakket` | an..35 | 1..1 | an..35 |  |
| &emsp;&emsp;`IdOntvngr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` | an..512 | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` | a1 | 1..1 | an1 | J, N |
| &emsp;&emsp;`OntvngstbevJN` | a1 | 1..1 | an1 | J, N |
| &emsp;**`AdmKantoor`** | Administratiekantoor | 0..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | an..100 | 1..1 | an..100 |  |
| &emsp;&emsp;`InschrijvingsnrKvK` | n..8 | 0..1 | n..8 |  |
| &emsp;&emsp;`VestigingsnrHandelsregister` | n..12 | 0..1 | n..12 |  |
| &emsp;**`Wrkgvr`** | Werkgever | 1..* | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | an..100 | 1..1 | an..100 |  |
| &emsp;&emsp;`InschrijvingsnrKvK` | n..8 | 0..1 | n..8 |  |
| &emsp;&emsp;`VestigingsnrHandelsregister` | n..12 | 0..1 | n..12 |  |
| &emsp;&emsp;`IdWrkgvrArbdnst` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`AansltnrGeguitwlngArbdnst` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;`IdWrkgvrUWV` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;`Lhnr` | an..12 | 1..1 | an..12 |  |
| &emsp;&emsp;`OrgeenhCd` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;`IndERDWGA` | a1 | 0..1 | an1 | J, N |
| &emsp;&emsp;`IngdatERDWGA` | an10 | 0..1 | datum |  |
| &emsp;&emsp;`EnddatERDWGA` | an10 | 0..1 | datum |  |
| &emsp;&emsp;`IndERDZW` | a1 | 0..1 | an1 | J, N |
| &emsp;&emsp;`IngdatERDZW` | an10 | 0..1 | datum |  |
| &emsp;&emsp;`EnddatERDZW` | an10 | 0..1 | datum |  |
| &emsp;&emsp;**`ArboCntrct`** | Arbocontract | 0..1 | groep |  |
| &emsp;&emsp;&emsp;`Cntrnr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;`Ingdat` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;**`Personeelssterkte`** | Personeelssterkte | 0..999 | groep |  |
| &emsp;&emsp;&emsp;`PeildatPersoneelssterkte` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`AantWrknmrs` | n..7 | 1..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantFTE` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantVrouwelijkeWrknmrs` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantVrouwelijkeFTE` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantMannelijkeWrknmrs` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantMannelijkeFTE` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantUrenFTE` | n..3 | 0..1 | n..3 |  |
| &emsp;&emsp;**`StrAdrNl`** | Straatadres nederland | 1..9 | groep |  |
| &emsp;&emsp;&emsp;`SrtAdrsCd` | an2 | 1..1 | an2 | 01, 02, 03, 05 |
| &emsp;&emsp;&emsp;`Ingdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Pc` | an6 | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;`Wnpl` | an..24 | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;`StraatLang` | an..80 | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;`Huisnr` | n..5 | 1..1 | n..5 |  |
| &emsp;&emsp;&emsp;`HuisToev` | an..4 | 0..1 | an..4 |  |
| &emsp;&emsp;**`PbadrsNl`** | Postbusadres nederland | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`Ingdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Pc` | an6 | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;`Wnpl` | an..24 | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;`Pbnr` | n..5 | 1..1 | n..5 |  |
| &emsp;&emsp;**`Com`** | Communicatie | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`SrtComCd` | an2 | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;`NrCom` | an..512 | 1..1 | an..512 |  |
| &emsp;&emsp;**`Cntprsn`** | Contactpersoon | 1..9 | groep |  |
| &emsp;&emsp;&emsp;`IdWrknmr` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`Persnr` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`Achternaam` | an..200 | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` | a..6 | 0..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Roepnaam` | a..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`GslchtCd` | an1 | 0..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;`RolCntprsnCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;**`Com`** | Communicatie | 1..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtComCd` | an2 | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;&emsp;`NrCom` | an..512 | 1..1 | an..512 |  |
| &emsp;&emsp;**`OrgEenh`** | Organisatie eenheid | 0..9999 | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;`Ingdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`IngdatMut` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`NmOrgeenh` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;`OrgeenhCd` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;`OndOrgeenhCd` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;`Lhnr` | an..12 | 0..1 | an..12 |  |
| &emsp;&emsp;&emsp;**`ArboCntrct`** | Arbocontract | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`Cntrnr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;**`Personeelssterkte`** | Personeelssterkte | 0..999 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`PeildatPersoneelssterkte` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`AantWrknmrs` | n..7 | 1..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantFTE` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantVrouwelijkeWrknmrs` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantVrouwelijkeFTE` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantMannelijkeWrknmrs` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantMannelijkeFTE` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantUrenFTE` | n..3 | 0..1 | n..3 |  |
| &emsp;&emsp;&emsp;**`StrAdrNl`** | Straatadres nederland | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtAdrsCd` | an2 | 1..1 | an2 | 01, 02, 03, 05 |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Pc` | an6 | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;&emsp;`Wnpl` | an..24 | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;&emsp;`StraatLang` | an..80 | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;&emsp;`Huisnr` | n..5 | 1..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`HuisToev` | an..4 | 0..1 | an..4 |  |
| &emsp;&emsp;&emsp;**`PbadrsNl`** | Postbusadres nederland | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Pc` | an6 | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;&emsp;`Wnpl` | an..24 | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;&emsp;`Pbnr` | n..5 | 1..1 | n..5 |  |
| &emsp;&emsp;&emsp;**`Cntprsn`** | Contactpersoon | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`IdWrknmr` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`Persnr` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`Achternaam` | an..200 | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;&emsp;`Voorl` | a..6 | 0..1 | an..6 |  |
| &emsp;&emsp;&emsp;&emsp;`Roepnaam` | a..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`GslchtCd` | an1 | 0..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;&emsp;`RolCntprsnCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;**`Com`** | Communicatie | 1..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`SrtComCd` | an2 | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`NrCom` | an..512 | 1..1 | an..512 |  |
| &emsp;&emsp;&emsp;**`Vrzkr`** | Verzekeraar/volmacht | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`HndlsnmOrg` | an..100 | 1..1 | an..100 |  |
| &emsp;&emsp;&emsp;&emsp;`IdVrzkrVolmachtCd` | an..4 | 0..1 | an..4 |  |
| &emsp;&emsp;&emsp;&emsp;**`Cntrct`** | Contract | 1..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Cntrnr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`CntrnrPakket` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Ingdat` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`SrtVrzmvrzCd` | an2 | 1..1 | an2 | 01, 02 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`AantVrzkrdn` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;**`Kostenplaats`** | Kostenplaats | 0..9999 | groep |  |
| &emsp;&emsp;&emsp;`Ingdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`IngdatMut` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`NmKostenplaats` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;`KostenplaatsCd` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;`OndKostenplaatsCd` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;**`Personeelssterkte`** | Personeelssterkte | 0..999 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`PeildatPersoneelssterkte` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`AantWrknmrs` | n..7 | 1..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantFTE` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantVrouwelijkeWrknmrs` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantVrouwelijkeFTE` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantMannelijkeWrknmrs` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantMannelijkeFTE` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantUrenFTE` | n..3 | 0..1 | n..3 |  |
| &emsp;&emsp;**`Vrzkr`** | Verzekeraar/volmacht | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`HndlsnmOrg` | an..100 | 1..1 | an..100 |  |
| &emsp;&emsp;&emsp;`IdVrzkrVolmachtCd` | an..4 | 0..1 | an..4 |  |
| &emsp;&emsp;&emsp;**`Cntrct`** | Contract | 1..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`Cntrnr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`CntrnrPakket` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`SrtVrzmvrzCd` | an2 | 1..1 | an2 | 01, 02 |
| &emsp;&emsp;&emsp;&emsp;`AantVrzkrdn` | n..5 | 0..1 | n..5 |  |
