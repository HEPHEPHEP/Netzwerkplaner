# ⬡ Netzwerkplaner

Visueller Netzwerkplan-Editor im Browser — eine einzelne HTML-Datei, kein Backend, keine Abhängigkeiten.

![HTML](https://img.shields.io/badge/Single_File-HTML-orange)
![License](https://img.shields.io/badge/License-MIT-blue)

## Features

- **Knoten erstellen** — Firewall, Router, Switch, Internet, VLAN mit individuellen Icons und Farben
- **Verbindungen** — Geräte verbinden, Ports und Farben zuweisen, Routen über Zwischenknoten definieren
- **Geräte-Verwaltung** — VLANs mit Gerätelisten (Name, IP, MAC, Modell)
- **Drag & Drop** — Knoten und Port-Labels frei positionieren
- **Zoom & Pan** — Stufenloses Zoomen und Verschieben der Topologie
- **Tabellenansicht** — Übersicht aller Knoten und Verbindungen
- **Import / Export** — Netzwerkplan als JSON speichern und laden
- **Zero Dependencies** — Eine einzige HTML-Datei, läuft komplett im Browser

## Verwendung

`netzwerkplan.html` im Browser öffnen — fertig.

Oder online: direkt die Datei auf einem Webserver hosten.

## Kurzanleitung

| Aktion | Bedienung |
|---|---|
| Knoten hinzufügen | Toolbar-Buttons oben |
| Knoten bearbeiten | Klick auf Knoten |
| Knoten verschieben | Drag & Drop |
| Verbindung erstellen | `+ Verbindung` Button |
| Verbindung bearbeiten | Klick auf Linie |
| Wegpunkt setzen | Doppelklick auf Linie |
| Wegpunkt entfernen | Rechtsklick auf Wegpunkt |
| Port-Label verschieben | Drag auf den Punkt neben dem Label |
| Zoom | Mausrad oder Slider |
| Pan | Klick + Ziehen auf leere Fläche |

## Datenformat

Der Export erzeugt eine JSON-Datei mit folgendem Aufbau:

```json
{
  "version": 2,
  "nodes": [
    {
      "id": "n_1",
      "type": "firewall",
      "label": "Firewall",
      "icon": "⛊",
      "color": "#f5923a",
      "x": 500,
      "y": 300,
      "config": { "ip": "10.0.0.1", "model": "Sophos XGS", "port": "", "notes": "" }
    }
  ],
  "connections": [
    {
      "id": 1,
      "from": "n_1",
      "to": "n_2",
      "via": [{ "id": "n_3" }],
      "port": "443",
      "color": "#ff6b6b"
    }
  ]
}
```

## Lizenz

[MIT](LICENSE)
