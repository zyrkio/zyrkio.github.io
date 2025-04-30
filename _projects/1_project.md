---
layout: page
title: "DeckDex – MTG-Kartenscanner"
description: "Ein innovatives IoT-System zur Erkennung, Organisation und Verwaltung von Magic: The Gathering-Karten"
img: assets/img/deckdex-hardware-cover.jpg
importance: 1
category: projects
related_publications: false
---

**DeckDex** ist ein interaktives System zur physischen Erkennung und Verwaltung von MTG-Karten. Es kombiniert optische Erkennung, motorisierte Steuerung und eine benutzerfreundliche Oberfläche für Sammler und Enthusiasten.

---

### 💡 Projektübersicht:

DeckDex nutzt ein Kamera-gestütztes Scansystem zur Kartenerkennung, gesteuert durch einen Raspberry Pi 5. Karten werden automatisch per Schrittmotor in eine definierte Position gefahren. Die Klassifikation und Verwaltung erfolgt über eine eigens programmierte App.

---

### 🛠️ Systemkomponenten:

| Komponente | Beschreibung |
|-----------|--------------|
| **Raspberry Pi 5** | Hauptsteuerungseinheit mit USB-Kamera und Datenverarbeitung |
| **Arduino** | Echtzeitsteuerung der Schrittmotoren via STEP/DIR |
| **TMC2209** | Leiser, präziser Schrittmotortreiber mit UART-Kommunikation |
| **NEMA17** | 2-Phasen-Schrittmotor zum Bewegen der Kartenplattform |
| **CAD-Designs** | Eigene 3D-gedruckte Komponenten für die Kartenführung |
| **OpenCV** | Bilderkennung zur Kartenerkennung (OCR / Template Matching) |
| **Datenbank** | Speicherung aller Karten & Metadaten lokal oder online |

---

### 🔍 Funktionale Features:

- **Automatische Kartenpositionierung** über Stepper + TMC2209 für präzise Bewegung der Kartenplattform.
- **Live-Bilderkennung** zur Erkennung von Kartennamen, Edition und Zustand mittels Kamera und OpenCV.
- **Datenbankintegration** zur strukturierten Speicherung und Verwaltung deiner Sammlung (lokal oder online).
- **Web-App & GUI** für:
  - Intuitive Steuerung und Visualisierung des Systems.
  - Preis-Tracking über externe APIs (Scryfall, TCGPlayer, Cardmarket).
  - Verwaltung von Duplikaten, Deckanalyse und Berechnung des Gesamtwerts.

---
### 🖼️ Systembilder:

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="assets/img/deckdex_Cad.jpeg" title="Hardware-Setup" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3">
    {% include figure.liquid path="assets/img/deckdex1.jpeg" title="CAD-Design der Plattform" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3">
    {% include figure.liquid path="assets/img/deckdex2.jpeg" title="Scan einer Karte" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Links: Das gesamte System im Betrieb.  
  Mitte: CAD-Ansicht der Kartenführung.  
  Rechts: Scan einer MTG-Karte mit Live-Erkennung.
</div>

---

---

### 🎨 UI mit Flutter & Dart

Die Benutzeroberfläche von **DeckDex** wird mit **Flutter** in der Programmiersprache **Dart** entwickelt. Diese Wahl ermöglicht eine moderne, responsive und plattformübergreifende Benutzererfahrung – ideal sowohl für Desktop als auch für mobile Geräte.

**Warum Flutter?**
- **Plattformunabhängigkeit**: Eine Codebasis für Web, Android, iOS und Desktop.
- **Hohe Performance**: Native Kompilierung sorgt für flüssige Animationen und schnelle Ladezeiten.
- **Flexible UI-Komponenten**: Ideal zur Darstellung dynamischer Kartendaten, Charts, Filter und Preisentwicklungen.
- **Einfaches State Management**: Sauberer Code für komplexe Interaktionen wie Live-Suche, Preisabfragen und Filterlogik.
- **Entwicklung unter Ubuntu**: Flutter funktioniert hervorragend unter Ubuntu, was schnelles Prototyping und reibungslose Entwicklung auf deinem System ermöglicht.

