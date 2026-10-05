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
| `index.html` | das komplette Spiel; HTML, CSS, JavaScript, Logo und QR-Code sind eingebettet |
| `vendor/three.min.js` | 3D-Bibliothek three.js r128. Fehlt sie, wird sie automatisch von cdnjs geladen. |
| `vendor/three-LICENSE.txt` | MIT-Lizenz von three.js |
| `assets/` | Original-Logo und Bewerbungs-QR-Code, nur zur Referenz. Das Spiel nutzt die eingebetteten Kopien. |
| `docs/PROMPT.md` | Beschreibung bzw. Prompt, mit dem sich das Spiel nachbauen lässt |
| `.nojekyll` | sorgt dafür, dass GitHub Pages die Dateien unverändert ausliefert |

## Hinweise

- **Browser:** Läuft in aktuellen Versionen von Chrome, Edge, Firefox und Safari, auch auf Smartphones im Hoch- und Querformat. WebGL wird benötigt.
- **Ton:** Musik und Sprachausgabe starten nach dem ersten Klick, weil Browser Ton vorher blockieren. Oben rechts lässt sich der Ton ein- und ausschalten.
- **Stimmen:** Das Spiel nutzt die Sprachausgabe des Browsers und wählt nur hochdeutsche Stimmen. Am natürlichsten klingt es in Microsoft Edge („Natural“-Stimmen) und in Chrome („Google Deutsch“).
- **Logo und QR-Code ändern:** Beide sind als Base64-Bilder in `index.html` eingebettet. Zum Austauschen in `index.html` nach `data:image/png;base64` suchen. Das erste Vorkommen ist das Logo, das zweite der QR-Code. Den jeweiligen Wert durch das neue Bild ersetzen, ebenfalls als Base64-PNG.

## Rechte

- **three.js:** © three.js authors, MIT-Lizenz (siehe `vendor/three-LICENSE.txt`)
- **Logo und Bewerbungs-QR-Code:** © Technologie-Initiative SmartFactory KL e.V.
- **Lizenz des Spiels:** Für das Spiel selbst ist noch keine Lizenz festgelegt. Bei einem öffentlichen Repository sollte eine `LICENSE`-Datei ergänzt werden.
