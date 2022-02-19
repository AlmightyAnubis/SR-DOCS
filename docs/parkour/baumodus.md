# Parkour Baumodus

Im Parkour Baumodus lassen sich komplett eigene Parkour Karten auf einer 200x200 Blöcke großen Fläche bauen.
Als Hilfsmittel kann man auch WorldEdit anwenden, das ist besonders für Terraforming von Flächen sehr interessant.


## Parkour Blöcke
Baut man einen Parkour, kommt man an den Parkourblocken nicht vorbei, mit diesen kann man markieren, wo ein Parkour anfängt, wo es Checkpoints gibt und wo ein Parkour enden soll.
Man kann diese Parkour Blöcke entweder im Baumenü erhalten, welches im Inventar liegt oder alternativ über das `/parkour todo` Buch erhalten.

!!! abstract "Beachte"
	Jede Karte kann maximal einen Start- und Ende Block haben, es können jedoch mehrere Checkpoints auf einer Karte gesetzt werden.


## Aktionskarten
Damit mehrere Spieler ungestört gleichzeitig die Karten spielen können und alle mit weniger Lag spielen können, gibt es im Parkour Spielmodus kein Redstone.
Möchte man bestimmte Aktionen bei einem Spieler auslösen, haben wir dafür die [[Aktionskarten]] entwickelt, diese erlauben dir viele, teils im normalen Spiel nicht zugängliche Features zu nutzen.

## Veröffentlichen von Karten
Hast du deine Karte gebaut und alle [Parkour Blöcke](#parkour-blocke) verteilt, kannst du damit beginnen, deine Karte zu veröffentlichen.

Folgende Schritte werden benötigt, um eine Karte zu veröffentlichen:

- [ ] Start Block platzieren
- [ ] Ende Block platzieren
- [ ] Checkpoint Blöcke platzieren
- [ ] Spawnpunkt der Karte mit `/parkour setspawn` setzen
- [ ] Der Karte mit `/parkour setname <Name>` einen Namen geben
- [ ] Den Parkour in den Spielmodus setzen, mit `/parkour playmode`
- [ ] Einen Testlauf bestehen, laufe dafür über den Startblock.
- [ ] Sofern du einen Fehler im Testlauf bemerkst, kannst du jederzeit mit `/parkour buildmode` zurück.
- [ ] Wenn du den Testlauf abgeschlossen hast, kannst du die Karte mit `/parkour publish` veröffentlichen.

Du kannst diese Liste auch im Spiel mit dem Befehl `/parkour todo` ansehen.

!!! warning "Wichtig"
	Hast du eine Karte erst veröffentlicht, kannst du keine Änderungen mehr an der Karte vornehmen, auch der Name kann dann nicht mehr geändert werden.
	
