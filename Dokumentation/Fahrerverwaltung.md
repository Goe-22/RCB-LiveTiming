# RCB LiveTiming – Fahrerverwaltung

## 1. Ziel

Die Fahrerverwaltung dient zur dauerhaften Speicherung aller Fahrer, Transponder und Klassen.

Ein Fahrer kann mehrere Fahrzeuge besitzen und somit mehrere Transponder und Klassen verwenden.

Die Daten bleiben dauerhaft gespeichert und stehen bei jedem Programmstart automatisch zur Verfügung.

---

# 2. Fahrer

Für jeden Fahrer werden folgende Daten gespeichert:

- Name
- Aktiv / Inaktiv
- Bemerkungen (optional)

Beispiel:

Name:
Christian Göhler

---

# 3. Transponder

Ein Fahrer kann beliebig viele Transponder besitzen.

Für jeden Transponder werden gespeichert:

- Transpondernummer
- Klasse
- Aktiv / Inaktiv

Beispiel:

Christian Göhler

| Transponder | Klasse |
|--------------|---------|
| 123456 | TT-02 |
| 654321 | Fun |

---

# 4. Automatische Erkennung

Wird ein bekannter Transponder erkannt, ordnet das Programm ihn automatisch dem Fahrer und der Klasse zu.

Beispiel:

Transponder 123456

↓

Christian Göhler

↓

TT-02

---

# 5. Unbekannte Transponder

Wird ein unbekannter Transponder erkannt, erscheint eine Meldung:

"Unbekannter Transponder erkannt."

Der Zeitnehmer kann:

- einem vorhandenen Fahrer zuordnen
- neuen Fahrer anlegen
- Vorgang abbrechen

---

# 6. Fahrer bearbeiten

Folgende Änderungen sind jederzeit möglich:

- Name ändern
- Transponder hinzufügen
- Transponder löschen
- Klasse ändern
- Fahrer deaktivieren
- Fahrer löschen

---

# 7. Suche

Die Suche erfolgt nach:

- Name
- Transpondernummer
- Klasse

---

# 8. Trainingsbetrieb

Während des Trainings werden angezeigt:

- Name
- Klasse
- Schnellste Runde
- Letzte Runde
- Durchschnitt
- Rundenzahl

Ein Fahrer kann mit verschiedenen Fahrzeugen trainieren.

Beispiel:

Christian Göhler – TT-02

Christian Göhler – Fun

Beide Einträge werden getrennt ausgewertet.

---

# 9. Datensicherheit

Alle Änderungen werden automatisch gespeichert.

Beim nächsten Programmstart stehen alle Daten wieder zur Verfügung.

---

# 10. Erweiterungen

Für zukünftige Versionen sind folgende Funktionen vorgesehen:

- Vereinszugehörigkeit
- Lizenznummer
- Persönliche Streckenrekorde
- Trainingshistorie
- Export und Import
