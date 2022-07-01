# Retourmelding

Verzuimstandaard Werkgevers ↔ Arbodiensten, release 2022.

| | |
|---|---|
| Schema | [`xsd/Retourmelding1.xsd`](../xsd/Retourmelding1.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/Retourmelding1/2022` |
| Versie | 2022.0 |
| Elementen | 17 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`Retourmelding1`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | an..5 | 1..1 | an..5 | 99999 |
| &emsp;&emsp;`VnrBrCd` | an..5 | 1..1 | an..5 | 00002 |
| &emsp;&emsp;`AandatBr` | an10 | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` | an8 | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`GebrSwPakket` | an..35 | 1..1 | an..35 |  |
| &emsp;&emsp;`IdOntvngr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` | an..512 | 1..1 | an..512 |  |
| &emsp;&emsp;`BerrefnrIngzndnBer` | an..512 | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` | a1 | 1..1 | an1 | J, N |
| &emsp;&emsp;`OntvngstbevJN` | a1 | 1..1 | an1 | J, N |
| &emsp;&emsp;`SrtRetmldngCd` | an2 | 1..1 | an2 | 01, 02, 03, 04 |
| &emsp;**`Foutmldng`** | Foutmelding | 0..* | groep |  |
| &emsp;&emsp;`SrtFoutCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05, 06, 99 |
| &emsp;&emsp;`Toelchtng` | an..512 | 0..1 | an..512 |  |
