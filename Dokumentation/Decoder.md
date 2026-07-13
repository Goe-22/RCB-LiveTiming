# RCB LiveTiming – Decoder

## 1. Ziel

RCB LiveTiming soll mit verschiedenen Zeitmess-Decodern arbeiten können.

Die eigentliche Zeitnahme darf dabei unabhängig vom Decoder funktionieren.

Der Decoder liefert lediglich die Durchfahrten.

Alle weiteren Berechnungen übernimmt RCB LiveTiming.

---

# 2. Unterstützte Decoder

Version 1.0

- AMB RC3 (Firmware 4.4)
- Vostok Electronics ID010 (AMB-kompatible Ausgabe)

Weitere Decoder sollen später ergänzt werden können.

---

# 3. Verbindung

Die Verbindung erfolgt über das Netzwerk.

Einstellbar:

- Decoder-Typ
- IP-Adresse
- Port

Die Einstellungen werden dauerhaft gespeichert.

Beim Programmstart verbindet sich RCB LiveTiming automatisch.

---

# 4. Verbindung überwachen

Während des Betriebs wird die Verbindung permanent überwacht.

Status:

🟢 Verbunden

🔴 Nicht verbunden

Bei einer Unterbrechung versucht das Programm automatisch die Verbindung wiederherzustellen.

Währenddessen bleibt die Benutzeroberfläche bedienbar.

---

# 5. Empfangene Daten

Der Decoder liefert mindestens:

- Transpondernummer
- Zeitpunkt der Durchfahrt

Aus diesen Daten berechnet RCB LiveTiming:

- Rundenzeit
- Letzte Runde
- Schnellste Runde
- Durchschnitt
- Rundenzahl

---

# 6. Mehrere Decoder

Jede Installation arbeitet mit genau einem Decoder.

Beispiele:

Laptop 1

- Strecke: Onroad
- Decoder: AMB RC3

Laptop 2

- Strecke: Offroad
- Decoder: Vostok ID010

Die Streckenzuordnung erfolgt einmalig in den Einstellungen.

---

# 7. Fehlerbehandlung

Mögliche Fehler:

- Decoder nicht erreichbar
- Netzwerkverbindung unterbrochen
- Ungültige Daten
- Zeitüberschreitung

Das Programm informiert den Benutzer über den Fehler.

Die Zeitnahme wird dabei nicht beendet.

---

# 8. Erweiterbarkeit

Neue Decoder sollen später ohne Änderungen an der Zeitnahme eingebunden werden können.

Die Decoder-Schnittstelle wird deshalb modular aufgebaut.

Alle Decoder liefern intern dieselben Informationen:

- Transpondernummer
- Zeitpunkt der Durchfahrt

Der Rest der Verarbeitung erfolgt ausschließlich im Zeitnahme-Modul.
