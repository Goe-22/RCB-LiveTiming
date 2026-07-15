# RCB LiveTiming – Datenfluss

**Version:** 1.0

**Stand:** 15.07.2026

---

# Ziel

Dieses Dokument beschreibt den vollständigen Datenfluss innerhalb von RCB LiveTiming.

Alle Module kommunizieren ausschließlich über den Core.

Dadurch bleiben die einzelnen Module unabhängig voneinander.

---

# Gesamtablauf

Decoder

↓

Decoder-Modul

↓

Zeitnahme (Core)

↓

Datenbank

↓

Benutzeroberfläche

↓

Homepage

↓

Sprachausgabe

---

# Decoder

Empfängt:

- Transpondernummer
- Zeitstempel

Gibt an den Core weiter:

- Transponder
- Uhrzeit

---

# Core

Berechnet:

- Rundenzeit
- Rundenzahl
- Schnellste Runde
- Letzte Runde
- Durchschnitt
- Persönliche Bestzeit
- Tagesbestzeit

Danach werden alle Daten gespeichert.

---

# Datenbank

Speichert:

- Fahrer
- Klassen
- Transponder
- Training
- Runden
- Einstellungen

Alle Änderungen werden sofort gespeichert.

---

# Benutzeroberfläche

Zeigt an:

- Fahrer
- Klasse
- Schnellste Runde
- Letzte Runde
- Durchschnitt
- Status

Die Anzeige aktualisiert sich automatisch.

---

# Homepage

Erhält ausschließlich fertige Daten.

Es erfolgen keine Berechnungen auf der Homepage.

---

# Sprachausgabe

Nach jeder gültigen Runde erhält die Sprachausgabe:

- Fahrername
- Klasse
- Rundenzeit
- Persönliche Bestzeit
- Tagesbestzeit

Anschließend erfolgt die Ansage.

---

# Fehlerbehandlung

Fällt ein Modul aus:

- Zeitnahme läuft weiter.
- Fehler werden protokolliert.
- Der Benutzer erhält eine Meldung.

Kein Fehler darf die Zeitnahme stoppen.

---

# Grundprinzip

Alle Module arbeiten unabhängig.

Die Zeitnahme besitzt immer höchste Priorität.
