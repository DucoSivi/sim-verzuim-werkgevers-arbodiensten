# Afspraken

Verzuimstandaard Werkgevers ↔ Arbodiensten, release 2022.

| | |
|---|---|
| Schema | [`xsd/Afspraken.xsd`](../xsd/Afspraken.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/Afspraken/2022` |
| Versie | 2022.0 |
| Elementen | 65 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`Afspraken`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | an..5 | 1..1 | an..5 | 00105 |
| &emsp;&emsp;`VnrBrCd` | an..5 | 1..1 | an..5 | 00004 |
| &emsp;&emsp;`AandatBr` | an10 | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` | an8 | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`GebrSwPakket` | an..35 | 1..1 | an..35 |  |
| &emsp;&emsp;`IdOntvngr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` | an..512 | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` | a1 | 1..1 | an1 | J, N |
| &emsp;&emsp;`OntvngstbevJN` | a1 | 1..1 | an1 | J, N |
| &emsp;**`Werkgever`** |  | 0..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | an..100 | 1..1 | an..100 |  |
| &emsp;&emsp;`InschrijvingsnrKvK` | n..8 | 0..1 | n..8 |  |
| &emsp;&emsp;`IdWrkgvrArbdnst` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`AansltnrGeguitwlngArbdnst` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;`Lhnr` | an..12 | 1..1 | an..12 |  |
| &emsp;**`Arbodienst`** |  | 0..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | an..100 | 1..1 | an..100 |  |
| &emsp;&emsp;`IdArbdnst` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;**`Contactpersoon`** |  | 0..1 | groep |  |
| &emsp;&emsp;&emsp;`Achternaam` | an..200 | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` | a..6 | 0..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Roepnaam` | a..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`GslchtCd` | an1 | 0..1 | an1 | M, V |
| &emsp;&emsp;&emsp;**`Communicatie`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtComCd` | Copyright SIVI | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;&emsp;`NrCom` | an..512 | 1..1 | an..512 |  |
| &emsp;**`Afspraak`** | Afspraak | 1..999 | groep |  |
| &emsp;&emsp;`IdAfspraak` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`IdAfspraakOud` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;`DatAfspraak` | an10 | 1..1 | datum |  |
| &emsp;&emsp;`DatAfspraakOud` | an10 | 0..1 | datum |  |
| &emsp;&emsp;`TijdAfspraak` | an8 | 1..1 | tijd |  |
| &emsp;&emsp;`TijdAfspraakOud` | an8 | 0..1 | tijd |  |
| &emsp;&emsp;`DuurAfspraak` | n..5,2 | 0..1 | n..5,2 |  |
| &emsp;&emsp;`StatusAfspraakCd` | an2 | 0..1 | an2 | 01, 02, 03, 04, 05, 06 |
| &emsp;&emsp;`OmsSrtAfspraak` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;**`Wrknmr`** | Werknemer | 1..1 | groep |  |
| &emsp;&emsp;&emsp;`SofiNr` | n..9 | 0..1 | n..9 |  |
| &emsp;&emsp;&emsp;`Gebdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Overldat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Achternaam` | an..200 | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` | a..6 | 0..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Roepnaam` | a..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`GslchtCd` | an1 | 0..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;`IdWrknmr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;**`StraatadresNederland`** |  | 0..1 | groep |  |
| &emsp;&emsp;&emsp;`Pc` | an6 | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;`Wnpl` | an..24 | 0..1 | an..24 |  |
| &emsp;&emsp;&emsp;`StraatLang` | an..80 | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;`Huisnr` | n..5 | 1..1 | n..5 |  |
| &emsp;&emsp;&emsp;`HuisToev` | an..4 | 0..1 | an..4 |  |
| &emsp;&emsp;**`UitvoerderAfspraak`** | Uitvoerder afspraak | 1..1 | groep |  |
| &emsp;&emsp;&emsp;`Achternaam` | an..200 | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` | a..6 | 0..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Roepnaam` | a..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`GslchtCd` | an1 | 0..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;`NmFnct` | an..35 | 1..1 | an..35 |  |
| &emsp;&emsp;**`Dienstverband`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`IdDnstvbnd` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`PersNr` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;**`Verzuim`** |  | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`DatEerstVrzmdg` | an10 | 1..1 | datum |  |
