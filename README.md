# Verzuimstandaard Werkgevers ↔ Arbodiensten

> **Simulatie.** Zo zou dit koppelvlak er op GitHub uitzien in de voorgestelde inrichting: één centrale ingang ([sim-verzuim-standaard](https://github.com/DucoSivi/sim-verzuim-standaard)) en per koppelvlak een eigen repository met de releases. De bestanden zijn de officiële publicaties van sivi.org, op 5 oktober 2026 geïmporteerd.

Deze repository bevat alle releases van de Verzuimstandaard Werkgevers ↔ Arbodiensten. Vragen, wijzigingsverzoeken en discussies lopen via de [centrale ingang](https://github.com/DucoSivi/sim-verzuim-standaard).

## Releases

De 3 meest recente releases zijn actueel. Oudere releases blijven beschikbaar.

| Release | Status | Berichten | Wat is er veranderd? |
|---|---|---|---|
| [2026](https://github.com/DucoSivi/sim-verzuim-werkgevers-arbodiensten/releases/tag/2026) | **actueel** | 10 | [2025 → 2026](https://github.com/DucoSivi/sim-verzuim-werkgevers-arbodiensten/compare/2025...2026) |
| [2025](https://github.com/DucoSivi/sim-verzuim-werkgevers-arbodiensten/releases/tag/2025) | **actueel** | 10 | [2024 → 2025](https://github.com/DucoSivi/sim-verzuim-werkgevers-arbodiensten/compare/2024...2025) |
| [2024](https://github.com/DucoSivi/sim-verzuim-werkgevers-arbodiensten/releases/tag/2024) | **actueel** | 10 | [2022 → 2024](https://github.com/DucoSivi/sim-verzuim-werkgevers-arbodiensten/compare/2022...2024) |
| [2022](https://github.com/DucoSivi/sim-verzuim-werkgevers-arbodiensten/releases/tag/2022) | archief | 8 | eerste release in deze repository |

Bij elke release horen de officiële bestanden: de toelichting en de functionele beschrijvingen (PDF), de XML-schema's (XSD), waar van toepassing de verzuimcontrolecodes (XLS) en de zips.

## Twee releases vergelijken

Elke release heeft het jaartal als label. Daarmee kun je elke twee releases naast elkaar leggen, per bericht en per element:

- vorige naar huidige: [2025 → 2026](https://github.com/DucoSivi/sim-verzuim-werkgevers-arbodiensten/compare/2025...2026)
- alles sinds de oudste release: [2022 → 2026](https://github.com/DucoSivi/sim-verzuim-werkgevers-arbodiensten/compare/2022...2026)
- zelf kiezen: `https://github.com/DucoSivi/sim-verzuim-werkgevers-arbodiensten/compare/<oud>...<nieuw>`

## Wat staat waar

| Map | Inhoud |
|---|---|
| [`xsd/`](xsd) | De XML-schema's van de nieuwste release, één bestand per bericht, zonder jaartal in de naam |
| [`berichten/`](berichten) | Per bericht de berichtstructuur in Markdown, afgeleid van de XSD |
| [Releases](https://github.com/DucoSivi/sim-verzuim-werkgevers-arbodiensten/releases) | De officiële PDF-, XLS-, XSD- en ZIP-bestanden per jaar |

De documentatie om te lezen staat op het [portaal](https://ducosivi.github.io/sim-verzuim-standaard/werkgevers-arbodiensten/).

## Vragen of een wijziging voorstellen

- [Stel een vraag](https://github.com/DucoSivi/sim-verzuim-standaard/issues/new?template=vraag.yml)
- [Dien een wijzigingsverzoek in](https://github.com/DucoSivi/sim-verzuim-standaard/issues/new?template=wijzigingsverzoek.yml)
- [Discussies](https://github.com/DucoSivi/sim-verzuim-standaard/discussions)
