# Implementatie & Kwaliteit

Praktische richtlijnen voor softwareontwikkelaars en integratiespecialisten die aansluiten op het koppelvlak `sim-verzuim-werkgevers-arbodiensten`.

---

## 1. Validatieregels
1. **XSD-validatie:** Elk uitgewisseld XML-bestand dient foutloos te valideren tegen `Verzuimmeldingen2026.xsd` en de bijbehorende deelschema's.
2. **Codelijstconsistentie:** Waarden in codelijstelementen moeten exact matchen met de gedefinieerde numerieke en alfanumerieke codes.
3. **AVG en Gegevensbescherming:**
    * Medische gegevens mogen onder GEEN beding in berichten naar de werkgever of verzekeraar worden opgenomen.
    * Slechts functionele beperkingen (bijv. 'niet tillen boven 10kg', 'halve dagen beeldschermwerk') mogen worden uitgewisseld.

---

## 2. Transport & Beveiliging
* **Protocol:** RESTful HTTPS API met MTLS (Mutual TLS) of API-sleutels via OAuth2 Bearer tokens.
* **Payload:** UTF-8 gecodeerde XML conform de SIVI-standaard.
* **Idempotentie:** Elk bericht dient een unieke `BerichtID` te bevatten om dubbele verwerking bij netwerkhaperingen te voorkomen.

---

## 3. Testen & Sandbox
Softwareleveranciers kunnen gebruikmaken van de referentieberichten in de repository onder `schema/voorbeelden/` voor ketentests.
