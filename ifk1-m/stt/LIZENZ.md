# Spracherkennung für den Zahlen-Sprint

Zwei Fremddateien, beide unter der Apache-Lizenz 2.0:

| Datei | Was | Quelle |
|---|---|---|
| `vosk.js` | vosk-browser 0.0.8, WebAssembly-Fassung des Erkenners Vosk/Kaldi für den Browser (Ciaran O'Reilly) | https://github.com/ccoreilly/vosk-browser · npm `vosk-browser@0.0.8`, `dist/vosk.js` unverändert |
| `model-de.tar.gz` | Vosk-Modell `vosk-model-small-de-0.15` (Alpha Cephei Inc., 2020), deutsches Sprachmodell für mobile Anwendungen, 46 MB | https://alphacephei.com/vosk/models · aus dem ZIP unverändert als tar.gz gepackt (Ordner `model/`) |

Das Applet `../zahlen-sprint-applet.html` lädt beide Dateien nur, wenn Sprechen an ist und
eine Runde oder der Mikrofontest beginnt; das Modell wandert in den Cache-Speicher des
Browsers. Die Erkennung läuft vollständig auf dem Gerät, es werden keine Aufnahmen gesendet.

Lizenztext: https://www.apache.org/licenses/LICENSE-2.0
