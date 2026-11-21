# Rückwärts – Sprachspiel

Web-App fürs Handy: Ein Wort aufnehmen, rückwärts anhören, das Rückwärts nachsprechen und die Nachahmung wieder umdrehen. Wer gut nachspricht, hört am Ende das Original.

## Ablauf
1. **Aufnehmen** – bis zu 8 Sekunden. Stille am Anfang und Ende wird automatisch abgeschnitten, die Lautstärke angeglichen.
2. **Nachsprechen** – Vorlage rückwärts anhören (optional langsamer), dann nachsprechen. Gern auch eine zweite Person.
3. **Ergebnis** – die Nachahmung wird umgedreht und abgespielt; Vergleich mit dem Original per Knopfdruck.

Alles läuft im Browser (Web Audio API + MediaRecorder). Es wird nichts hochgeladen.

## Starten
Das Mikrofon funktioniert nur über **https** (oder `localhost`).

Lokal:
```bash
python3 -m http.server 8000
```
Dann `http://localhost:8000` öffnen.

Aufs Handy: z. B. über GitHub Pages veröffentlichen (Settings → Pages → Branch wählen, Ordner `/`). Die App lässt sich dann über „Zum Home-Bildschirm“ installieren und funktioniert offline.

## Dateien
- `index.html` – komplette App (HTML, CSS, JS)
- `manifest.webmanifest`, `sw.js` – Installierbarkeit und Offline-Cache
- `icon.svg`, `icon-*.png`, `apple-touch-icon.png` – App-Icons

Design: RSJ-Design (Tinte/Limette, Montserrat + Open Sans).
