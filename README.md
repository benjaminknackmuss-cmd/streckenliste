# Streckenliste

Einfache, offline-fähige App (PWA) zum Erfassen von Abschüssen im Revier. Am Ende des Jagdjahres (1. April bis 31. März) erzeugt sie eine Streckenliste als PDF zum Drucken oder Verschicken.

**App öffnen:** https://benjaminknackmuss-cmd.github.io/streckenliste/

## Installation auf Android
1. Link oben in Chrome öffnen.
2. Oben rechts auf die drei Punkte tippen, dann „App installieren“ bzw. „Zum Startbildschirm hinzufügen“.
3. Danach funktioniert die App auch ohne Netz.

## Funktionen
- Erfassung: Wildart, Geschlecht, Altersklasse, Datum/Uhrzeit, Ort (auch per GPS), Erleger, Gewicht, Art des Abgangs, Besonderheiten, Wildmarke, Trichinenprobe, Verwertung.
- PDF-Streckenliste (A4 quer): Einzelnachweis, Zusammenfassung je Wildart, Unterschriftszeile. Teilen per E-Mail/WhatsApp.
- Datensicherung (JSON) senden und einspielen, CSV-Export für Excel.
- „Hilfe anfordern“: Meldung mit Nummer an den Helfer, inkl. Link zum Anlegen eines GitHub-Tickets (Label `hilfe`).

## Technik
Reines HTML/CSS/JS ohne Build-Schritt. Daten liegen nur im `localStorage` des Geräts. PDF mit jsPDF + jspdf-autotable (lokal in `vendor/`). `sw.js` cached alles für den Offline-Betrieb.
