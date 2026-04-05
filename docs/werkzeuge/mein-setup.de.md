# Mein Setup

*Hardware, Software, und wie alles zusammenspielt.*

## Die Geräte

**CPAP**: Löwenstein prismaSMART max (seit Jan 2025). APAP-Modus, Druckbereich 10–14 cmH₂O. Daten auf SD-Karte, täglich ausgelesen.

**Pulsoximeter**: Wellue O2Ring. Misst SpO₂ und Herzfrequenz über die ganze Nacht, sekündlich. Datenübertragung per Bluetooth (BLE) auf einen Raspberry Pi.

**Schlafphasen**: Apple Watch. Liefert Deep/Core/REM/Awake-Klassifikation über Apple Health.

**Video**: REOLINK-Kamera. Infrarot-Nachtsicht, RTSP-Stream, aufgezeichnet per ffmpeg auf dem Raspberry Pi.

**Raspberry Pi**: Das Herzstück der Nachtüberwachung. Läuft unbeaufsichtigt, startet abends automatisch, nimmt BLE-Daten vom O2Ring und Video von der Kamera auf.

## Die Software

**OSCAR**: Open Source CPAP Analysis Reporter. War mein Einstieg in die CPAP-Datenanalyse. Zeigt Druck, Flow, Events, Leckage — alles, was auf der SD-Karte liegt.

**SDA5 (System-5)**: Mein eigenes Analysesystem. Python, PostgreSQL, über 1.500 Commits. Verarbeitet CPAP-, O2Ring-, Apple-Health- und Videodaten in einer automatisierten 12-Schritt-Morgenroutine. Erzeugt HTML-Nachtberichte mit Narrativ, Korrelationen und Einordnung.

Vier Systemgenerationen sind diesem vorausgegangen (S1–S4), jeweils komplett neu gebaut. Die ersten zwei mit ChatGPT, die letzten zwei mit Claude.

## Der tägliche Ablauf

Morgens: SD-Karte aus dem CPAP, Morgenroutine starten, 3–5 Minuten warten. Danach liegt ein vollständiger Nachtbericht vor — mit AHI, SpO₂-Statistiken, Schlafphasen, Atemfrequenz, und einer narrativen Einordnung.

Die Daten landen in einer PostgreSQL-Datenbank. Aktuell: über 619 Nächte, 21 Monate, lückenlos.

---

*Zurück: [Werkzeuge](index.md)*
