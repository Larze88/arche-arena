# Arche-Arena

Ein Auto-Battler mit Tieren für zwei Personen, angelehnt an Super Auto Pets. Beide spielen im Browser auf ihrem eigenen Gerät und verbinden sich per Einladungslink.

**Spielen:** https://larze88.github.io/arche-arena/

## So funktioniert's

1. Seite öffnen, Namen eingeben, **Spiel erstellen**.
2. Den Einladungslink an die zweite Person schicken.
3. Beide kaufen gleichzeitig Tiere und Futter ein, danach kämpfen die Teams automatisch.

Die Nachrichten laufen über öffentliche MQTT-Server (HiveMQ und EMQX, beide parallel), dadurch klappt die Verbindung in jedem Netz, auch im Mobilfunk. Kämpfe berechnet jedes Gerät selbst aus demselben Zufalls-Startwert. Die Person, die das Spiel erstellt hat, muss die Seite offen lassen, weil ihr Browser den Spielablauf steuert.

Das ganze Spiel steckt in `index.html`, ohne Build-Schritt.
