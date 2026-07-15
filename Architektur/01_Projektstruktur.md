# RCB LiveTiming – Projektstruktur

**Version:** 1.0

**Stand:** 15.07.2026

---

# Ziel

RCB LiveTiming wird modular aufgebaut.

Jede Hauptfunktion arbeitet unabhängig von den anderen Modulen.

Dadurch können neue Funktionen oder Decoder später problemlos ergänzt werden.

---

# Projektübersicht

RCB LiveTiming besteht aus folgenden Modulen:

- Benutzeroberfläche
- Zeitnahme
- Decoder
- Fahrerverwaltung
- Datenbank
- Homepage
- Sprachausgabe
- Statistik
- Einstellungen

---

# Modul: Benutzeroberfläche

Aufgaben:

- Anzeige aller Fahrer
- Bedienung
- Rundentabelle
- Statusanzeigen

---

# Modul: Zeitnahme

Aufgaben:

- Runden berechnen
- Durchschnitt berechnen
- Persönliche Bestzeit
- Tagesbestzeit
- Trainingsverwaltung

---

# Modul: Decoder

Aufgaben:

- Verbindung herstellen
- Decoder überwachen
- Transponderdaten empfangen
- Fehler erkennen

Unterstützt:

- AMB RC3
- Vostok ID010

---

# Modul: Fahrerverwaltung

Aufgaben:

- Fahrer anlegen
- Fahrer bearbeiten
- Mehrere Transponder
- Klassenverwaltung

---

# Modul: Datenbank

Aufgaben:

- Fahrer speichern
- Trainings speichern
- Runden speichern
- Einstellungen speichern

Automatische Speicherung.

---

# Modul: Homepage

Aufgaben:

- Live-Daten übertragen
- Trainingsarchiv
- Rundentabellen
- Fahrerdetails

---

# Modul: Sprachausgabe

Aufgaben:

- Fahrername ansagen
- Rundenzeit ansagen
- Persönliche Bestzeit
- Tagesbestzeit

---

# Modul: Statistik

Aufgaben:

- Rekorde
- Durchschnitt
- Trainingshistorie
- Auswertungen

---

# Modul: Einstellungen

Aufgaben:

- Decoder
- Strecke
- Homepage
- Sprache
- Sicherung

---

# Kommunikation

Decoder

↓

Zeitnahme

↓

Datenbank

↓

Homepage

↓

Benutzeroberfläche

↓

Sprachausgabe

Alle Module arbeiten unabhängig voneinander.

Ein Fehler in einem Modul darf die Zeitnahme nicht unterbrechen.
