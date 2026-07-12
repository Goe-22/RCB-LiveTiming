# RCB LiveTiming – Benutzeroberfläche Version 1.0

## 1. Ziel

Die Benutzeroberfläche ist für den täglichen Trainingsbetrieb ausgelegt.

Der Zeitnehmer soll nach dem Start des Programms möglichst keine weiteren Einstellungen vornehmen müssen.

Das Programm verbindet sich automatisch mit dem hinterlegten Decoder und überträgt die Daten live an die Homepage.

---

# 2. Hauptfenster

Das Hauptfenster ist die zentrale Anzeige während des Trainings.

## Kopfbereich

Anzeige:

- Projektname: RCB LiveTiming
- aktive Strecke
- Decoderstatus
- Homepagestatus

Beispiel:
RCB LiveTiming

Strecke: Onroad

Decoder:
🟢 Verbunden

Homepage:
🟢 Live aktiv
---

# 3. Live Fahrerübersicht

Die Haupttabelle zeigt alle aktuell aktiven Fahrer.

Spalten:

- Name
- Klasse
- Schnellste Runde
- Letzte Runde
- Durchschnitt
- Rundenzahl
- Status

Beispiel:

| Name | Klasse | Schnellste | Letzte | Durchschnitt | Runden | Status |
|---|---|---|---|---|---|---|
| Christian Göhler | TT-02 | 23.123 | 23.456 | 23.890 | 25 | 🟢 |
| Max Mustermann | FWD | 20.345 | 20.678 | 20.900 | 18 | 🟡 |

---

# 4. Fahrerdetails

Durch Anklicken des Namens öffnet sich die Detailansicht.

Anzeige:

- Name
- Klasse
- Transpondernummer
- Strecke
- Trainingszeit
- gefahrene Runden
- schnellste Runde
- Durchschnitt

Zusätzlich:

## Rundentabelle

| Runde | Zeit | Abstand |
|---|---|---|
| 1 | 24.102 | +0.979 |
| 2 | 23.456 | +0.333 |
| 3 | 23.123 | +0.000 |

---

# 5. Statusanzeige

Der Statusbereich zeigt:

## Strecke

Beispiel:

Strecke:
Onroad
oder
Strecke:
Offroad

---

## Decoder

Normalbetrieb:

