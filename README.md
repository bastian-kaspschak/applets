# Physik-Applets

Öffentliches Repository für die interaktiven Applets aus dem Physikunterricht von Bastian
Kaspschak (Lore-Lorentz-Schule). Schülerinnen und Schüler erreichen die Applets über GitHub
Pages:

**https://bastian-kaspschak.github.io/physik-applets/**

## Inhalt

| Datei | Kurs, Reihe | Was das Applet zeigt |
|---|---|---|
| `mittelwert-sigma-applet.html` | 11NF PH, Messen und Messfehler (September 2026) | Mittelwert als Schätzwert für den wahren Wert, Standardabweichung als typische Abweichung; Abweichungen als Pfeile, ihre Quadrate, das mittlere Quadrat und seine Seite σ |

`index.html` ist die Linkliste, die unter der Adresse oben erscheint.

## Wie die Applets gebaut sind

- **Eine Datei, offline.** HTML, CSS, JavaScript und Schriften stecken in derselben Datei. Nach dem
  Laden braucht ein Applet kein Internet; es lädt nichts nach und sendet nichts. Was Schüler
  einstellen, bleibt in ihrem Browser.
- **Formeln** stehen im Quelltext als LaTeX und werden im Browser als MathML gesetzt. Ein kleiner
  eingebauter Konverter übersetzt die benötigte LaTeX-Teilmenge; eine Formelbibliothek wird nicht
  nachgeladen. Formelschrift ist Latin Modern Math (GUST Font License), als Base64 eingebettet.
  Deshalb ist die Datei rund 1 MB groß.
- **Browser:** jeder aktuelle Chrome, Edge, Firefox oder Safari, auch auf dem Handy. Sehr alte
  Browser ohne MathML zeigen die Formeln als Fließtext.

## Pflege

Die Quelle jedes Applets liegt im (privaten) Planungsrepository im Materialordner der zugehörigen
Stunde, hier `Jahresplanungen/stunden/11nf-ph/2026-09-04-organisation/material/`. Dieses Repo
enthält nur Kopien für die Veröffentlichung. Nach einer Änderung an der Quelle:

1. Datei hierher kopieren,
2. bei einem neuen Applet einen Eintrag in `index.html` und in der Tabelle oben ergänzen,
3. committen und pushen. GitHub Pages veröffentlicht den Stand von `main` innerhalb etwa einer
   Minute.

Hier liegt nur, was Schüler sehen dürfen: keine Lösungen, keine Klausuren, keine Lehrerfassungen.
