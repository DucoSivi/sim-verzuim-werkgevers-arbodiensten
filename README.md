# SIVI Verzuim: Werkgevers ↔ Arbodiensten

[![GitHub Pages](https://img.shields.io/badge/Docs-GitHub%20Pages-teal.svg)](https://ducosivi.github.io/sim-verzuim-werkgevers-arbodiensten/)
[![Licentie](https://img.shields.io/badge/Licentie-SIVI%20Open-yellow.svg)](https://www.sivi.org)

Specificatie en documentatie voor gegevensuitwisseling tussen Werkgevers (HR/Salarissystemen) en Arbodiensten.

---

## 📖 Documentatie

De complete functionele en technische documentatie is beschikbaar via GitHub Pages:  
👉 **[https://ducosivi.github.io/sim-verzuim-werkgevers-arbodiensten/](https://ducosivi.github.io/sim-verzuim-werkgevers-arbodiensten/)**

---

## 🔺 De SIVI Verzuim Driehoek (Model B)

Dit koppelvlak maakt deel uit van de gescheiden 3-trapsraket van SIVI Verzuim:

| Koppelvlak | Betrokken partijen | Repository & Docs |
|:---|:---|:---|
| **1** | Werkgevers ↔ Arbodiensten | [sim-verzuim-werkgevers-arbodiensten](https://ducosivi.github.io/sim-verzuim-werkgevers-arbodiensten/) |
| **2** | Werkgevers ↔ Verzekeraars | [sim-verzuim-werkgevers-verzekeraars](https://ducosivi.github.io/sim-verzuim-werkgevers-verzekeraars/) |
| **3** | Arbodiensten ↔ Verzekeraars | [sim-verzuim-arbodiensten-verzekeraars](https://ducosivi.github.io/sim-verzuim-arbodiensten-verzekeraars/) |

---

## 📁 Repository Structuur

```
├── .github/workflows/deploy.yml   # Automatische publicatie naar GitHub Pages
├── docs/                          # Bronbestanden van de MkDocs documentatie
│   ├── assets/sivi-logo.png       # SIVI beeldmerk
│   ├── stylesheets/sivi.css       # SIVI huisstijl
│   ├── index.md                   # Inleiding en doel
│   ├── processen.md               # Bedrijfsprocessen
│   ├── berichten.md               # Berichtspecificaties
│   ├── codelijsten.md             # SIVI Codelijsten
│   └── implementatie.md           # Implementatierichtlijnen
├── mkdocs.yml                     # Configuratie MkDocs Material
└── schema/                        # XSD definities en XML voorbeelden
    ├── Verzuimmeldingen2026.xsd
    ├── WerknemerDienstverband2026.xsd
    └── voorbeelden/
        ├── voorbeeld-ziekmelding.xml
        └── voorbeeld-dienstverband.xml
```

---

&copy; SIVI &mdash; Kennis- en standaardisatie-instituut voor de financiële dienstverlening
