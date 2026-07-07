# Glass Poker

Glass Poker ist eine minimalistische, einhändig bedienbare Web-App für Poker (Texas Hold'em) gegen KI-Gegner. Das gesamte Interface basiert auf einem modernen, hochauflösenden Liquid-Glass-Design (Glassmorphismus), welches durch semi-transparente Flächen, Unschärfe-Effekte und weiche Kanten eine saubere Tiefenwirkung erzeugt.

## Features

### Liquid Glass Interface
Das gesamte UI verzichtet auf klassische Neon-Effekte oder ablenkende Banner. Alle Menüs, Knöpfe, Overlays und die Navigation sind als funktionale Glaselemente mit Backdrop-Filter implementiert. Die Navigations-Icons sind einheitlich in weiß gehalten.

### Automatisiertes Gameplay
Der Spieler agiert immer als Erster (Pre-Flop, Flop, Turn, River). Nach der Aktion des Spielers führen alle aktiven KI-Bots ihre Züge vollautomatisch nacheinander mit einer kurzen zeitlichen Verzögerung aus. Nach Abschluss der Runde wird die nächste Phase geladen, ohne dass manuelle Zwischenschritte erforderlich sind.

### Swipe-to-Fold Gestensteuerung
Klassische Fold-Buttons wurden entfernt. Das Ablegen schlechter Blätter erfolgt über eine direkte Wischgeste. Die Karten werden per Touch oder Zeiger nach oben gezogen, fliegen visuell auf den Tisch und lösen die Fold-Aktion aus. Die Umsetzung basiert auf PointerEvents mit Pointer-Capture zur Verhinderung von Browser-Scrolling.

### Taktische HUD-Anzeige
Direkt neben den Hauptaktionen (Call und Raise) befindet sich eine permanente Informationsbox, welche die aktuelle statistische Gewinnwahrscheinlichkeit in Echtzeit für die jeweilige Spielphase ausgibt.

### Visuelles Regel-Overlay
Ein Klick auf die Gemeinschaftskarten (Community Board) öffnet ein bildschirmfüllendes Glass-Panel. Dieses enthält eine Übersicht aller Poker-Hand-Kombinationen, visualisiert durch miniaturisierte, gerenderte Spielkarten als direkte Beispielbilder.

### Vollwertiges Tisch-Setup & Bankroll-Tresor
Vor Spielbeginn ermöglicht ein Schieberegler die Anpassung der Stakes (Blinds) und des Buy-Ins. Über den Tresor-Bereich (Vault) steht ein simuliertes Auflade-System zur Verfügung, das den Erhalt neuer Test-Chips über eine bildschirmfüllende Lade- und Bestätigungsanimation abbildet.

## Technische Details

* Architektur: Single-Page-Application (SPA)
* Technologien: HTML5, CSS3 (Flexbox, CSS Grid, 3D-Transforms), JavaScript (Vanilla ES6)
* Eingabe-Handling: PointerEvents API zur präzisen Gesten-Erkennung auf mobilen Endgeräten und Desktop-Browsern
* Design-System: Reiner Glassmorphismus über fortgeschrittene CSS-Eigenschaften (backdrop-filter)

## Installation und Start

Da das Projekt ausschließlich aus Client-seitigem Code besteht, ist keine Installation oder Server-Umgebung notwendig.

1. Klone das Repository:
   git clone https://github.com/dein-benutzername/glass-poker.git

2. Navigiere in das Verzeichnis:
   cd glass-poker

3. Öffne die Datei index.html direkt in einem modernen Webbrowser deiner Wahl.

## Lizenz

Dieses Projekt ist unter der MIT-Lizenz lizenziert. Details dazu finden sich in der LICENSE-Datei.
