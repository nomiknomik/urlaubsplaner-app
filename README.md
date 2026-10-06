# Urlaubsplaner

Jahresplaner für die Ferienbetreuung: er zeigt, welche betreuungspflichtigen
Ferientage schon abgedeckt sind und wo Lücken bleiben. Eine einzige Datei,
`index.html`, ohne Build und ohne Abhängigkeiten.

**→ [Planer öffnen](https://nomiknomik.github.io/urlaubsplaner-app/)**

## Was er kann

* Jahresraster 12 × 31 — das ganze Jahr ohne Scrollen, Arbeits- und Druckansicht
  in einem.
* Urlaub und Betreuungsquellen per Klick und Ziehen eintragen, Blöcke benennen.
* Lückenanalyse: betreuungspflichtige Werktage gegen das, was abgedeckt ist,
  mit Kalenderwochen, Brückentagen und einer Warnung vor gemeinsamem Urlaub —
  der kostet zwei Urlaubstage und deckt nur einen Betreuungstag ab.
* Schulferien Baden-Württemberg für 2027 und 2028 eingebaut, weitere Jahre über
  [openholidaysapi.org](https://openholidaysapi.org) oder von Hand. Gesetzliche
  Feiertage werden aus dem Ostersonntag berechnet.
* Besondere Termine (Fortbildung, Kongress) sperren Tage für Urlaub.
* Druck auf eine Seite A4 quer, inklusive Bilanz und Legende.
* Online-Abgleich mehrerer Geräte über eine **verschlüsselte** Datei in einem
  **privaten** GitHub-Repo, mit Zusammenführung Eintrag für Eintrag.

## Daten

Alles bleibt im Browser. Es gibt keinen Server, keine Konten, keine Tracker und
keine externen Skripte. Namen trägst du selbst ein; dieser Quelltext kennt
keine. Für den Geräteabgleich legst du selbst ein privates Repo und einen
Fine-grained-Token an — beides bleibt in deiner Hand, der Dateiinhalt ist mit
deinem Passwort verschlüsselt (AES-GCM-256, PBKDF2-SHA256).

## Herkunft

Dieses Repo ist nur die Auslieferung für GitHub Pages und enthält bewusst nur
die ausgelieferte Datei. Entwicklung, Konzept und Abnahmeprüfung liegen in
einem separaten, privaten Repo.
