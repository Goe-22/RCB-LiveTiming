# RCB LiveTiming – Decoder

**Version:** 1.0

**Stand:** 15.07.2026

---

# Ziel

Das Decoder-Modul ist für die Kommunikation mit der Zeitmessanlage verantwortlich.

Es empfängt ausschließlich die Daten des Decoders.

Alle weiteren Berechnungen übernimmt RCB LiveTiming.

---

# Unterstützte Decoder

Version 1.0

- AMB RC3 (Firmware 4.4)
- Vostok Electronics ID010 (AMB-kompatible Ausgabe)
- RCM Decoder Simulator

Weitere Decoder können später ergänzt werden.

---

# Verbindung

Die Verbindung erfolgt über das Netzwerk.

Einstellungen:

- Decoder-Typ
- IP-Adresse
- Port

Die Verbindung wird beim Programmstart automatisch hergestellt.

---

# Verbindung überwachen

Das Programm überwacht permanent:

- Netzwerkverbindung
- Decoder erreichbar
- Datenempfang

Statusanzeigen:

🟢 Verbunden

🟡 Verbinde...

🔴 Nicht verbunden

---

# Automatische Wiederverbindung

Bei einer Unterbrechung versucht das Programm automatisch erneut eine Verbindung aufzubauen.

Dabei läuft die Benutzeroberfläche weiter.

Der Benutzer muss nichts bestätigen.

---

# Empfangene Daten

Der Decoder liefert:

- Transpondernummer
- Zeitpunkt der Durchfahrt

Diese Daten werden sofort an den Core weitergegeben.

---

# Datenprüfung

Jeder Datensatz wird geprüft.

Geprüft werden:

- gültige Transpondernummer
- gültiger Zeitstempel
- doppelte Durchfahrten
- Mindest-Rundenzeit

Ungültige Daten werden protokolliert.

---

# Mehrere Decoder

Jede Installation arbeitet mit genau einem Decoder.

Beispiele:

Laptop Onroad

→ AMB RC3

Laptop Offroad

→ Vostok ID010

Die Auswahl erfolgt einmalig in den Einstellungen.

---

# Fehlerbehandlung

Mögliche Fehler:

- Netzwerk getrennt
- Decoder nicht erreichbar
- Zeitüberschreitung
- Ungültige Daten
- Verbindungsabbruch

Alle Fehler werden protokolliert.

Die Zeitnahme bleibt weiterhin bedienbar.

---

# Simulator

Für Entwicklung und Tests kann der RCM Decoder Simulator verwendet werden.

Der Simulator wird vom Programm wie ein echter Decoder behandelt.

---

# Erweiterbarkeit

Neue Decoder werden über eine einheitliche Schnittstelle eingebunden.

Dadurch muss die eigentliche Zeitnahme später nicht geändert werden.

---

# Grundprinzip

Der Decoder liefert ausschließlich Messdaten.

Alle Berechnungen erfolgen im Core.

Dadurch bleibt das Programm unabhängig vom verwendeten Decoder.