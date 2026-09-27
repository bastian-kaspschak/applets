# Applets

Öffentliches Repository für die interaktiven Applets aus dem Physik- und Mathematikunterricht
von Bastian Kaspschak (Lore-Lorentz-Schule). Schülerinnen und Schüler erreichen die Applets über GitHub
Pages:

**https://bastian-kaspschak.github.io/applets/**

## Inhalt

| Datei | Kurs, Reihe | Was das Applet zeigt |
|---|---|---|
| `11nf-ph/mittelwert-sigma-applet.html` | 11NF PH, Messen und Messfehler (September 2026) | Mittelwert als Schätzwert für den wahren Wert, Standardabweichung als typische Abweichung; Abweichungen als Pfeile, ihre Quadrate, das mittlere Quadrat und seine Seite σ; Histogramm der Messwerte mit x̄ ± σ |
| `11nf-ph/zielscheibe-applet.html` | 11NF PH, Messen und Messfehler (September 2026) | Die Zielscheibe des A3-Blatts aus dem Unterricht mit zwei Reglern, Verschiebung (systematischer Fehler) und Wackeln (statistischer Fehler); Würfe simulieren, Mittelwert als Kreuz und Streubereich x̄ ± σ sehen, Histogramm der Treffer je 1-cm-Feld mit Farbskala, Kennzahlen wie auf dem Arbeitsblatt |
| `11nf-ph/zwei-sigma-applet.html` | 11NF PH, Messen und Messfehler (September 2026) | Zapfsäule auf dem Prüfstand des Eichamts: jede Zapfung als Füllstand im Hals der Eichkanne und als Punkt auf der Liter-Achse, Säulendiagramm je 5 ml, Streifen x̄ ± 1σ, ± 2σ, ± 3σ mit „x von n = y %“, Regler für die Streuung; die ersten 30 Zapfungen sind fest, damit Unterricht und Hausaufgabe dieselben Zahlen zeigen |
| `11nf-pht/nonius-applet.html` | 11NF PHT-Pr, Messen und Messfehler (September 2026) | Messschieber von vorn (Schiene, Schieber mit Nonius und Schnabel, Werkstück), Nonius 1/10, 1/20 oder 1/50 mm; Schieber ziehen oder Zufallswert, ablesen, eintippen, prüfen; Lupe folgt dem Finger, Anzeige markiert den passenden Noniusstrich; Aufgaben 1 bis 4 und die drei Schritte des Messens |
| `11wi2-m/zwei-punkte-applet.html` | 11WI2 M, Von Daten zu Funktionen I (September 2026) | Zwei Punkte im Koordinatensystem ziehen (Raster 1 oder 0,5) oder zufällig setzen, Graph mit Steigungsdreieck ein- und ausblenden, Funktionsgleichung eingeben und prüfen; die Eingabe wird als Term gelesen (2x + 3, 3 + 2x, y = 2x + 3, 2/3x − 1), gerundete Dezimalzahlen gelten als „fast richtig“; nach dem Prüfen der Rechenweg in vier Schritten mit Probe und ein Hinweis auf den Schritt, an dem es hängt |
| `11wi2-m/gewinnschwelle-applet.html` | 11WI2 M, Von Daten zu Funktionen I (September 2026) | Betrieb wählen (WI-Shirt, drei weitere, eigene Werte) oder Preis p, Stückkosten kᵥ und Fixkosten K_f mit Reglern einstellen; Graph der Gewinnfunktion G(x) mit markierter Nullstelle, Verlust- und Gewinnzone auf der x-Achse und G(0) = −K_f auf der y-Achse; Kontrolle G(⌊x₀⌋), G(⌈x₀⌉) zum Aufrunden; „E(x) und K(x) einblenden“ zeigt Erlös- und Kostengerade mit dem Schnittpunkt über der Nullstelle |
| `12pe1-m/extrempunkte-applet.html` | 12PE1 M, Extremwertprobleme (September 2026) | Sechs Beispielfunktionen; f, f′ und f″ untereinander mit ziehbarem Punkt und Tangente, f′ und f″ ausblendbar; Rechenweg zu den Extrempunkten in vier Schritten (notwendige und hinreichende Bedingung), jeder Schritt in den Graphen markiert |
| `12pe1-m/ableitungs-sprint-applet.html` | 12PE1 M, Differenzialrechnung (ab September 2026, wird im Schuljahr um weitere Funktionstypen erweitert) | Übungsspiel mit ablaufender Zeit (2, 3 oder 5 Minuten, oder ohne Zeit): zu jeder zufällig erzeugten ganzrationalen Funktion f′(x) und f″(x) bilden (einstellbar nur f′ oder bis f‴), Grad 2 bis 5 wählbar, auf Wunsch mit Bruchkoeffizienten; jede richtige Ableitung ein Punkt. Die Eingabe wird als Term gelesen (Reihenfolge der Summanden egal, „stimmt, aber fasse zusammen“ bei zu vielen Summanden) und an acht Stellen mit der Ableitung verglichen. Eingabe über eigene Tasten (x, x², x³, x⁴, Brüche; am PC auch die Tastatur; Systemtastatur oder Scribble in ein Textfeld, x2 gilt als x²) oder mit dem Stift: Handschrifterkennung im Gerät ohne Dienst und Bibliothek (Striche werden nach Lage zu Zeichen gruppiert, Hochzahlen rechts oben, Bruchstriche, Komma und Malpunkt; jedes Zeichen liest ein kleines Faltungsnetz, 90.000 Parameter als 120 KB im Applet, trainiert auf dem freien Datensatz HASYv2 und gesammelten Handschriftproben), Anzeige des Gelesenen, Korrektur per Tipp auf das Zeichen; Korrekturen und „Zeichen trainieren“ sammeln Proben, die per „Handschrift exportieren“ als JSON-Datei in die nächste Fassung des Erkenners einfließen, oder durch Sprechen („sechs x hoch zwei minus vier x plus drei“, auch „x Quadrat“, „ein halb x“, „null Komma fünf x“): derselbe Erkenner wie im Zahlen-Sprint (Vosk als WebAssembly, deutsches Modell aus `ifk1-m/stt/`, 46 MB, einmal geladen, bleibt im Gerät), Grammatik aus Zahlwörtern, x, hoch, quadrat, plus, minus, Bruchwörtern; das Zuhören beginnt bei jeder Aufgabe von selbst, Mikrofontest auf der Startseite. Bei Fehlern bleibt die Eingabe zum Verbessern stehen oder „Lösung zeigen“; Fehlerliste am Ende, Rekord im Browser, Teilen als Bild oder Text |
| `12pe1-m/gleichungs-sprint-applet.html` | 12PE1 M, Gleichungen (ab September 2026) | Übungsspiel mit ablaufender Zeit (3, 5 oder 10 Minuten, oder ohne Zeit): zufällige lineare (1 Punkt) und quadratische Gleichungen (2 Punkte), Zeile für Zeile wie im Heft mit der Umformung rechts (−3, :2, ·4, −2x). Geprüft wird jeder Schritt mit exakter Bruchrechnung: die neue Gleichung muss aus der angegebenen Umformung folgen, Vereinfachen und Ausmultiplizieren brauchen keine Angabe, fehlende oder unpassende Umformungen werden benannt („gerechnet hast du −2“), Multiplizieren mit x gilt nicht als Äquivalenzumformung. Quadratisch: erst Normalform, dann pq-Formel mit eingesetzten Zahlen (auch vereinfacht 2 ± 1), dann x₁ = …; x₂ = …, x = … oder „keine Lösung“. „Schritt zeigen“ berechnet den nächsten Schritt aus der aktuellen Zeile mit Erklärung, die Gleichung zählt dann keine Punkte. Eigene Tasten (x, x², √, ±, |, =, x₁,₂ =) oder Systemtastatur, Fehlerliste am Ende, Rekord im Browser, Teilen als Bild oder Text |
| `ifk1-m/zahlen-sprint-applet.html` | IFK1 M, Mathe als Sprache (September 2026) | Übungsspiel fürs Handy mit ablaufender Zeit (1, 2 oder 3 Minuten): kurze Aufgaben in zufälliger Reihenfolge, gezählt werden die richtigen Antworten. Zahlwörter wählen, tippen, schreiben, hören (Sprachausgabe) und sprechen (Zahl, Ordnungszahl, Uhrzeit, Datum, Bruch, Rechnung über einen eigenen Erkenner im Browser: Vosk als WebAssembly mit deutschem Modell in `ifk1-m/stt/`, 46 MB, wird beim ersten Start geladen und bleibt im Gerät; drei Versuche, kein Selbstvergleich, Mikrofontest und Ausschalter auf der Startseite), Zählen an Bildern, Reihen, Ordnen, Paare; Ordnungszahlen, Uhrzeit, Datum, Brüche, Rechnungen in Worten und Zeichen, richtig/falsch, Summe/Differenz/Produkt/Quotient, Rechen- und Vergleichszeichen; Themen abwählbar, Fehlerliste am Ende, Rekord im Browser, Teilen als Bild oder Text |

`index.html` an der Wurzel ist nur die Liste der Kurse. Die Applets selbst stehen auf der
`index.html` des jeweiligen Kursordners.

## Ordnerstruktur

Jeder Kurs hat einen eigenen Ordner. Der Ordnername ist die Kurs-ID aus dem Planungsrepository
(`Jahresplanungen/stunden/<kursId>/`), damit Quelle und Kopie denselben Schlüssel tragen:

| Ordner | Kurs |
|---|---|
| `11nf-ph/` | 11NF PH |
| `11nf-pht/` | 11NF PHT und 11NF PHT-Pr (ein gemeinsamer Ordner für Theorie und Praktikum) |
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
- **Eine Ausnahme vom „nichts nachladen“:** Die Sprechaufgaben des Zahlen-Sprints (IFK1 M)
  brauchen einen Spracherkenner. Die Erkennungsdienste der Browser (Google, Microsoft) fielen auf
  den Geräten der Klasse aus, deshalb liegt ein eigener Erkenner neben dem Applet:
  `ifk1-m/stt/vosk.js` (Vosk als WebAssembly) und `ifk1-m/stt/model-de.tar.gz` (deutsches
  Modell, 46 MB), beide Apache 2.0, siehe `ifk1-m/stt/LIZENZ.md`. Geladen wird nur, wenn
  Sprechen an ist und eine Runde oder der Mikrofontest beginnt; das Modell bleibt im
  Cache-Speicher des Browsers, die Erkennung läuft auf dem Gerät, Aufnahmen verlassen es nicht.
  Der Ableitungs-Sprint (12PE1 M) nutzt dieselben zwei Dateien über den Pfad `../ifk1-m/stt/`
  (Rückfall: ein Ordner `stt/` neben dem Applet) und denselben Cache-Namen, damit ein Gerät das
  Modell nur einmal lädt. Der Ordner `ifk1-m/stt/` darf deshalb nicht umziehen, ohne beide
  Applets anzupassen.

## Pflege

Die Quelle jedes Applets liegt im (privaten) Planungsrepository im Materialordner der zugehörigen
Stunde, hier `Jahresplanungen/stunden/11nf-ph/2026-09-04-organisation/material/`,
`Jahresplanungen/stunden/11nf-ph/2026-09-08-physikalische-grossen/material/`,
`Jahresplanungen/stunden/11nf-ph/2026-09-11-ubung-zehnerpotenzen-vorsilben-grossenordnungen/material/`,
`Jahresplanungen/stunden/11wi2-m/2026-09-14-ubung-geradengleichungen-aufstellen-und-deuten/material/`
und `Jahresplanungen/stunden/12pe1-m/2026-09-04-wiederholung/material/`. Ein Applet, das keiner
einzelnen Stunde gehört, liegt im Kursordner des Planungsrepositories, hier
`Jahresplanungen/kurse/ifk1-m/` (Zahlen-Sprint, Bildbausteine in `bilder/`) und
`Jahresplanungen/kurse/12pe1-m/` (Ableitungs-Sprint, dazu der Kerntest `test-ableitungs-sprint.mjs`). Dieses Repo enthält nur
Kopien für die Veröffentlichung; im Workspace ist es als `applets/` neben `Vault/` und
`Jahresplanungen/` ausgecheckt. Nach einer Änderung an der Quelle:

1. Datei in den Kursordner `<kursId>/` kopieren. Ist es das erste Applet des Kurses: Ordner
   anlegen, die `index.html` eines bestehenden Kursordners hineinkopieren, Kursname in Titel,
   Kopfzeile, Überschrift und Fußzeile anpassen, Liste leeren, und den Kurs in der `index.html`
   an der Wurzel eintragen.
2. Bei einem neuen Applet je einen Eintrag in der `index.html` des Kursordners und in der
   Tabelle oben ergänzen.
3. Committen und pushen. GitHub Pages veröffentlicht den Stand von `main` innerhalb etwa einer
   Minute.

Hier liegt nur, was Schüler sehen dürfen: keine Lösungen, keine Klausuren, keine Lehrerfassungen.
