# Handball-Tracker

PWA zum Erfassen von Spielergebnissen (Torschützinnen, 7-Meter, Strafen) und Trainingsbewertungen (Anwesenheit, Bewertung pro Spielerin, Trainingsfazit). Jedes Ereignis kann als Markdown-Datei exportiert werden — im Format passend zum Second Brain (`20 - Bereiche/Handball/Saison & Spiele`).

## Funktionen

- **Spiele:** Gegner, Heim/Auswärts, Ergebnis (+ Halbzeit), pro Spielerin Anwesenheit (da / entschuldigt / unentschuldigt), Bewertung 1–5 Sterne + Notiz, Feldtore, 7m verwandelt/verworfen, 2-Minuten-Strafen, gelbe/rote Karten, Notizen (beste Spielerinnen, was lief gut, Verbesserungspunkte, Fazit)
- **Trainings:** Anwesenheit (da / entschuldigt / unentschuldigt), Bewertung 1–5 Sterne + Notiz pro Spielerin, bis zu 9 durchgeführte Übungen (Name mit Vorschlägen, 1–5 Sterne „wie hat's funktioniert", Notiz), Gesamtbewertung des Trainings
- **MD-Export:** pro Ereignis über den 📄-Button — auf dem Handy per Teilen-Dialog, sonst als Download
- **Statistik:** Saison-Bilanz, Torschützinnenliste, Spiel- und Trainingsbeteiligung mit Ø-Bewertung
- **Kader:** Spielerinnen hinzufügen, umbenennen, deaktivieren (vorbefüllt mit dem aktuellen Kader)
- **Backup:** Alle Daten liegen im localStorage des Geräts; JSON-Export/-Import unter „Kader → Daten"

## Technik

Wie der Bewegungstracker: eine `index.html` (HTML/CSS/JS inline), `manifest.json`, `sw.js` (Network-first mit Offline-Cache), kein Build-Schritt. Installierbar über „Zum Startbildschirm hinzufügen".
