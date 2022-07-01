# Documenten

Verzuimstandaard Werkgevers ↔ Arbodiensten, release 2022.

| | |
|---|---|
| Schema | [`xsd/Documenten.xsd`](../xsd/Documenten.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/Documenten/2022` |
| Versie | 2022.0 |
| Elementen | 83 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`Documenten`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | an..5 | 1..1 | an..5 | 00500 |
| &emsp;&emsp;`VnrBrCd` | an..5 | 1..1 | an..5 | 00005 |
| &emsp;&emsp;`AandatBr` | an10 | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` | an8 | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`IdOntvngr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` | an..512 | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` | a1 | 1..1 | an1 | J, N |
| &emsp;&emsp;`OntvngstbevJN` | a1 | 1..1 | an1 | J, N |
| &emsp;**`Wrkgvr`** | Werkgever | 0..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | an..100 | 1..1 | an..100 |  |
| &emsp;&emsp;`InschrijvingsnrKvK` | n..8 | 0..1 | n..8 |  |
| &emsp;&emsp;`VestigingsnrHandelsregister` | n..12 | 0..1 | n..12 |  |
| &emsp;&emsp;`IdWrkgvrArbdnst` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`AansltnrGeguitwlngArbdnst` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;`Lhnr` | an..12 | 0..1 | an..12 |  |
| &emsp;**`CntprsnOntvanger`** | Contactpersoon ontvanger | 0..1 | groep |  |
| &emsp;&emsp;`Achternaam` | an..200 | 1..1 | an..200 |  |
| &emsp;&emsp;`Voorl` | a..6 | 0..1 | an..6 |  |
| &emsp;&emsp;`Roepnaam` | a..35 | 0..1 | an..35 |  |
| &emsp;&emsp;`GslchtCd` | an1 | 0..1 | an1 | M, O, V |
| &emsp;&emsp;**`Com`** | Communicatie | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`SrtComCd` | an2 | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;`NrCom` | an..512 | 1..1 | an..512 |  |
| &emsp;**`CntprsnZender`** | Contactpersoon zender | 0..1 | groep |  |
| &emsp;&emsp;`Achternaam` | an..200 | 1..1 | an..200 |  |
| &emsp;&emsp;`Voorl` | a..6 | 0..1 | an..6 |  |
| &emsp;&emsp;`Roepnaam` | a..35 | 0..1 | an..35 |  |
| &emsp;&emsp;`GslchtCd` | an1 | 0..1 | an1 | M, O, V |
| &emsp;&emsp;**`Com`** | Communicatie | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`SrtComCd` | an2 | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;`NrCom` | an..512 | 1..1 | an..512 |  |
| &emsp;**`Document`** | Document | 1..9999 | groep |  |
| &emsp;&emsp;`IdDocument` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`IdDocumentOud` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;`DatDocument` | an10 | 1..1 | datum |  |
| &emsp;&emsp;`SrtDocumentCd` | an3 | 1..1 | an3 | 23 waarden, o.a. 100, 104, 158, 208, 215 … |
| &emsp;&emsp;`SrtDocumentOms` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;`StatDocumentCd` | an2 | 0..1 | an2 | 01, 02 |
| &emsp;&emsp;`KenmerkZendPartij` | Copyright SIVI | 1..1 | an..512 |  |
| &emsp;&emsp;`RdAanlevDocumentCd` | an2 | 0..1 | an2 | 01, 02, 03 |
| &emsp;&emsp;`PrioriteitCd` | an2 | 0..1 | an2 | 01, 02, 03 |
| &emsp;&emsp;`BestandTypCd` | an2 | 0..1 | an2 | 14 waarden, o.a. 01, 02, 03, 04, 05 … |
| &emsp;&emsp;`Bestandsnm` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;`AdresseringCd` | an2 | 0..1 | an2 | 01, 02, 03 |
| &emsp;&emsp;`Datastring` | an..* | 1..1 | string |  |
| &emsp;&emsp;**`Wrknmr`** | Werknemer | 1..1 | groep |  |
| &emsp;&emsp;&emsp;`SofiNr` | n..9 | 0..1 | n..9 |  |
| &emsp;&emsp;&emsp;`Gebdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Achternaam` | an..200 | 0..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` | a..6 | 0..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Roepnaam` | a..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`GslchtCd` | an1 | 0..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;`IdWrknmr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;**`Dnstvbnd`** | Dienstverband | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`IdDnstvbnd` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`Ingdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`PersNr` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;**`PrevDienst`** | Preventieve dienst | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`IdPrevDienst` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`PreventDienst` | an2 | 1..1 | an2 | 22 waarden, o.a. 01, 02, 03, 04, 05 … |
| &emsp;&emsp;&emsp;&emsp;`PevDienstToev` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`DatTotPrevD` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`VerbPrevDCode` | an..10 | 0..1 | an..10 |  |
| &emsp;&emsp;&emsp;&emsp;`VerbPrevDOms` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;**`Vrzm`** | Verzuim | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`VrzmgvlId` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`DatEerstVrzmdg` | an10 | 1..1 | datum |  |
| &emsp;&emsp;**`Afspraak`** | Afspraak | 0..1 | groep |  |
| &emsp;&emsp;&emsp;`IdAfspraak` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`DatAfspraak` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`TijdAfspraak` | an8 | 0..1 | tijd |  |
| &emsp;&emsp;&emsp;`DuurAfspraak` | n..5,2 | 0..1 | n..5,2 |  |
| &emsp;&emsp;&emsp;`StatusAfspraakCd` | an2 | 0..1 | an2 | 01, 02, 03, 04, 05, 06 |
| &emsp;&emsp;&emsp;`OmsSrtAfspraak` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;**`UitvoerderAfspraak`** | Uitvoerder afspraak | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`Achternaam` | an..200 | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;&emsp;`Voorl` | a..6 | 0..1 | an..6 |  |
| &emsp;&emsp;&emsp;&emsp;`Roepnaam` | a..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`GslchtCd` | an1 | 0..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;&emsp;`NmFnct` | an..35 | 1..1 | an..35 |  |
