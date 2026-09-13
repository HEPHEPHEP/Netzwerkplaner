# Netzwerkplaner

Visueller Netzwerk-Topologie-Editor im Browser. Eine einzelne HTML-Datei, keine Build-Tools, keine Abhängigkeiten.

![HTML](https://img.shields.io/badge/Single_File-HTML-orange)
![License](https://img.shields.io/badge/License-MIT-blue)

## Funktionen

- **Einzelne HTML-Datei** — kein Build-Prozess, kein Backend, läuft komplett im Browser
- **Dunkles und helles Theme** — je Ansicht umschaltbar; im hellen Modus werden Farben automatisch kontrastverstärkt
- **Knotentypen** — Firewall, Router, Switch, Internet, VLAN mit individuellen Icons und Farben
- **Freie Geräte-Knoten** — z. B. Server als eigenständige Kacheln ausserhalb von VLANs
- **VLAN-Geräteverwaltung** — Geräte wie PCs, Drucker etc. innerhalb von VLANs verwalten (Name, IP, MAC, Modell)
- **Drag & Drop** — Knoten frei auf der Zeichenfläche positionieren
- **Toolpalette für Formen** — Rechteck, Kreis, Dreieck, Raute, Sechseck, Linie, Pfeil, Doppelpfeil und Text frei im Plan platzieren (Farbe, Füllung, Linienstärke, Drehung, Ebene)
- **Markieren & Verknüpfen** — Kacheln und Formen per Shift+Klick oder Auswahlrahmen markieren und verknüpfen; verknüpfte Objekte werden gemeinsam verschoben
- **Undo/Redo** — alle Änderungen am Plan schrittweise zurücknehmen und wiederholen (Strg+Z / Strg+Y)
- **Verbindungsrouting** — Verbindungen über Zwischenknoten (Wegpunkte) führen
- **Parallele Verbindungen** — mehrere Verbindungen zwischen gleichen Knoten mit senkrechtem Versatz
- **Verbindungs-Highlighting** — Verbindungen hervorheben und Port-Labels direkt inline bearbeiten
- **Animierte Verbindungen** — leuchtende Punkte laufen von der Quelle zum Ziel oder Strichmuster wandern die Linie entlang; pro Verbindung wählbar, ebenso für gestrichelte Formen, global abschaltbar
- **Skizzenmodus** — vereinfachte Ansicht für Präsentationsgrafiken: Symbole und Bezeichnungen statt IP-Adressen, farbige Bereiche mit Titelbalken; jederzeit zwischen Detail und Skizze umschaltbar, die technischen Daten bleiben erhalten
- **Symbolbibliothek mit Suche** — über 40 Strichsymbole, z. B. PC, Server, NAS, Switch, Router, Firewall, Konnektor, VPN und Medizingeräte
- **Eigene Symbole** — Bilder (PNG, JPG, SVG, WebP) hochladen; sie werden verkleinert im Browser gespeichert und beim JSON-Export mitgegeben
- **Rechtwinklige Verbindungen mit Sammellinien** — mehrere Verbindungen laufen auf einer gemeinsamen Linie zusammen; Pfeile, Linienstärke und Strichart pro Verbindung
- **Hilfslinien** — Kacheln rasten beim Verschieben an Mitte und Höhe anderer Objekte ein
- **Bereiche aufräumen** — Kacheln im Raster anordnen und wahlweise den Rahmen an die Kacheln oder die Kacheln an den Rahmen anpassen
- **Kachelgröße** — 50–200 % für markierte oder alle Kacheln, zusätzlich pro Kachel einstellbar
- **Freihand und Radiergummi** — mit wählbarer Farbe und Stärke zeichnen; die mittlere Maustaste verschiebt dabei die Zeichenfläche
- **Portbeschriftungen ein- und ausblendbar** — getrennt für Detail- und Skizzenansicht
- **PNG-Export** — Plan als Bild speichern (lädt dafür bei Bedarf html2canvas nach)
- **Zoom & Pan** — stufenloses Zoomen und Verschieben der Zeichenfläche
- **Tabellenübersicht** — alle Knoten und Verbindungen in Tabellenform
- **JSON Import/Export** — Netzwerkplan als JSON-Datei speichern und laden
- **Auto-Speichern lokal** — Fortschritt wird im Browser gespeichert und nach Neuladen wiederhergestellt
- **Oberfläche auf Deutsch**

## Nutzung

Die Datei `netzwerkplan.html` in einem beliebigen Browser öffnen — fertig. Es ist keine Installation oder Konfiguration nötig.

## Lizenz

Dieses Projekt steht unter der [MIT-Lizenz](LICENSE).
