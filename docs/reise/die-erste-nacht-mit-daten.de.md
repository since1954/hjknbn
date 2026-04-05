# Die erste Nacht mit Daten

*14. Juli 2024. Ein Pulsoximeter, ein CPAP-Gerät, und der Anfang von etwas, das ich nicht hatte kommen sehen.*

## Das Setup

Das CPAP-Gerät lief schon seit Jahren: eine Löwenstein Prisma Smart, Modus APAP, Druckbereich 7–12 cmH₂O. Was fehlte, war die unabhängige Messung der Sauerstoffsättigung — denn das Gerät selbst misst kein SpO₂.

Ich kaufte einen Wellue O2Ring. Ein kleiner Ring, der am Finger die Sauerstoffsättigung und Herzfrequenz über die gesamte Nacht aufzeichnet. Dazu: OSCAR, die Open-Source-Software, um die CPAP-Daten von der SD-Karte auszulesen.

Am 14. Juli 2024 zeichnete ich zum ersten Mal beides gleichzeitig auf. Nacht 1 in der Datenbank.

## Was die Daten zeigten

Der AHI im Juli 2024 lag bei durchschnittlich 4,29. Nicht schlecht. Aber der O2Ring erzählte eine andere Geschichte: Der ODI (Oxygen Desaturation Index) lag bei rund 21 — also 21 Sauerstoffeinbrüche pro Stunde, deutlich mehr als die Apnoe-Events, die das CPAP-Gerät zählte.

Die CPAP-Maschine sagte: "Alles im Griff." Der O2Ring sagte: "Da passiert noch etwas, das das Gerät nicht sieht."

## Die Config-Odyssee

Was folgte, waren vier Monate des Ausprobierens. Sechs verschiedene Druckkonfigurationen zwischen Juli und Oktober 2024 — von APAP über einen Festdruck-Versuch (der nach einer Nacht abgebrochen wurde und den AHI auf 327 trieb) bis zur ersten stabilen Einstellung.

Im September 2024 erreichte der Monats-AHI 15,58 — ein Wert, der ohne eigene Datenerhebung unsichtbar geblieben wäre. Er wäre im Jahresdurchschnitt des nächsten Arztbesuchs untergegangen.

Ab Oktober stabilisierte sich der AHI um 4. Aber der ODI blieb bei 21, egal welche Config. Das war die erste echte Erkenntnis: Der CPAP-Druck kontrolliert die Apnoen, aber die Sauerstoffeinbrüche haben offenbar eine eigene Dynamik.

## Was ich damals noch nicht wusste

Dass aus dieser Tabellenkalkulation ein eigenes Analysesystem werden würde. Dass ich innerhalb von 18 Monaten vier Generationen Software bauen würde, zusammen mit einer KI. Dass ich eines Tages die Atemfrequenz direkt aus den CPAP-Rohdaten berechnen, Schlafvideos mit Physiologie-Daten synchronisieren, und ein geschlossenes Sauerstoff-Supplementierungssystem simulieren würde.

Am 14. Juli 2024 wusste ich nur: Mein CPAP-Gerät erzählt mir nicht die ganze Geschichte. Und ich wollte den Rest hören.

---

*Weiter: [Der Gerätewechsel](der-geraetewechsel.md)*
