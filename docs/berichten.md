# Berichtenspecificatie: SIVI Verzuim: Werkgevers ↔ Arbodiensten

De berichten in dit koppelvlak zijn gedefinieerd met XML Schema Definition (XSD). 

---

## Schema-overzicht

De schema's zijn te vinden in de repository onder de map [`schema/`](https://github.com/DucoSivi/sim-verzuim-werkgevers-arbodiensten/tree/main/schema):

| Schemabestand | Doel | Hoofdelement |
|:---|:---|:---|
| [`Verzuimmeldingen2026.xsd`](https://github.com/DucoSivi/sim-verzuim-werkgevers-arbodiensten/blob/main/schema/Verzuimmeldingen2026.xsd) | Primaire transactie | Rootbericht |
| [`WerknemerDienstverband2026.xsd`](https://github.com/DucoSivi/sim-verzuim-werkgevers-arbodiensten/blob/main/schema/WerknemerDienstverband2026.xsd) | Ondersteunende transactie | Secundair bericht |

---

## Voorbeeldberichten

Onder `schema/voorbeelden/` zijn representatieve testberichten opgenomen:
* `voorbeeld-ziekmelding.xml`
* `voorbeeld-dienstverband.xml`

### Voorbeeldfragment (`Verzuimmeldingen2026.xsd`)

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SIVIVerzuimBericht xmlns="http://www.sivi.org/verzuim/2026"
                   xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
    <Kop>
        <BerichtID>20261001-90124</BerichtID>
        <Aanmaakdatum>2026-10-01T12:00:00</Aanmaakdatum>
        <Koppelvlak>sim-verzuim-werkgevers-arbodiensten</Koppelvlak>
    </Kop>
    <Inhoud>
        <Status>Actief</Status>
    </Inhoud>
</SIVIVerzuimBericht>
```
