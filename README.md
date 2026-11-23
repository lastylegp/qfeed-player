# qfeed-player

Kleine Player-Seite für [Q-Feed](https://github.com/lastylegp/QFeed) auf Samsung-TVs (Tizen).

YouTube spielt eingebettete Videos nur auf Seiten mit echter Web-Adresse ab
(sonst „Fehler bei der Konfiguration des Videoplayers“ / Fehler 153). Eine Tizen-App ist
eine lokale Datei – deshalb lädt Q-Feed diese Seite per GitHub Pages im integrierten Player:

```
https://lastylegp.github.io/qfeed-player/?v=<VIDEO-ID>
```

Steuerung erfolgt per `postMessage` aus der App (Play/Pause, Spulen), die Seite meldet
Zeit, Dauer und Status zurück. Keine Daten, kein Tracking, keine Zugangsdaten.
