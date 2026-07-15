# RCB LiveTiming – Datenbank

**Version:** 1.0

**Stand:** 15.07.2026

---

# Ziel

Die Datenbank speichert alle Informationen dauerhaft.

Alle Änderungen werden sofort gespeichert.

Es gibt keinen manuellen Speichervorgang.

---

# Datenbanktyp

Version 1.0 verwendet SQLite.

Vorteile:

- Keine Installation notwendig
- Eine einzige Datenbankdatei
- Sehr schnell
- Perfekt für einen einzelnen Windows-PC
- Einfache Datensicherung

---

# Tabellen

## Fahrer

Speichert alle Fahrer.

Felder:

- Fahrer-ID
- Name
- Erstellt am
- Geändert am

---

## Transponder

Speichert alle Transponder.

Felder:

- Transponder-ID
- Fahrer-ID
- Transpondernummer
- Klasse
- Aktiv

Ein Fahrer kann beliebig viele Transponder besitzen.

---

## Klassen

Speichert alle Klassen.

Felder:

- Klassen-ID
- Name

Beispiele:

TT-02

FWD

Fun

GT

M-Chassis

---

## Training

Speichert jede Trainingseinheit.

Felder:

- Trainings-ID
- Datum
- Startzeit
- Endzeit
- Strecke
- Decoder
- Bemerkung

---

## Runden

Speichert jede einzelne Runde.

Felder:

- Runden-ID
- Trainings-ID
- Fahrer-ID
- Transpondernummer
- Rundennummer
- Zeitstempel
- Rundenzeit
- Persönliche Bestzeit
- Tagesbestzeit

---

## Einstellungen

Speichert alle Programmeinstellungen.

Beispiele:

- Decoder
- IP-Adresse
- Port
- Strecke
- Homepage
- Sprachausgabe
- Lautstärke

---

# Beziehungen

Ein Fahrer

↓

Mehrere Transponder

↓

Mehrere Trainings

↓

Viele Runden

---

# Automatische Speicherung

Alle Änderungen werden unmittelbar gespeichert.

Nach einem Programmabsturz gehen höchstens die Daten der aktuell verarbeiteten Runde verloren.

---

# Datensicherung

Beim Beenden des Programms wird automatisch eine Sicherung erstellt.

Zusätzlich kann jederzeit manuell eine Sicherung erstellt werden.

---

# Wiederherstellung

Eine Sicherungsdatei kann jederzeit wieder eingespielt werden.

Dabei bleiben alle Trainings erhalten.

---

# Erweiterbarkeit

Die Datenbank ist so aufgebaut, dass später weitere Funktionen ergänzt werden können.

Beispiele:

- Rennen
- Meisterschaften
- Teamrennen
- Rekorde
- Stream-Daten