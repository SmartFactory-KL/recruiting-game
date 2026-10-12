# Smartys Kaffeepanne

Ein kleines 3D-Browserspiel der **Technologie-Initiative SmartFactory KL e.V.**: Der Transportroboter Smarty rammt die Kaffeemaschine, und die Spielenden schicken die richtigen Fachkräfte los, um sie zu reparieren:

- **Tanja** (Technikerin) für die Elektrik
- **Sam** (Programmierer\*in) für die Software
- **Jonas** (Maschinenbauingenieur) für das Getriebe

Es gibt vier Level. Das letzte ist ein Team-Einsatz mit allen dreien. Am Ende erscheint ein Bewerbungsaufruf mit QR-Code.

> Mit KI generierter Inhalt. Das Spiel wurde mit Unterstützung von Claude (Anthropic) erstellt.

## Spielen

**Online über GitHub Pages**

1. Den Inhalt dieses Ordners in ein GitHub-Repository hochladen. `index.html` muss im Hauptverzeichnis liegen.
2. Im Repository unter **Settings → Pages** bei „Source“ den Punkt **Deploy from a branch** wählen, dann den Branch `main` mit dem Ordner `/ (root)` auswählen und speichern.
3. Nach ein bis zwei Minuten ist das Spiel unter `https://<benutzername>.github.io/<repository-name>/` erreichbar.

**Lokal**

`index.html` im Browser öffnen. Der Ordner `vendor/` muss daneben liegen.

## Ordnerstruktur

| Pfad | Inhalt |
|---|---|
| `index.html` | das komplette Spiel; HTML, CSS, JavaScript, Schriften, Logo und QR-Code sind eingebettet |
| `vendor/three.min.js` | 3D-Bibliothek three.js r128 |
| `vendor/three-LICENSE.txt` | MIT-Lizenz von three.js |
| `vendor/fonts-OFL-LICENSE.txt` | Lizenz der eingebetteten Schriften (SIL Open Font License 1.1) |
| `assets/` | Original-Logo und Bewerbungs-QR-Code, nur zur Referenz. Das Spiel nutzt die eingebetteten Kopien. |
| `docs/PROMPT.md` | Beschreibung bzw. Prompt, mit dem sich das Spiel nachbauen lässt |
| `LICENSE` | MIT-Lizenz für den Code des Spiels |
| `.nojekyll` | sorgt dafür, dass GitHub Pages die Dateien unverändert ausliefert |

## Hinweise

- **Browser:** Läuft in aktuellen Versionen von Chrome, Edge, Firefox und Safari, auch auf Smartphones im Hoch- und Querformat. WebGL wird benötigt.
- **Ton:** Musik und Sprachausgabe starten nach dem ersten Klick, weil Browser Ton vorher blockieren. Oben rechts lässt sich der Ton ein- und ausschalten.
- **Stimmen:** Das Spiel nutzt die Sprachausgabe des Browsers und wählt nur hochdeutsche Stimmen. Am natürlichsten klingt es in Microsoft Edge („Natural“-Stimmen) und in Chrome („Google Deutsch“).
- **Logo und QR-Code ändern:** Beide sind als Base64-Bilder in `index.html` eingebettet. Zum Austauschen in `index.html` nach `data:image/png;base64` suchen. Das erste Vorkommen ist das Logo, das zweite der QR-Code. Den jeweiligen Wert durch das neue Bild ersetzen, ebenfalls als Base64-PNG.

## Lizenz

Der Code des Spiels steht unter der **MIT-Lizenz** (siehe [`LICENSE`](LICENSE)).

**Ausgenommen** davon sind das Logo der SmartFactory KL und der Bewerbungs-QR-Code, im Ordner `assets/` und eingebettet in `index.html`. Beide bleiben Eigentum der Technologie-Initiative SmartFactory KL e.V. und dürfen nicht ohne Erlaubnis weiterverwendet werden. Wer das Spiel für eigene Zwecke anpasst, ersetzt Logo und QR-Code bitte durch eigene.

Die mitgelieferte 3D-Bibliothek three.js steht ebenfalls unter der MIT-Lizenz, © three.js authors (siehe `vendor/three-LICENSE.txt`).

Die Schriften Chakra Petch, Atkinson Hyperlegible und IBM Plex Mono sind in `index.html` eingebettet und stehen unter der SIL Open Font License 1.1 (siehe `vendor/fonts-OFL-LICENSE.txt`).

## Datenschutz

Das Spiel lädt keine Inhalte von fremden Servern: Schriften und die 3D-Bibliothek liegen im Projekt, es gibt kein Google Fonts, kein CDN, keine Cookies und kein Tracking. Externe Verbindungen entstehen nur, wenn jemand den Karriere-Link bzw. QR-Code öffnet (smartfactory.de). Hinweis: Manche Browser-Stimmen (z. B. „Natural“-Stimmen in Edge, „Google Deutsch“ in Chrome) erzeugen die Sprachausgabe auf Servern von Microsoft bzw. Google; dabei werden nur die festen Spieltexte übertragen.
