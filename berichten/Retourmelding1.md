# Retourmelding

Verzuimstandaard Werkgevers ↔ Arbodiensten, release 2025.

| | |
|---|---|
| Schema | [`xsd/Retourmelding1.xsd`](../xsd/Retourmelding1.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/Retourmelding1/2025` |
| Versie | 2025.0 |
| Elementen | 17 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`Retourmelding1`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | Bericht, code | 1..1 | an..5 | 99999 |
| &emsp;&emsp;`VnrBrCd` | Versienummer bericht, code | 1..1 | an..5 | 00003 |
| &emsp;&emsp;`AandatBr` | Aanmaakdatum bericht | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` | Aanmaaktijd bericht | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` | Identificatie inzender | 1..1 | an..40 |  |
| &emsp;&emsp;`GebrSwPakket` | Gebruikt softwarepakket | 1..1 | an..35 |  |
| &emsp;&emsp;`IdOntvngr` | Identificatie ontvanger | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` | Berichtreferentienummer | 1..1 | an..512 |  |
| &emsp;&emsp;`BerrefnrIngzndnBer` | Berichtreferentienummer ingezonden bericht | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` | Test J/N | 1..1 | an1 | J, N |
| &emsp;&emsp;`OntvngstbevJN` | Ontvangstbevestiging gewenst J/N | 1..1 | an1 | J, N |
| &emsp;&emsp;`SrtRetmldngCd` | Soort retourmelding, code | 1..1 | an2 | 02, 03 |
| &emsp;**`Foutmldng`** | Foutmelding | 0..* | groep |  |
| &emsp;&emsp;`SrtFoutCd` | Soort fout, code | 1..1 | an2 | 01, 06, 99 |
| &emsp;&emsp;`Toelchtng` | Toelichting | 0..1 | an..512 |  |
