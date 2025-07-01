# Afspraken

Verzuimstandaard Werkgevers ↔ Arbodiensten, release 2025.

| | |
|---|---|
| Schema | [`xsd/Afspraken.xsd`](../xsd/Afspraken.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/Afspraken/2025` |
| Versie | 2025.0 |
| Elementen | 65 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`Afspraken`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | Bericht, code | 1..1 | an..5 | 00105 |
| &emsp;&emsp;`VnrBrCd` | Versienummer bericht, code | 1..1 | an..5 | 00005 |
| &emsp;&emsp;`AandatBr` | Aanmaakdatum bericht | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` | Aanmaaktijd bericht | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` | Identificatie inzender | 1..1 | an..40 |  |
| &emsp;&emsp;`GebrSwPakket` | Gebruikt softwarepakket | 1..1 | an..35 |  |
| &emsp;&emsp;`IdOntvngr` | Identificatie ontvanger | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` | Berichtreferentienummer | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` | Test J/N | 1..1 | an1 | J, N |
| &emsp;&emsp;`OntvngstbevJN` | Ontvangstbevestiging gewenst J/N | 1..1 | an1 | J, N |
| &emsp;**`Werkgever`** |  | 0..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | Handelsnaam organisatie | 1..1 | an..100 |  |
| &emsp;&emsp;`InschrijvingsnrKvK` | Inschrijvingsnummer Kamer van Koophandel | 0..1 | n..8 |  |
| &emsp;&emsp;`IdWrkgvrArbdnst` | Identificatie werkgever bij arbodienst | 1..1 | an..40 |  |
| &emsp;&emsp;`AansltnrGeguitwlngArbdnst` | Aansluitnummer gegevensuitwisseling Arbodienst | 1..1 | an..70 |  |
| &emsp;&emsp;`Lhnr` | Loonheffingennummer | 1..1 | an..12 |  |
| &emsp;**`Arbodienst`** |  | 0..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | Handelsnaam organisatie | 1..1 | an..100 |  |
| &emsp;&emsp;`IdArbdnst` | Identificatie Arbo-dienst | 0..1 | an..40 |  |
| &emsp;&emsp;**`Contactpersoon`** |  | 0..1 | groep |  |
| &emsp;&emsp;&emsp;`Achternaam` | Achternaam/Achternamen | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` | Voorletters | 1..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Roepnaam` | Roepnaam | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`GslchtCd` | Geslachtsaanduiding, code | 1..1 | an1 | M, V |
| &emsp;&emsp;&emsp;**`Communicatie`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtComCd` | Copyright SIVI | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;&emsp;`NrCom` | Nummer/adres communicatie | 1..1 | an..512 |  |
| &emsp;**`Afspraak`** | Afspraak | 1..999 | groep |  |
| &emsp;&emsp;`IdAfspraak` | Identificatie  afspraak | 1..1 | an..40 |  |
| &emsp;&emsp;`IdAfspraakOud` | Identificatie afspraak oud | 0..1 | an..40 |  |
| &emsp;&emsp;`DatAfspraak` | Datum afspraak | 1..1 | datum |  |
| &emsp;&emsp;`DatAfspraakOud` | Datum  afspraak oud | 0..1 | datum |  |
| &emsp;&emsp;`TijdAfspraak` | Tijdstip afspraak | 1..1 | tijd |  |
| &emsp;&emsp;`TijdAfspraakOud` | Tijdstip afspraak oud | 0..1 | tijd |  |
| &emsp;&emsp;`DuurAfspraak` | Duur afspraak | 0..1 | n..5,2 |  |
| &emsp;&emsp;`StatusAfspraakCd` | Status afspraak, code | 0..1 | an2 | 01, 02, 03, 04, 05, 06 |
| &emsp;&emsp;`OmsSrtAfspraak` | Omschrijving soort afspraak | 1..1 | an..70 |  |
| &emsp;&emsp;**`Wrknmr`** | Werknemer | 1..1 | groep |  |
| &emsp;&emsp;&emsp;`SofiNr` | Burgerservicenummer | 0..1 | n..9 |  |
| &emsp;&emsp;&emsp;`Gebdat` | Geboortedatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Overldat` | Overlijdensdatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Achternaam` | Achternaam/Achternamen | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` | Voorletters | 0..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Roepnaam` | Roepnaam | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`GslchtCd` | Geslachtsaanduiding, code | 0..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;`IdWrknmr` | Identificatie werknemer | 1..1 | an..40 |  |
| &emsp;&emsp;**`StraatadresNederland`** |  | 0..1 | groep |  |
| &emsp;&emsp;&emsp;`Pc` | Postcode | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;`Wnpl` | Woonplaatsnaam | 0..1 | an..24 |  |
| &emsp;&emsp;&emsp;`StraatLang` | Straatnaam_ | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;`Huisnr` | Huisnummer | 1..1 | n..5 |  |
| &emsp;&emsp;&emsp;`HuisToev` | Huisnummertoevoeging | 0..1 | an..4 |  |
| &emsp;&emsp;**`UitvoerderAfspraak`** | Uitvoerder afspraak | 1..1 | groep |  |
| &emsp;&emsp;&emsp;`Achternaam` | Achternaam/Achternamen | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` | Voorletters | 0..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Roepnaam` | Roepnaam | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`GslchtCd` | Geslachtsaanduiding, code | 0..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;`NmFnct` | Naam functie | 1..1 | an..35 |  |
| &emsp;&emsp;**`Dienstverband`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`IdDnstvbnd` | Identificatie dienstverband | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`PersNr` | Personeelsnummer | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;**`Verzuim`** |  | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`DatEerstVrzmdg` | Datum eerste verzuimdag | 1..1 | datum |  |
