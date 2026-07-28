# Immobilien-Cockpit

Verwaltungs-Cockpit für den Immobilienbestand Specht & Waschkowski – eine einzelne HTML-Datei, keine Installation nötig.

## Nutzung

1. `index.html` öffnen – entweder direkt oder über GitHub Pages.
2. Beim ersten Start die lokale Datei `immobilien-daten.json` hineinziehen (liegt **nicht** in diesem Repo – Datenschutz!).
3. Die Daten werden nur im Browser (localStorage) gespeichert und verlassen den Rechner nicht.

## Funktionen

- **Übersicht:** Kennzahlen, Cashflow, Warnungen, Miete vs. Rate je Objekt
- **Objekte:** Details, Mieter, Finanzierung, Street-View-Button je Objekt
- **Bank & Zahlungen:** CSV-/CAMT-Import aus dem Online-Banking, automatische Zuordnung eingehender Mieten (IBAN → Name → Betrag), Soll/Ist je Monat, manuelle Nachzuordnung
- **Mietspiegel-Check:** €/m² je Einheit vs. ortsübliche Vergleichsmiete, Wartefrist (§558 BGB) und Kappungsgrenze, Erhöhungspotenzial
- **Erinnerungen:** automatisch abgeleitete Termine (Mieterhöhungen, Zinsbindungen, BK-Fristen) als .ics-Download
- **KI-Fragen:** Fragen an Claude mit vollem Portfolio-Kontext (eigener Anthropic-API-Key nötig, wird nur lokal gespeichert)

## Datenschutz

Objekt- und Mieterdaten liegen ausschließlich in der lokalen `immobilien-daten.json` bzw. im Browser-Speicher. Dieses Repo enthält nur den Code.
