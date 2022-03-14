# Techniker Fertigkeit im Citybuild


## 1. Portale
Mit Portalen können sich die Nutzer von einem Punkt des Servers zu einem anderen teleportieren. Dabei spielt es keine Rolle, wo dieser Ort ist. Man muss an beiden Orten die Berechtigung haben, bauen zu können, ansonsten lässt sich das Portal nicht auf beiden Seiten (Eingang und Ausgang) erschaffen.

1. Erstellung von Portalen
    
    1. Zuerst sollte sichergestellt werden, dass das Ziel, an welchem das Portal erstellt werden soll, sicher ist. Der Ersteller des Portals kann haftbar gemacht werden, sollten Spieler bei der Nutzung eines Portals sterben. Sofern der sichere Ort durch z. B. eine Stadt oder einen anderen Schutz garantiert ist, kann man fortfahren.
    
    2. Mit dem Portalende lässt sich einfach beginnen. Es muss ein Schild mit dem folgenden Inhalt unter dem Boden, des Portalausgangs mit folgendem Inhalt auf den korrekten Zeilen erstellt werden:
    ```linenums="1"
    nichts
    [MC1113]
    Portalname
    nichts
    ```

    3. Der Portalname kann frei gewählt werden, sollte aber nicht zu lang sein. In dieses Schild muss nun ein Redstone Clock Signal geleitet werden, um das andere Portal regelmäßig über die eigene Existenz zu informieren. Sollte dies nicht möglich sein, kann bei `[MC1113]` ein `S` angehängt werden: `[MC1113]S`
    4. Jetzt kann der Portaleingang erstellt werden. Dieser funktioniert mit Redstone, folgender Aufbau hat sich bewährt:
    5. Druckplatte setzen
    6. 5 Blöcke unter die Druckplatte graben
    7. Genau 5 Blöcke unter der Druckplatte ein Schild an eine Wand setzen, mit folgendem Inhalt:
    ```linenums="1"
    nichts
    [MC1112]
    Portalname
    1,1,1=^0:5:0
    ```
    8. Sobald das Schild steht, muss Redstone von der Druckplatte genau auf das Schild zeigen.
    9. Damit das Portal zum ersten mal verknüpft werden kann, muss jeweils am Anfang und Ende jemand stehen. Danach kann man das Portal betreten, manchmal benötigt dies einige Versuche. Nachdem das Portal verknüpft wurde, ist dies nicht länger nötig. Alle Portale sind immer nur von Eingang zum Ausgang, man kann nicht in beide Richtungen teleportiert werden.
    10. Das Portal sollte nun gehen, wenn es Probleme geht, wende dich im Spiel an uns über ein [[Ticket]].

## 2. Homeportal
Mit Homeportalen können sich Spieler zum Home des Homeportal Erstellers teleportieren lassen.

1. Erstellung von Homeportalen
    1. Zuerst muss man mit `/sethome name` ein Home erstellen, dieses wird daraufhin mit einem Schild verlinkt.
    ```
    hometeleport
    homename
    Optional: private (Nur von dir verwendbar)
    nichts
    ```
    2. Spieler können nun auf das Schild klicken und werden zum Home teleportiert. Fallen sind nicht erlaubt.
    3. Spieler sollten nach Nutzung des Portals, jegliche Art von Schaden meiden, da man sonst zurück teleportiert wird. Dies dient zur Sicherheit vor Spielerfallen.
    4. Man kann auch Druckplatten über den Schildern platzieren (`Druckplatte->Zwischenblock->Teleportschild`) und Spieler werden daraufhin mit der Druckplatte teleportiert.
!!! warning "Beachte"
    Es ist nicht erlaubt, Fallen mit den Homeportalen zu bauen.


## 3. Sortiermaschine
Sortiermaschinen können viel Arbeit abnehmen, da diese auch große Mengen an verschiedensten Gegenständen aussortieren können. Diese Sortiermaschine basiert auf die Minecraft Namen.

!!! tip
    Die Minecraft Namen kann man entweder das Internet erfahren oder man verwendet ++f3+h++, um die Namen der Gegenstände direkt im Inventar anzuzeigen.

1. Erstellung von Sortiermaschinen
    1. Es werden Gleise benötigt, auf denen das Kistenminecart fahren kann.
    2. Zuerst platziert man sich Eisenerze an allen Stellen, wo sortiert werden soll, unter den Erzen wird Platz für ein Schild benötigt.
    3. Wenn ein lückenloser Kreis gebaut wurde, können nun Gleise verwendet werden, damit das Kistenminecart fahren kann.
    4. An jedem Eisenerz muss nun eine Kiste platziert werden, wenn die Eisenerze zu eng aneinander legen, können auch Redstonekisten verwendet werden.
    5. Nun kann man zuerst eine Eingangskiste festlegen, welche die Items in das Minecart befördert, bei dieser muss unter dem Eisenerz ein Schild mit folgendem Inhalt erstellt werden:
    ```linenums="1"
    nichts
    [Deposit]
    nichts
    nichts
    ```
    6. Daraufhin können unter allen Eisenerzen Schilder platziert, um die gewünschten Items zu sortieren, dies ist mit folgendem Inhalt möglich:

        === "Vorschau"
            ```linenums="1" hl_lines="3"
            nichts
            [Collect]
            Item Name
            nichts
            ```
        === "Beispiel"
            ```linenums="1" hl_lines="3"
            nichts
            [Collect]
            dirt
            nichts
            ```

    7. Sobald man fertig ist, sollte am Ende noch ein Eisenerz mit Kiste übrig bleiben oder zusätzlich erstellt werden, um restliche Items, die nicht aussortiert werden konnten, aus dem System zu bringen, dies passiert mit folgendem Schild:
    ```linenums="1"
    nichts
    [Collect]
    nichts
    nichts
    ```
    8. Wenn dies geschafft ist, kann das Minecart direkt gestartet werden, wichtig ist, dass das Kistenminecart von der Eingangskiste weg in Richtung der sortierten Kisten fährt, um zum Schluss die restlichen, nicht sortierbaren Items bei der letzten Sortierkiste auszuleeren.
!!! help "Hilfe"
    Gibt es Fragen zur Sortiermaschine? Gerne helfen wir dir über ein [[Ticket]] dabei, deine Sortiermaschine aufzubauen.

## 4. Saugmaschine

Anders als Trichter können Saugmaschinenen durch die starke Leistung weitreichender Gegenstände einsammeln, automatisch sortieren und auch direkt mit einem Röhrensystem verbunden werden. Hinweis: Fremde Items unerlaubt absaugen ist verboten.

!!! note "Information"
    Saugmaschinen können in vielen Fällen sehr praktisch sein, jedoch ist die Saugleistung auf einen Radius von maximal 10 Blöcken reduziert. Anstelle viele einzelne Saugmaschinen mit komplexen Systemen aufzustellen, kann man als Techniker auch die [Supersauger](#12-supersauger) nutzen, die einen gesamten Chunk absaugen können.


1. Erstellung von Saugmaschinen

    1. Zuerst muss man an dem Ort stehen, an dem Items aufgefangen werden sollen. Es wird ein Schild und Items für eine Clock benötigt, hier ist eine langsame Clock mit z. B. Trichtern wünschenswert, da die Saugmaschine sonst überhitzen kann.
    2. Möglichst nah an der Stelle, an der die Items aufgesammelt werden sollen, wird die Saugmaschine aufgestellt. Jetzt muss die Saugleistung in Form von Radius an Blöcken um die Saugmaschine überprüft werden, je mehr radius an Blöcken die Saugmaschine ansaugen muss, je schneller kann sie überhitzen.
    3. Jetzt platziert man die Saugmaschine mithilfe von einem Schild an einem Block, mit folgendem Inhalt:

        === "Vorschau"
            ```linenums="1"
            nichts
            [MC1214]
            radius (z. B. 3 Blöcke, maximal 10.)
            nichts (Optional: Name, welcher gesammelt werden soll oder -Name, welcher nicht gesammelt werden soll.)
            ```
        === "Nur Erde (Radius 5)"
            ```linenums="1"
            nichts
            [MC1214]
            5
            dirt
            ```
        === "Alles außer Erde (Radius 10)"
            ```linenums="1"
            nichts
            [MC1214]
            10
            -dirt
            ```
        === "Beispielbild"
            ![Saugmaschine](https://files.steempeak.com/file/steempeak/immanuel94/9QNDIwAb-saugmaschine.png){ align=right }

    4. Sobald die Saugmaschine platziert wurde, muss eine Kiste auf den Block gestellt werden, an dem das Schild hängt, daraufhin wird nun ein langsames Redstone Clock Signal benötigt, welches auf das Schild zeigt.
    5. Möchte man optional die Saugmaschine mit einer Röhre verbinden, erstellt man eine Röhre direkt an der Kiste eine Röhre, die Kiste der Saugmaschine entspricht der Kiste, die von der Röhre verwendet wird, es muss ein Schalter hinter dem Block mit dem Saugmaschinen Schild gesetzt werden, der die Röhre automatisch startet, sobald etwas aufgesammelt wurde.
    6. Sollte etwas nicht richtig funktionieren, helfen wir dir gerne über ein [[Ticket]] weiter.

## 5. Craftingmaschine
Gerade bei großen Mengen an Gegenständen, die umständlich zu craften sind, ist die Craftingmaschine eine große Hilfe.

1. Erstellung von Craftingmaschinen
    1. Es wird ein Dropper, eine Kiste sowie ein Trichter benötigt.
    2. Zuerst platziert man die Kiste, in die die fertigen Gegenstände geworfen werden sollen.
    3. Daraufhin platziert man den Werfer so, dass dieser in die Kiste zeigt, damit diese die Gegenstände direkt dort hinein legt.
    4. Nun wird ein Block unter dem Werfer platziert und auf diesem Block ein Schild mit folgendem Inhalt erstellt:
    ```linenums="1"
    nichts
    [MC1219]
    nichts
    nichts
    ```
    5. Wenn das Schild korrekt platziert wurde, kann im Werfer ein Rezept wie in der Werkbank (Workbench) platziert werden. Sofern mehr als 1 Item in jedem für das Rezept verwendeten Slot liegt, wird bei einem Redstone Signal ein Gegenstand gecraftet.
    6. Zuletzt wird eine Clock erstellt, deren Signal mit einem Redstone direkt auf das Schild zeigt, diese kann variabel schnell laufen, jenachdem, wie viele Items in den Werfer kommen. Der Werfer kann mit einem Trichter befüllt werden.
    7. Gibt es Fragen zur Funktion? Wir helfen wir über ein [[Ticket]].

## 6. Versteckter Schalter
Mit dem Verstecken Schalter kann man durch Rechtsklick auf einen Block ein Redstonesignal ausgeben und somit z.B. Eine Tür oder ein Tor(Gate) öffnen lassen.

1. Erstellung von Versteckten Schaltern
    1. Schild mit folgendem Inhalt hinter den Block stellen:
    ```linenums="1"
    nichts
    [X]
    nichts (Optional der Rang name z.B spender, admin….)
    nichts
    ```
    2. Hinter auf der anderen Seite des Blocks kann ein Schalter oder Knopf platziert werden, sobald jemand den Block nun Rechtsklickt, wird der Schalter für eine Sekunde ausgelöst.
    3. Fragen dazu, wir helfen gerne über ein [[Ticket]].

## 7. Gates
Mit Gates können Tore aus Glas und Zäunen erstellt werden, dank Redstonekompatiblität sind diese auch einfach zu verbauen.

1. Erstellung von Gates
    1. Ein Gate aus Glas oder Zäunen aufstellen, es funktionieren nur normale Glasscheiben.
    2. Ein Schild mit folgendem Inhalt an der Wand neben dem Gate (oder unter dem Boden, daneben) aufstellen:
    ```linenums="1"
    nichts
    [Gate]
    nichts
    nichts
    ```
    3. Nun sollte sich das Gate umschalten lassen, es ist zu Redstone kompatibel und schaltet um, sofern Redstone direkt darauf zeigt.
    4. Fragen dazu? Wir helfen dir gerne über ein [[Ticket]] weiter.
    5. Falls das Gate nicht erkannt wird, klicke mit dem gleichen Block, mit dem das Gate funktionieren soll, auf das Gate Schild, bis der Name des Items auf dem Gate Schild angezeigt wird und versuche es erneut. Nun sollte das Gate erkannt werden.
    !!! note "Verwendbare Blöcke"
        minecraft:acacia_fence, minecraft:birch_fence, minecraft:jungle_fence, minecraft:oak_fence, minecraft:spruce_fence, minecraft:dark_oak_fence, minecraft:nether_brick_fence, minecraft:iron_bars, minecraft:glass_pane

## 8. Brücken
Mit Brücken lassen sich Burgen und andere Sicherheitseinrichtungen vor ungewollten Feinden sichern.

1. Erstellung von Brücken
    1. Bauen einer Bücke (3 breit)
    2. Am Ende der Brücke jeweils ein Schild mit dem entweder direkt auf der Brücke oder darunter mit folgendem Inhalt aufstellen:

        === "Vorschau"
            ```linenums="1"
            nichts
            [Bridge]
            nichts
            nichts
            ```
        === "Beispielbild"
            ![Brücke](https://cdn.steemitimages.com/DQmeofKbGBAnCmGySubQNzTgQyw6Xxcq8VS9wUSjDXCWxPV/bridge.png){ align=right }

    3. Die Brücke ist auch durch ein direktes Redstonesignal umstellbar.
    4. Bei Fragen zum Brückenbau helfen wir gerne im Spiel über ein [[Ticket]] weiter.
    5. Blöcke die benutzt werden können:
    !!! note "Verwendbare Blöcke"
        acacia_planks, acacia_slab, birch_planks, birch_slab, brick_slab, cobblestone, cobblestone_slab, dark_oak_planks, dark_oak_slab, dark_prismarine_slab, glass, jungle_planks, jungle_slab, nether_brick_slab, oak_planks, oak_slab, petrified_oak_slab, prismarine_brick_slab, prismarine_slab, purpur_slab, quartz_slab, red_sandstone_slab, sandstone_slab, spruce_planks, spruce_slab, stone_brick_slab, stone_slab

## 9. Röhren
Röhren helfen dabei, Gegenstände über weite Wege schnell zu transportieren. Dank der effizienten Transportmethode sind Röhren die schnellste Methode auf dem Server, Gegenstände zu transportieren.

1. Erstellung von Röhren
    1. Zuerst wird eine Kiste dort platziert, wo die Items abtransportiert werden, dahinter wird ein klebriger Kolben platziert, welcher auf die Kiste zeigt.
    2. Auf dem klebrigen Kolben wird ein Schild mit dem folgenden Inhalt platziert:
    ```linenums="1"
    nichts
    [Pipe]
    nichts
    nichts
    ```
    3. Daraufhin kann man mit Glas die Röhre bauen, am anderen Ende der Röhre muss ein normaler Kolben in eine Kiste oder ein anderer Block mit Inventar zeigen. Es ist allerdings möglich mehrere Kolben an die Röhre an zu schließen und somit z.B. ein Lagersystem zu bauen, da man über den Kolben Schilder mit einer Whitelist oder einer Blacklist von Items erstellen kann oder man füllt die Angeschlossene Kiste mit nur einem Item komplett, so sieht die Pipe, dass nur dieses Item in diese Kiste kommen kann. Dies ist jedoch nicht notwendig:
    ```linenums="1"
    nichts
    [Pipe]
    nichts (oder Items die hier reinkommen sollen „Whitelist“)
    nichts (oder Items, die hier nicht reinkommen sollen „Blacklist“)
    ```
    4. Jede Farbe von Glas kann benutzt werden. So ist es möglich mehrere Pipes direkt nebeneinander zu legen, da die Items nur durch die selbe Farbe transportiert werden.
    5. Nun ist die Röhre fertig, sobald Redstone direkt auf das Schild an dem Klebrigen Kolben trifft, wird jeweils ein Stack von Gegenständen befördert, Clocks sind möglich, bestenfalls allerdings mit Comparator zum prüfen, ob die Röhre überhaupt etwas transportieren muss.
    6. Fertig, bei Fragen zum Bau von Röhren können wir im Spiel oder über ein [[Ticket]] gerne helfen.

## 10. Bezahlsystem
Mit Bezahlsystemen kann man anderen Spielern die Möglichkeit geben, für ein Redstonesignal zu bezahlen.

1. Erstellung von Bezahlsystemen
    1. Schild mit folgendem Inhalt an eine Wand stellen:
    ```linenums="1"
    nichts
    [Pay]
    Talermenge
    nichts
    ```
    2. Hinter auf der anderen Seite des Blocks kann ein Schalter platziert werden, sobald jemand etwas über das Bezahlsystem kauft, wird der Schalter für eine Sekunde ausgelöst.
    3. Fragen dazu? Wir helfen dir auch über ein [[Ticket]].


## 11. Clock
Mit der Clock können Aktionen in einem definierten Zeitintervall ausgelöst werden.

1. Erstellung von Clocks
    1. Schild mit folgendem Inhalt an eine Wand stellen:
    ```linenums="1"
    nichts
    [MC1421]
    Zeitintervall in Ticks
    nichts
    ```
    2. Hinter auf der anderen Seite des Blocks muss ein Schalter platziert werden, sobald die Zeit vergangen ist, wird dieser automatisch kurz umgelegt.
    3. Fragen dazu? Wir helfen auch über ein [[Ticket]] direkt.

## 12. Supersauger
Mit dem Supersauger werden alle Items, die in dem Chunk des Supersaugers platziert werden, zum Supersauger teleportiert oder in eine Kiste über dem Supersauger gesaugt. Während der Supersauger sehr teuer herzustellen ist, so erlaubt er sehr effiziente Farmmethoden durch die starke Saugkraft.

1. Erstellen und platzieren von Supersaugern
    1. Supersauger können mit einem Crafting Rezept hergestellt werden:
    ![Crafting Rezept für Supersauger](assets/images/crafting_supersauger.png)
    2. Um einen Supersauger zu platzieren, muss man ein Techniker sein und den Supersauger innerhalb einer Stadt platzieren.
	3. Jetzt saugt der Supersauger alle Items aus dem Chunk an, in welchem er platziert wurde.
	4. Wenn man die Items lieber in einer Kiste haben will, kann man über dem Supersauger auch eine Kiste platzieren und diese mit einer [Röhre](#9-rohren) verbinden, um die Items effizient zu transportieren.

    !!! note "Wichtig"
        Bevor ein Chunk mit einem Supersauger von einer Stadt entfernt wird, sollte der Supersauger aus Sicherheitsgründen abgebaut werden, damit dieser nicht versehentlich zerstört wird.

