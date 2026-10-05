# Prompt: „Smartys Kaffeepanne“ – 3D-Recruiting-Spiel der SmartFactory KL

> **Anhänge zum Prompt:** SmartFactory-KL-Logo (PNG) und Bewerbungs-QR-Code (PNG).

---

Erstelle ein browserbasiertes 3D-Lernspiel als **eine einzige, eigenständige HTML-Datei** (HTML, CSS und JavaScript inline, three.js r128 von cdnjs). Sprache durchgehend **Deutsch**. Logo und QR-Code werden als Base64 direkt in die Datei eingebettet. Das Spiel soll junge Menschen spielerisch für technische Berufe begeistern und endet mit einem Bewerbungsaufruf.

## Story und Ablauf

- **Schauplatz:** Eine moderne Modellfabrik-Halle mit Produktionslinie, Regalen, Signalsäulen und einer vernetzten Kaffeemaschine an „Modul 07“.
- **Auslöser:** Der mobile Transportroboter **Smarty** nimmt die Kurve zu eng, rammt die Kaffeemaschine und löst eine Störung aus („Oh nein! Das war ich!“).
- **Personalauswahl:** Die spielende Person liest die Störmeldung und wählt aus, wer helfen soll: eine oder mehrere von drei Fachkräften. Wer umsonst kommt oder fehlt, kostet 25 Punkte.
- **Reparatur:** Die gewählten Personen laufen zur Maschine und lösen die Aufgabe interaktiv per Klick/Tipp in der 3D-Szene.
- **Probelauf:** Die Maschine brüht einen Espresso, alle jubeln, und Smarty bedankt sich.

## Die vier Level

Anzeige oben als **„Level 1/4“ bis „Level 4/4“**. Level 1–3 sind die drei Einzelaufgaben in zufälliger Reihenfolge, Level 4 ist immer der Team-Einsatz.

### Die drei Fachkräfte

| Person | Beruf | Aussehen und Ausrüstung |
|---|---|---|
| **Tanja** (weiblich) | Technikerin | Pferdeschwanz, dunkelblaue Arbeitskleidung mit Warnstreifen, Werkzeuggürtel, Schraubendreher in der Hand |
| **Sam** (divers) | Programmierer*in / Softwareentwickler*in | Bob-Frisur, Headset, hält ein Tablet |
| **Jonas** (männlich) | Maschinenbauingenieur | Brille, hellblaues Kurzarmhemd, Kragen, Lanyard mit Ausweis |

### Aufgabe 1 – Elektrik (Tanja)

1. Tanja öffnet die linke Wartungsklappe mit der Hand am Griff.
2. Die Spielenden ordnen drei lose Adern den Klemmen zu: braun = L, blau = N, grün-gelb = PE (IEC 60445).
3. Tanja greift jeweils das Aderende, führt es zur Klemme und dreht die Schraube mit dem Schraubendreher fest.
4. Danach legt sie den Hauptschalter um.

### Aufgabe 2 – Software (Sam)

1. Ein Hologramm-Panel „PROGRAM Brühablauf“ erscheint.
2. Fünf Funktionsbausteine kommen in die richtige Reihenfolge: Mahlen(18 g), Tampern(15 kg), Vorbrühen(3 s), Extrahieren(9 bar), Ausgeben(). Sam greift jeden Baustein mit der Hand und trägt ihn zum Slot.
3. Danach wird der Brüh-Sollwert gewählt: 93 °C ist richtig, 75 und 110 °C sind falsch und werden kurz erklärt.
4. Abschließend wird die Firmware geflasht (Fortschrittsbalken im Display).

### Aufgabe 3 – Getriebe (Jonas)

1. Jonas öffnet die rechte Klappe und sieht ein Stirnradgetriebe (Modul m = 1 mm). Motorrad z₁ = 16 und Mahlwerk z₂ = 24 sind gegeben, das Zwischenrad fehlt. Der Achsabstand wird mit Maßlinie angezeigt.
2. Ein Ersatzteillager bietet drei Zwischenräder (z = 12/18/24), die Beschriftung steht groß direkt auf dem Zahnrad.
3. Jonas läuft auf einem Weg außen am Lager entlang und nie durch die Zahnräder hindurch. Er nimmt das gewählte Rad in die Hand und setzt es ein. Ein falsches Rad passt nicht (zu klein / zu groß) und wird zurückgebracht.
4. Danach folgt die Frage nach der Mahlwerk-Drehzahl (n₂ = n₁ · z₁/z₂; das Zwischenrad ändert nur die Drehrichtung).
5. Nach der richtigen Lösung verschwinden die übrigen Zahnräder und alle Zahlen und Beschriftungen.

### Level 4 – Team-Einsatz

Alle drei arbeiten nacheinander:

1. Tanja schließt die Adern an.
2. Jonas setzt das Zwischenrad ein.
3. Sam trägt den neuen Drehzahl-Sollwert ein, dabei hilft Jonas mit einem Hinweis.
4. Tanja schaltet den Strom wieder ein („Jonas, bist du fertig? Dann schalte ich den Strom wieder ein.“).

## Bewertung und Ergebnis

- **Punkte:** Start mit 100 Punkten je Level, Abzüge für Fehler (−10), Hinweise (−5) und Fehlbesetzungen (−25), dazu ein Zeitbonus. Pro Level werden 1–3 Sterne vergeben.
- **Ergebnisseite:** Punkte, Zeit, Fehlbesetzungen und Fehlgriffe.
- **Automatischer Ablauf:** Nach jedem Level startet das nächste nach **3 Sekunden** Countdown auf dem Knopf, ein Klick davor ist möglich. Ab Level 2 fährt Smarty nach 3 Sekunden von selbst los. Nur Level 1 braucht einen Klick, weil Browser Ton erst nach einer Nutzeraktion erlauben.
- **Spielende:** Nach Level 4, wenn alle fertig gejubelt haben, wird groß **„Bewirb dich jetzt!“** mit dem **QR-Code** darunter eingeblendet. Darunter steht ein Knopf „Zum Ergebnis“. Die Ergebnisseite zeigt die Gesamtpunkte und „Nochmal spielen“ (startet wieder bei Level 1). Nach Level 4 gibt es keinen automatischen Neustart, damit der QR-Code in Ruhe gescannt werden kann.

## Branding

- **SmartFactory-KL-Logo** an diesen Stellen:
  - oben links neben dem Titel „Smartys Kaffeepanne“
  - groß als Schild an der Hallenwand
  - am Tisch der Kaffeemaschine
  - auf Smartys Oberkörper, zusätzlich mit dem Namensschild „SMARTY“
- **Farben:** dunkles Industrie-Design mit Akzent Orange (#FFB547) und Türkis (#45D3CB). Das Bewerbungs-Overlay ist weiß mit SmartFactory-Blau (#004f9f).

## Figuren und Animation

- **Personen:** realistischere Proportionen mit Torso aus Lathe-Geometrie, Hüfte, Oberschenkel/Unterschenkel mit Knie, Ober-/Unterarm mit Ellbogen und Händen mit Daumen. Das Gesicht hat Augäpfel mit Iris und Blinzeln, Augenbrauen, Nase, Ohren und Mund. Die Haut wirkt mit leichtem Eigenleuchten weicher.
- **Gang:** natürlich, mit Kniebeugung und Armschwung.
- **Greifen:** Two-Bone-IK, damit die Hand den bearbeiteten Gegenstand tatsächlich erreicht. Bei Bedarf gehen die Figuren vorher näher heran oder stellen sich auf die Zehenspitzen. Getragene Gegenstände folgen der Hand.
- **Kollision:** Die Figuren laufen nie durch Maschine, Tisch, Hologramm oder Ersatzteile. Alle Bedienelemente liegen in Greifhöhe.
- **Smarty:** freundlicher Roboter mit Display-Gesicht, dessen Augen glücklich oder traurig schauen, und einer leuchtenden Antenne.

## Ton

- **Sprachausgabe:** Alle Sprechblasen werden mit der Web Speech API vorgelesen.
  - **Nur Hochdeutsch (de-DE):** keine Schweizer oder österreichischen Stimmen und keine Novelty-Stimmen. Die beste verfügbare Qualität wird bevorzugt („Natural“/„Online“, Google Deutsch, Premium/Enhanced).
  - Jede Figur bekommt nach Möglichkeit eine eigene Stimme. Tonhöhe und Tempo bleiben nahe am Natürlichen, Smarty klingt nur leicht höher.
  - Die Sätze laufen über eine Warteschlange und werden nie abgebrochen.
  - Gegen abgeschnittene Wörter: eine kurze Pause am Satzanfang und ein Satzzeichen am Ende, Referenzen auf die Utterances halten (Chrome-Fehler) und ein Watchdog, falls das Ende nicht gemeldet wird.
  - Alle Sätze sind einfache, verständliche Alltagssprache ohne Fachjargon.
- **Hintergrundmusik:** live mit der Web Audio API erzeugt, fröhlich, modern und unaufdringlich. Etwa 104 BPM mit den Akkorden C–G–Am–F, weichem Bass, Arpeggio, sanften Drums und einer Melodie im Wechsel. Die Musik startet beim ersten Klick und wird leiser, während jemand spricht.
- **Ton-Knopf:** Ein Knopf in der Kopfzeile schaltet Musik und Sprache zusammen ein und aus.

## Darstellung und Bedienung

- **Kamera:** Die Szene wird mit Finger oder Maus gedreht und mit zwei Fingern gezoomt. Die Kamera fliegt je nach Aufgabe automatisch an die passende Stelle.
- **Smartphone, Hochformat:** kompakte Kopfzeile und ein Textfeld unten. Die Personenkarten stehen in drei Spalten, mit Silbentrennung für lange Berufsnamen.
- **Smartphone, Querformat:** Das Textfeld steht rechts als Seitenleiste, die 3D-Szene wird links daneben zentriert.
- **Nichts wird abgeschnitten:**
  - 3D-Schilder verkleinern ihre Schrift automatisch, bis sie passt.
  - Sprechblasen brechen um und bleiben immer im Bild.
  - Der Haupt-Knopf (Losschicken / Nächstes Level / Nochmal spielen) bleibt immer sichtbar, auch wenn das Textfeld scrollt.
- **Fehlerfälle:** Fehlt WebGL oder lädt die 3D-Bibliothek nicht, erscheint ein freundlicher Hinweis.
- **Barrierefreiheit:** reduzierte Animationen bei `prefers-reduced-motion`, ARIA-Labels, Fokus-Rahmen und Touch-Ziele von mindestens 44 px.
