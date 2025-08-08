# 🎮 Arduino PONG – Modern Remake

Ein Remake des allerersten Videospiels – **PONG** – mit modernen Features wie **Power-Ups**, **Singleplayer- & Multiplayer-Modus** und einem selbst entworfenen **3D-gedruckten Gehäuse** im Nintendo-Switch-Stil.  
Entwickelt im Rahmen eines Computer-Architecture-Projekts.

---

## 📦 Features

- **Multiplayer** (1vs1) über zwei Joysticks
- **Singleplayer-Modus** mit zerstörbaren Farbfeldern
- **Vier Power-Ups**:
  - 🟥 **Ball** – Fügt einen zweiten Ball hinzu
  - 🟨 **Racket** – Vergrößert den eigenen Schläger und verkleinert den des Gegners
  - ⬜ **Mirror** – Spiegelt die Ballrichtung
  - 🟦 **Speed** – Erhöht die Ballgeschwindigkeit
- **3D-gedrucktes, tragbares Gehäuse** im Nintendo-Switch-Look
- **Einfache Stromversorgung** per USB (Laptop oder Powerbank)

---

## 🛠 Hardware-Komponenten

| Komponente                  | Menge |
|-----------------------------|-------|
| Arduino Uno                 | 1     |
| TFT 4-Zoll Bildschirm       | 1     |
| Joystick                    | 2     |
| USB A–B Kabel               | 1     |
| Jumperkabel (M/F)           | 12    |
| Steckverbinder (M/F)        | 24    |
| PLA-Filament für 3D-Druck   | 1     |

---

## 📚 Verwendete Libraries

Von der offiziellen Herstellerseite des TFT-Bildschirms:

- `DEV_Config.h`
- `LCD_Driver.h`
- `LCD_GUI.h`
- `fonts.h`

---

## 🎮 Bedienungsanleitung

1. **Gerät anschließen** (Laptop oder Powerbank).
2. **Startscreen** erscheint, gefolgt vom **Choice-Screen**.
3. **Modus wählen**:
   - **Multiplayer**: Linken Joystick nach oben bewegen.
   - **Singleplayer**: Rechten Joystick nach unten bewegen.
4. **Spielen!**:
   - Multiplayer: Ball zurückschlagen, bevor er die Wand hinter dir trifft.  
     Erster Spieler mit 10 Punkten gewinnt.
   - Singleplayer: Farbfelder abbauen, bis alle verschwunden sind.

---

## 🖥 Implementierung

- **GUI**: Direkte Ansteuerung des Displays über `LCD_Driver.h` für flüssige Bewegungen.
- **Grafik**: Minimalistisch im Retro-Stil des Original-PONG, aber mit farbigen Schlägern und Bällen.
- **Game-Logic**: Realistische Ballbewegung inkl. "Spin"-Effekt bei bewegtem Schläger.
- **Power-Ups**: Zufällige Erzeugung nach Ballkontakt mit Schläger, maximal 5 gleichzeitig auf dem Feld.
- **Singleplayer**: 2D-Array für Farbfelder, Farbwechsel in Stufen (rot → orange → gelb → grün → blau → gelöscht).

---

## 🖨 3D-Gehäuse

- **Design**: In *Fusion360* entworfen, inspiriert von Nintendo Switch.
- **Funktion**: Spieler sitzen sich gegenüber, minimiert gegenseitige Behinderung.
- **Bau**: 26 Stunden Druckzeit, inklusive Ständer und eigener Joystick-Sticks.
- **Optimierung**: Kabelmanagement durch Y-Splitter, um Platz zu sparen.

---


## 📝 Zusammenfassung

Dieses Projekt kombiniert Nostalgie mit moderner Hardware.  
Ein handgefertigtes, tragbares PONG-Spiel mit Multiplayer, Singleplayer und Power-Ups – betrieben auf einem Arduino Uno, angezeigt auf einem 4-Zoll-TFT, gesteuert mit zwei Joysticks, verpackt in einem maßgeschneiderten 3D-gedruckten Gehäuse.

---
