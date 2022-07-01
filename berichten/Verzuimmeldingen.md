# Verzuimmeldingen

Verzuimstandaard Werkgevers ↔ Arbodiensten, release 2022.

| | |
|---|---|
| Schema | [`xsd/Verzuimmeldingen.xsd`](../xsd/Verzuimmeldingen.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/Verzuimmeldingen/2022` |
| Versie | 2022.0 |
| Elementen | 195 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`Verzuimmeldingen`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | an..5 | 1..1 | an..5 | 00100 |
| &emsp;&emsp;`VnrBrCd` | an..5 | 1..1 | an..5 | 00010 |
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
| &emsp;&emsp;`Lhnr` | an..12 | 0..1 | an..12 |  |
| &emsp;&emsp;`IndERDWGA` | a1 | 0..1 | an1 | J, N |
| &emsp;&emsp;`IndERDZW` | a1 | 0..1 | an1 | J, N |
| &emsp;&emsp;**`StrAdrNl`** | Straatadres nederland | 0..9 | groep |  |
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
| &emsp;&emsp;**`Cntprsn`** | Contactpersoon | 0..9 | groep |  |
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
| &emsp;&emsp;**`Wrknmr`** | Werknemer | 1..* | groep |  |
| &emsp;&emsp;&emsp;`IngdatMut` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`SofiNr` | n..9 | 0..1 | n..9 |  |
| &emsp;&emsp;&emsp;`Gebdat` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`Overldat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`SignNm` | an..200 | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` | a..6 | 1..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Voorv` | Copyright SIVI | 0..1 | an..10 |  |
| &emsp;&emsp;&emsp;`Roepnaam` | a..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`TitVNm` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`TitANm` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`NmvrkrCd` | an2 | 1..1 | an2 | 01, 02, 03, 04 |
| &emsp;&emsp;&emsp;`GslchtCd` | an1 | 1..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;`NivOpldngCd` | an2 | 0..1 | an2 | 01, 02, 03, 04, 05, 06, 07, 99 |
| &emsp;&emsp;&emsp;`IdWrknmr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;`IdWrknmrOud` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;**`BnkGiro`** | Bankrekening | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`Iban` | an..34 | 0..1 | an..34 |  |
| &emsp;&emsp;&emsp;&emsp;`Bic` | an..11 | 0..1 | an..11 |  |
| &emsp;&emsp;&emsp;**`Prtnr`** | Partner | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SignNm` | an..200 | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;&emsp;`Voorv` | Copyright SIVI | 0..1 | an..10 |  |
| &emsp;&emsp;&emsp;**`StrAdrNl`** | Straatadres nederland | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtAdrsCd` | an2 | 1..1 | an2 | 01, 06 |
| &emsp;&emsp;&emsp;&emsp;`SrtVrplgadrsCd` | an2 | 0..1 | an2 | 01, 02, 03, 99 |
| &emsp;&emsp;&emsp;&emsp;`NmVrpladrs` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Pc` | an6 | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;&emsp;`Wnpl` | an..24 | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;&emsp;`StraatLang` | an..80 | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;&emsp;`Huisnr` | n..5 | 1..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`HuisToev` | an..4 | 0..1 | an..4 |  |
| &emsp;&emsp;&emsp;**`StrAdrBl`** | Straatadres buitenland | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtAdrsCd` | an2 | 1..1 | an2 | 01, 06 |
| &emsp;&emsp;&emsp;&emsp;`SrtVrplgadrsCd` | an2 | 0..1 | an2 | 01, 02, 03, 99 |
| &emsp;&emsp;&emsp;&emsp;`NmVrpladrs` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`LocomsBtl` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`PcBtl` | an..9 | 0..1 | an..9 |  |
| &emsp;&emsp;&emsp;&emsp;`WnplBtl` | an..24 | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;&emsp;`RegBtl` | an..24 | 0..1 | an..24 |  |
| &emsp;&emsp;&emsp;&emsp;`LandCd` | a2 | 1..1 | an2 |  |
| &emsp;&emsp;&emsp;&emsp;`Landnm` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`StraatLang` | an..80 | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;&emsp;`HuisnrBtl` | an..9 | 1..1 | an..9 |  |
| &emsp;&emsp;&emsp;**`Com`** | Communicatie | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtComCd` | an2 | 1..1 | an2 | 05, 06, 07, 08, 09, 10 |
| &emsp;&emsp;&emsp;&emsp;`NrCom` | an..512 | 1..1 | an..512 |  |
| &emsp;&emsp;&emsp;**`Dnstvbnd`** | Dienstverband | 1..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`IngdatMut` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`IdDnstvbnd` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`IdDnstvbndOud` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`RdEndDnstvbndCd` | an2 | 0..1 | an2 | 01, 03, 05, 06, 08, 09, 10, 99 |
| &emsp;&emsp;&emsp;&emsp;`PersNr` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`PersNrOud` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`CntrnrArbdnst` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`SrtDnstvbndCd` | an2 | 0..1 | an2 | 04, 05, 07, 20, 21, 22, 23, 24 |
| &emsp;&emsp;&emsp;&emsp;`Fnctcd` | Copyright SIVI | 0..1 | an..15 |  |
| &emsp;&emsp;&emsp;&emsp;`NmFnct` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`NmOrgeenh` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`OrgeenhCd` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`OndOrgeenhCd` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`OndOrgeenhCdNm` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`PcStandplts` | an..9 | 0..1 | an..9 |  |
| &emsp;&emsp;&emsp;&emsp;`OmsStandplts` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`VrdlngCd` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`CdBepTd` | an1 | 0..1 | an1 | B, O |
| &emsp;&emsp;&emsp;&emsp;`AantCtrcturenPWk` | n..5,2 | 0..1 | n..5,2 |  |
| &emsp;&emsp;&emsp;&emsp;`AantUNormWk` | n..6,2 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;&emsp;`SrtVarWrktdCd` | an2 | 0..1 | an2 | 01, 02, 03, 04 |
| &emsp;&emsp;&emsp;&emsp;`AantLnwchtdgn` | n..3 | 0..1 | n..3 |  |
| &emsp;&emsp;&emsp;&emsp;`PrcLndrbtng` | n..6,2 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;&emsp;**`Arbeidsrelatie`** | Arbeidsrelatie | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IdArbeidsrelatie` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IdArbeidsrelatieOud` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`PersNr` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`PersNrOud` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Ingdat` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IngdatMut` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`AantCtrcturenPWk` | n..5,2 | 1..1 | n..5,2 |  |
| &emsp;&emsp;&emsp;&emsp;**`Kostenplaats`** | Kostenplaats | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Ingdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IngdatMut` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`NmKostenplaats` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`KostenplaatsCd` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`OndKostenplaatsCd` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`OndKostenplaatsNm` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;**`Vrzm`** | Verzuim | 1..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VrwrkCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IngdatMutVrzm` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IngdatMutVrzmOud` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VrzmgvlId` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VrzmgvlIdOud` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VrzmgvlVnrMld` | n..3 | 1..1 | n..3 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`EndVrzmJN` | a1 | 1..1 | an1 | J, N |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatVrzmWrkgvr` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatEerstVrzmdg` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatEerstVrzmdgOud` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatHrstld` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatHrstldWrkgvr` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatVrwHrstl` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`PrcVrzm` | n..6,2 | 1..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`BijzRdnStartVrzmCd` | an2 | 0..1 | an2 | 01, 02, 03, 04 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`OorzkVrzmCd` | an2 | 1..1 | an2 | 10, 11, 99 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VngntJN` | a1 | 1..1 | an1 | J, N, O |
| &emsp;&emsp;&emsp;&emsp;&emsp;`RdnEndVrzmCd` | an2 | 0..1 | an2 | 01, 03, 04, 05, 07, 08, 09, 10, 11, 12, 99 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`WAZOCd` | an2 | 0..1 | an2 | 01, 02, 03 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`PrcArbther` | n..6,2 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;**`Cntprsn`** | Contactpersoon | 1..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`IdWrknmr` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`Persnr` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`Achternaam` | an..200 | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`Voorl` | a..6 | 0..1 | an..6 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`Roepnaam` | a..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`GslchtCd` | an1 | 0..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`RolCntprsnCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;**`Com`** | Communicatie | 1..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`SrtComCd` | an2 | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`NrCom` | an..512 | 1..1 | an..512 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;**`Actie`** | Actie | 0..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`ActieCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05, 08, 13 |
| &emsp;&emsp;&emsp;&emsp;&emsp;**`VrTkst`** | Vrije tekst | 0..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`VrijeTekst` | an..512 | 1..1 | an..512 |  |
| &emsp;&emsp;&emsp;&emsp;**`Cntprsn`** | Contactpersoon | 1..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IdWrknmr` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Persnr` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Achternaam` | an..200 | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Voorl` | a..6 | 0..1 | an..6 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Roepnaam` | a..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`GslchtCd` | an1 | 0..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;&emsp;&emsp;`RolCntprsnCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;&emsp;**`Com`** | Communicatie | 1..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`SrtComCd` | an2 | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`NrCom` | an..512 | 1..1 | an..512 |  |
