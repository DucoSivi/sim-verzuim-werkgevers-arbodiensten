# Medische kaart

Verzuimstandaard Werkgevers ↔ Arbodiensten, release 2024.

| | |
|---|---|
| Schema | [`xsd/MedischeKaart.xsd`](../xsd/MedischeKaart.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/MedischeKaart/2024` |
| Versie | 2024.0 |
| Elementen | 62 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`MedischeKaart`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** |  | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` |  | 1..1 | an..5 | 00501 |
| &emsp;&emsp;`VnrBrCd` |  | 1..1 | an..5 | 00001 |
| &emsp;&emsp;`FunctieBrCd` |  | 1..1 | an2 | 07, 08 |
| &emsp;&emsp;`AandatBr` |  | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` |  | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` |  | 1..1 | an..40 |  |
| &emsp;&emsp;`IdOntvngr` |  | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` |  | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` |  | 1..1 | an1 | J, N |
| &emsp;&emsp;`OntvngstbevJN` |  | 1..1 | an1 | J, N |
| &emsp;**`Wrkgvr`** |  | 0..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` |  | 1..1 | an..100 |  |
| &emsp;&emsp;`InschrijvingsnrKvK` |  | 0..1 | n..8 |  |
| &emsp;&emsp;`VestigingsnrHandelsregister` |  | 0..1 | n..12 |  |
| &emsp;&emsp;`IdWrkgvrArbdnst` |  | 1..1 | an..40 |  |
| &emsp;&emsp;`AansltnrGeguitwlngArbdnst` |  | 1..1 | an..70 |  |
| &emsp;&emsp;`Lhnr` |  | 0..1 | an..12 |  |
| &emsp;**`Document`** |  | 1..9999 | groep |  |
| &emsp;&emsp;`IdDocument` |  | 1..1 | an..40 |  |
| &emsp;&emsp;`IdDocumentOud` |  | 0..1 | an..40 |  |
| &emsp;&emsp;`DatDocument` |  | 1..1 | datum |  |
| &emsp;&emsp;`SrtDocumentCd` |  | 1..1 | an3 | 920, 921 |
| &emsp;&emsp;`BestandTypCd` |  | 0..1 | an2 | 14 waarden, o.a. 01, 02, 03, 04, 05 … |
| &emsp;&emsp;`Bestandsnm` |  | 0..1 | an..70 |  |
| &emsp;&emsp;`Datastring` |  | 1..1 | string |  |
| &emsp;&emsp;**`Wrknmr`** |  | 1..1 | groep |  |
| &emsp;&emsp;&emsp;`SofiNr` |  | 1..1 | n..9 |  |
| &emsp;&emsp;&emsp;`Gebdat` |  | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`Achternaam` |  | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` |  | 1..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Roepnaam` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`GslchtCd` |  | 1..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;`IdWrknmr` |  | 0..1 | an..40 |  |
| &emsp;&emsp;**`Dnstvbnd`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`IdDnstvbnd` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`Ingdat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`PersNr` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;**`PrevDienst`** |  | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`IdPrevDienst` |  | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`PreventDienst` |  | 1..1 | an2 | 22 waarden, o.a. 01, 02, 03, 04, 05 … |
| &emsp;&emsp;&emsp;&emsp;`PevDienstToev` |  | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`DatTotPrevD` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`VerbPrevDCode` |  | 0..1 | an..10 |  |
| &emsp;&emsp;&emsp;&emsp;`VerbPrevDOms` |  | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;**`Vrzm`** |  | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`VrzmgvlId` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`DatEerstVrzmdg` |  | 1..1 | datum |  |
| &emsp;&emsp;**`Afspraak`** |  | 0..1 | groep |  |
| &emsp;&emsp;&emsp;`IdAfspraak` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`DatAfspraak` |  | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`TijdAfspraak` |  | 0..1 | tijd |  |
| &emsp;&emsp;&emsp;`DuurAfspraak` |  | 0..1 | n..5,2 |  |
| &emsp;&emsp;&emsp;`StatusAfspraakCd` |  | 0..1 | an2 | 01, 02, 03, 04, 05, 06 |
| &emsp;&emsp;&emsp;`OmsSrtAfspraak` |  | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;**`UitvoerderAfspraak`** |  | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`Achternaam` |  | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;&emsp;`Voorl` |  | 0..1 | an..6 |  |
| &emsp;&emsp;&emsp;&emsp;`Roepnaam` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`GslchtCd` |  | 0..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;&emsp;`NmFnct` |  | 1..1 | an..35 |  |
