# Applets

Öffentliches Repository für die interaktiven Applets aus dem Physik- und Mathematikunterricht
von Bastian Kaspschak (Lore-Lorentz-Schule). Schülerinnen und Schüler erreichen die Applets über GitHub
Pages:

**https://bastian-kaspschak.github.io/applets/**

## Inhalt

| Datei | Kurs, Reihe | Was das Applet zeigt |
|---|---|---|
| `11nf-ph/mittelwert-sigma-applet.html` | 11NF PH, Messen und Messfehler (September 2026) | Mittelwert als Schätzwert für den wahren Wert, Standardabweichung als typische Abweichung; Abweichungen als Pfeile, ihre Quadrate, das mittlere Quadrat und seine Seite σ |
| `12pe1-m/extrempunkte-applet.html` | 12PE1 M, Extremwertprobleme (September 2026) | Sechs Beispielfunktionen; f, f′ und f″ untereinander mit ziehbarem Punkt und Tangente, f′ und f″ ausblendbar; Rechenweg zu den Extrempunkten in vier Schritten (notwendige und hinreichende Bedingung), jeder Schritt in den Graphen markiert |

`index.html` an der Wurzel ist die Gesamtübersicht, nach Kursen gegliedert. Jeder Kursordner hat
eine eigene `index.html`, die nur die Applets dieses Kurses zeigt.

## Ordnerstruktur

Jeder Kurs hat einen eigenen Ordner. Der Ordnername ist die Kurs-ID aus dem Planungsrepository
(`Jahresplanungen/stunden/<kursId>/`), damit Quelle und Kopie denselben Schlüssel tragen:

| Ordner | Kurs |
|---|---|
| `11nf-etec/` | 11NF ETEC |
| `11nf-ph/` | 11NF PH |
| `11nf-pht/` | 11NF PHT |
| `11nf-pht-pr/` | 11NF PHT-Pr |
| `11np-pht-pr/` | 11NP PHT-Pr |
| `11wi2-m/` | 11WI2 M |
| `12pe1-m/` | 12PE1 M |
| `ifk1-m/` | IFK1 M |

Ein Ordner entsteht mit dem ersten Applet seines Kurses; leere Ordner gibt es nicht. Er enthält
die Applets des Kurses und eine `index.html` als Einstiegsseite. Daraus folgen zwei Adressen:

- **Die Klasse bekommt ihre Kursseite:** `https://bastian-kaspschak.github.io/applets/<kursId>/`.
  Ein Link oder QR-Code genügt für das ganze Schuljahr; neue Applets erscheinen dort von selbst.
- **Ein einzelnes Applet** (etwa als QR-Code auf dem Arbeitsblatt der Stunde):
  `https://bastian-kaspschak.github.io/applets/<kursId>/<datei>`.

Bis zum 06.09.2026 hieß das Repository `physik-applets` und lag flach; die Adressen unter
`https://bastian-kaspschak.github.io/physik-applets/` gibt es seither nicht mehr.

## Wie die Applets gebaut sind

- **Eine Datei, offline.** HTML, CSS, JavaScript und Schriften stecken in derselben Datei. Nach dem
  Laden braucht ein Applet kein Internet; es lädt nichts nach und sendet nichts. Was Schüler
  einstellen, bleibt in ihrem Browser.
- **Formeln** brauchen keine Bibliothek. Wo sie aufwendig sind (Wurzeln, Summen, Brüche im
  Mittelwert-Applet), stehen sie im Quelltext als LaTeX und werden von einem kleinen eingebauten
  Konverter als MathML gesetzt; Formelschrift ist Latin Modern Math (GUST Font License), als
  Base64 eingebettet — deshalb ist diese Datei rund 1 MB groß. Wo einfache Terme reichen
  (Extrempunkte-Applet), sind sie gewöhnliches HTML, und die Datei bleibt klein.
- **Browser:** jeder aktuelle Chrome, Edge, Firefox oder Safari, auch auf dem Handy. Sehr alte
  Browser ohne MathML zeigen die Formeln als Fließtext.

## Pflege

Die Quelle jedes Applets liegt im (privaten) Planungsrepository im Materialordner der zugehörigen
Stunde, hier `Jahresplanungen/stunden/11nf-ph/2026-09-04-organisation/material/` und
`Jahresplanungen/stunden/12pe1-m/2026-09-04-wiederholung/material/`. Dieses Repo enthält nur
Kopien für die Veröffentlichung; im Workspace ist es als `applets/` neben `Vault/` und
`Jahresplanungen/` ausgecheckt. Nach einer Änderung an der Quelle:

1. Datei in den Kursordner `<kursId>/` kopieren. Ist es das erste Applet des Kurses: Ordner
   anlegen und die `index.html` eines bestehenden Kursordners hineinkopieren, Kursname in
   Titel, Kopfzeile, Überschrift und Fußzeile anpassen, Liste leeren.
2. Bei einem neuen Applet je einen Eintrag in der `index.html` des Kursordners, in der
   `index.html` an der Wurzel unter der Kursüberschrift und in der Tabelle oben ergänzen.
3. Committen und pushen. GitHub Pages veröffentlicht den Stand von `main` innerhalb etwa einer
   Minute.

Hier liegt nur, was Schüler sehen dürfen: keine Lösungen, keine Klausuren, keine Lehrerfassungen.
