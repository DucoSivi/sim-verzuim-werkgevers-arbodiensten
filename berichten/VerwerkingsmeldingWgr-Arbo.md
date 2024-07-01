# Verwerkingsmelding werkgever - arbodienst

Verzuimstandaard Werkgevers ↔ Arbodiensten, release 2024.

| | |
|---|---|
| Schema | [`xsd/VerwerkingsmeldingWgr-Arbo.xsd`](../xsd/VerwerkingsmeldingWgr-Arbo.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/VerwerkingsmeldingWerkgeverArbodienst/2024` |
| Versie | 2024.0 |
| Elementen | 23 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`VerwerkingsmeldingWerkgeverArbodienst`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | Bericht, code | 1..1 | an..5 |  |
| &emsp;&emsp;`VnrBrCd` | Versienummer bericht, code | 1..1 | an..5 |  |
| &emsp;&emsp;`AandatBr` | Aanmaakdatum bericht | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` | Aanmaaktijd bericht | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` | Identificatie inzender | 1..1 | an..40 |  |
| &emsp;&emsp;`GebrSwPakket` | Gebruikt softwarepakket | 1..1 | an..35 |  |
| &emsp;&emsp;`IdOntvngr` | Identificatie ontvanger | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` | Berichtreferentienummer | 1..1 | an..512 |  |
| &emsp;&emsp;`BerrefnrIngzndnBer` | Berichtreferentienummer ingezonden bericht | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` | Test J/N | 1..1 | an1 |  |
| &emsp;&emsp;`OntvngstbevJN` | Ontvangstbevestiging gewenst J/N | 1..1 | an1 |  |
| &emsp;**`VrwrkMld`** | Verwerkingsmelding | 1..* | groep |  |
| &emsp;&emsp;`VrwrkbhdCd` | Verwerkbaarheid, code | 1..1 | an2 | 01, 02, 03 |
| &emsp;&emsp;`VrzmgvlId` | Verzuimgeval identificatie | 1..1 | an..40 |  |
| &emsp;&emsp;`VrzmgvlVnrMld` | Verzuimgeval volgnummer melding | 1..1 | n..3 |  |
| &emsp;&emsp;`AansltnrGeguitwlngArbdnst` | Aansluitnummer gegevensuitwisseling Arbodienst | 1..1 | an..70 |  |
| &emsp;&emsp;`IdWrkgvrArbdnst` | Identificatie werkgever bij arbodienst | 1..1 | an..40 |  |
| &emsp;&emsp;`CtrlCd` | Controle, code | 1..1 | an5 |  |
| &emsp;&emsp;`MldngTkst` | Meldingstekst | 1..1 | an..512 |  |
| &emsp;&emsp;**`VrTkst`** | Vrije tekst | 0..1 | groep |  |
| &emsp;&emsp;&emsp;`VrijeTekst` | Vrije tekst | 1..1 | an..512 |  |
