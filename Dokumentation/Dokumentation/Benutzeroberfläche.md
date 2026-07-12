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

Decoder verbunden

Fehler:

Decoder nicht erreichbar

 ---

## Homepage

Normalbetrieb:

Live Übertragung aktiv

Fehler:

Keine Verbindung zur Homepage

---

# 6. Menüstruktur

## Datei

- Neues Training starten
- Training speichern
- Training beenden
- Programm beenden

---

## Fahrer

- Fahrer verwalten
- Transponder verwalten
- Klassen verwalten

---

## Einstellungen

- Decoder Einstellungen
- Streckeneinstellungen
- Homepage Einstellungen
- Sprachausgabe
- Anzeige

---

## Hilfe

- Informationen zum Programm
- Versionsnummer

---

# 7. Zweite Anzeige (optional)

Für einen zusätzlichen Monitor kann eine vereinfachte Anzeige verwendet werden.

Beispiel:

RCB LiveTiming

Christian Göhler

Klasse:
TT-02

Letzte Runde:

23.123 Sekunden

Beste Runde:

22.987 Sekunden

---

# 8. Bedienphilosophie

Das Programm ist speziell für den Trainingsbetrieb entwickelt.

Ablauf:

1. Laptop starten
2. RCB LiveTiming starten
3. Decoder verbindet automatisch
4. Fahrer fahren auf die Strecke
5. Runden werden automatisch erkannt
6. Rundenzeiten werden angesagt
7. Live-Daten werden auf die Homepage übertragen

Während des Trainings sind keine zusätzlichen Eingaben notwendig.
