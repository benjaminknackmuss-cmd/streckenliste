# Streckenliste – Hinweise für Claude

- Nutzer der App: ein älterer Jäger (Vater von Benjamin) auf Android/Chrome. Oberfläche komplett auf Deutsch, große Knöpfe, einfache Sprache (Sie-Form).
- Kein Build-Schritt: `index.html` enthält CSS und JS. Wird über GitHub Pages von `main` (Root) ausgeliefert.
- Bei jeder Änderung an ausgelieferten Dateien `CACHE` in `sw.js` hochzählen (`streckenliste-vN`) und `APP_VERSION` und `APP_DATE` in `index.html` erhöhen (Version wird in der App unten und in den Einstellungen angezeigt), damit Handys die neue Version laden.
- Gespeicherte Daten (`localStorage`-Schlüssel `streckenliste.v1`, `streckenliste.settings.v1`, `streckenliste.tickets.v1`, `streckenliste.zugang.v1`) niemals inkompatibel ändern: Einträge des Vaters dürfen nicht verloren gehen. Neue Felder nur optional ergänzen.
- Hilfe-Tickets kommen als GitHub-Issues mit Label `hilfe`. Vorgehen: Problem nachstellen (Playwright, Handy-Viewport 390×844), Fix auf eigenem Branch, PR mit deutscher Beschreibung, im Issue kurz auf Deutsch antworten, was geändert wurde.
- Bei jeder neuen Version oben in `NEUES` (index.html, Abschnitt „Was ist neu?“) einen Eintrag ergänzen: kurze Überschrift + ein, zwei Sätze in einfacher Sprache (Sie-Form), was der Vater jetzt anders oder neu machen kann. Reine Fehlerbehebungen kurz als „Fehler behoben: …“. Die App zeigt das nach dem Update einmal an.
