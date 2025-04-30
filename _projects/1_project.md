---
layout: page
title: "DeckDex – MTG Card Scanner"
description: "An innovative IoT system for identifying, organizing, and managing Magic: The Gathering cards"
img: assets/img/deckdex_Cad.jpeg
importance: 1
category: fun
related_publications: false
---

**DeckDex** is an interactive system for the physical recognition and management of Magic: The Gathering (MTG) cards. It combines optical recognition, motorized movement, and a user-friendly interface for collectors and enthusiasts.

- GitHub Repository: [zyrkio/deckdex_app](https://github.com/zyrkio/deckdex_app)

---

### 💡 Project Overview

DeckDex uses a camera-based scanning system for card detection, controlled by a Raspberry Pi 5. Cards are automatically moved into a defined position via stepper motor mechanics. Classification and management are handled through a custom-built app.

---

### 🛠️ System Components

| Component         | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| **Raspberry Pi 5** | Main control unit with USB camera and local data processing                |
| **Arduino**        | Real-time motor control using STEP/DIR signals                             |
| **TMC2209**        | Silent and precise stepper driver with UART configuration                  |
| **NEMA17**         | Bipolar stepper motor for card platform movement                           |
| **CAD Designs**    | Custom 3D-printed parts for guiding and holding cards                      |
| **OpenCV**         | Optical recognition for card details (OCR / template matching)             |
| **Database**       | Stores card metadata and collection data locally or optionally online      |

---

### 🔍 Key Features

- **Automatic Card Positioning**  
  With stepper motors and TMC2209 drivers for precise and reliable movement.

- **Live Card Recognition**  
  Detects card name, edition, and condition using real-time camera input and OpenCV.

- **Database Integration**  
  Structure and manage your card collection offline or optionally sync with cloud storage.

- **Web App & GUI**  
  - Intuitive control of the scanning process and visualization  
  - Price tracking via external APIs (Scryfall, TCGPlayer, Cardmarket)  
  - Tools for duplicate handling, deck analysis, and collection value computation

---

### 🖼️ System Images

<div class="row">
  <div class="col-sm mt-3">
    {% include figure.liquid path="assets/img/deckdex_Cad.jpeg" title="Hardware Setup" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3">
    {% include figure.liquid path="assets/img/deckdex1.jpeg" title="CAD Design of Platform" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3">
    {% include figure.liquid path="assets/img/deckdex2.jpeg" title="Scanning a Card" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Left: Full hardware system in operation.  
  Center: CAD view of the card-guiding platform.  
  Right: Live scan of an MTG card.
</div>

---

### 🎨 UI Built with Flutter & Dart

The user interface for **DeckDex** is developed using **Flutter** and **Dart**, enabling a modern, responsive, and cross-platform experience suitable for both desktop and mobile devices.

**Why Flutter?**
- **Cross-platform**: One codebase for Web, Android, iOS, and Desktop
- **High Performance**: Native compilation ensures smooth animations and fast rendering
- **Flexible UI Widgets**: Perfect for showing dynamic card data, charts, filters, and prices
- **Clean State Management**: Structured and maintainable code for real-time updates and interactions
- **Optimized for Ubuntu**: Flutter runs seamlessly under Ubuntu for fast prototyping and deployment

