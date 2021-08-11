

!!! info inline end ""
    ![Altenburg](https://files.steempeak.com/file/steempeak/skyroad-wiki/bRVgahRK-altenburg.png)
    Der Stadtspawn der Stadt Altenburg im Creative.
   
Spieler auf Skyroad können im Survival und Freebuild eigene Städte erstellen. Städte erlauben eine Sicherung vor Griefern und Plünderern, die es auf wertvolle Blöcke abgesehen haben.
Mit der Stadterstellung kommen auch Kosten einher, daher sollte man sich gut überlegen, ob man wirklich dafür bereit ist, eine Stadt zu erstellen und nicht doch lieber einer Stadt beizutreten.
Neben einer Sicherung für sich selbst, können Städte in vermietbare Grundstücke eingeteilt werden, die von der Stadt auf Wunsch besteuert werden können. Dies gibt dem Stadtbetreiber eine Einnahmequelle.


## 1. Einer Stadt beitreten
1. Zuerst empfiehlt sich ein erster Blick in die Stadtliste, diese kann mit dem Befehl `/town list` geöffnet werden.
2. Städte, die mit **[Open]** oder **[Offen]** gekennzeichnet sind, können direkt betreten werden und benötigen keine Einladung des Bürgermeisters oder eines Assistenten.
3. Um die Suche einfacher zu machen und sicher zu gehen, dass einem die Stadt gefällt, kann man diese zuvor mit `/town spawn Stadtname` besuchen. Das erlaubt einem, das Aussehen der Stadt einzuschätzen und ob man dort einziehen möchte.
4. Hat man eine Stadt gefunden, die als **[Open]** oder **[Offen]** gekennzeichnet ist, kann man dieser Stadt mit dem Befehl `/town join Stadtname` beitreten.
5. Sollte man in eine nicht öffentliche Stadt beitreten wollen, ist es notwendig, sich direkt an den Bürgermeister der Stadt zu wenden, den Namen erfährt man über den Befehl `/town Stadtname`. Auch Assistenten können Spieler einladen.
6. Sobald man der Stadt beigetreten ist, kann man sich kostenfrei jederzeit mit `/town spawn` zum Spawnpunkt der Stadt teleportieren.
7. Am Spawnpunkt der Stadt angekommen, kann man nun ein passendes und freies Grundstück suchen. Freie Grundstücke sind entweder für neue Spieler markiert oder dadurch erkennbar, dass im Chat **For Sale** oder **Zum verkauf** steht, wenn man Freie Grundstücke findet man über den `/plots` Befehl, klicke dort auf **Freie Grundstücke**, um alle freien Grundstücke der Stadt zu sehen.
8. Hat man ein schönes Grundstück gefunden, welches man kaufen möchte, kann man dieses mit dem Befehl `/plot claim` kaufen. Damit das funktioniert, muss man während man den Befehl eingibt, auf dem Grundstück stehen.

!!! note "Beachte"
    Die Mitgliedschaft und der Besitz von Grundstücken ist in den meisten Fällen mit Kosten verbunden. Schaue daher immer mit `/money` auf dein Konto und überwache die Kosten mit `/res tax`, um immer genug auf dem Konto zu haben.

---

## 2. Selbst eine eigene Stadt erstellen
#### 2.1 Erste Schritte

![Wildnis](https://files.steempeak.com/file/steempeak/skyroad-wiki/OeCul5ze-freiesland.png)

!!! tip
    Ein optimaler Ort ist eine weitesgehend unbearbeitete Landschaft, bei der es keinen Spieler oder eine Stadt gibt, die das Land für sich beanspruchen.


1. Bevor man eine Stadt erstellt, sollte man zuerst einen optimalen Ort finden, an dem man die Stadt erstellen möchte. Ein späteres versetzen an einen weiter entfernten Ort kommt mit weiteren Kosten und ist daher nicht zu empfehlen.
2. Erstelle die Stadt mithilfe des Befehls `/town new Stadtname`, der Stadtname lässt sich später ändern.
3. Städte, die kein Geld mehr auf ihrem Konto haben, werden bankrott gehen und am nächsten Tag automatisch gelöscht, achte daher darauf, dass die Stadt die Stadtsteuer von 50 {{ servervars.currencyname }} pro Tag bezahlen kann. Mit `/town` sieht man, wieviel {{ servervars.currencyname }} auf dem Stadtkonto sind. Bestenfalls zahlst du direkt zum Anfang etwas mithilfe von `/town deposit 500` ein, in diesem Fall 500 {{ servervars.currencyname }}, was für 5 Tage im Survival ausreichend wäre.
4. Nun werden weitere Chunks geclaimt, dies kann entweder Chunk für Chunk, mithilfe von `/town claim` erfolgen, oder auch einfach mit Radius <Angabe>, wieviele Chunks im Umkreis von einem geclaimt werden sollen, z. B. `/town claim 2`. Beachte, dass durch das claimen von Grundstücken weitere Kosten entstehen, die von dem Konto deiner Stadt abgezogen werden.
5. Nachdem man die Stadt erweitert hat, muss diese für andere Spieler konfiguriert werden, sofern dies gewünscht ist, ansonsten ist die Stadt hier fertig. Falls man nur mit engen Freunden zusammen spielt, kann man diese nun mit `/t add Spielername` einladen.
----
  
#### 2.2 Berechtigungen einstellen und Stadt öffentlich machen
1. Damit nur der Bürgermeister überall in der Stadt abbauen kann, sollten die Rechte allgemein entfernt werden, dies ist mit `/town set perm reset` und `/town set perm off` sehr einfach.
<div class="pull-right"><a href="https://files.steempeak.com/file/steempeak/skyroad-wiki/D29Ri5kl-townsetting.png"><img src="https://files.steempeak.com/file/steempeak/skyroad-wiki/D29Ri5kl-townsetting.png"/></a></div>
2. Jetzt sollten bei `/town` unter **Permissions** oder **Rechte** alle Einstellungen auf `---` stehen. Siehe Bild.
3. Da die Stadt nun sicher ist, kann sie für andere Spieler geöffnet werden, gib dafür `/town toggle open` ein. Sofern im Chat steht "Inviteless joining is now Enabled", ist die Stadt nun offen. Die Warnung kann ignoriert werden, da bereits alle Maßnahmen zur Sicherung der Stadt vorgenommen wurden, falls etwas anderes im Chat steht, kann es sein, dass die Meldung auf Deutsch ausgegeben wurde. Um zu überprüfen, ob die Stadt wirklich für jeden zugänglich ist, kann man mit `/t list` seine Stadt suchen, diese sollte mit **[Open]** oder **[Offen]** gekennzeichnet sein. Sollte dies nicht der Fall sein, gib einfach erneut `/town toggle open` ein und versuche es erneut. Spieler können nun mit `/town join Stadtname` beitreten.
4. Sofern die Berechtigungen in den letzten drei Schritten entfernt wurden, ist es Einwohnern deiner Stadt ist es nicht möglich, zu bauen oder abzubauen, daher sollten folgend sogenannte **Plots / Grundstücke** eingerichtet werden. Diese sind immer einen Chunk groß, welcher immer genau 16x16 Blöcke groß ist. Mit der Tastenkombination **F3** und gleichzeitig **G** kann man die Chunks sehen, mit gleicher Kombination lässt sich die Ansicht auch wieder abschalten.
---
  
#### 2.3 Plots / Grundstücke einrichten
1. Als Bürgermeister kann man sich nun Orte suchen, an denen man selbst nichts bauen, aber gerne anderen ein Grundstück anbieten möchte. Es ist wichtig, vorher darüber nachzudenken, denn deine Bewohner werden sich nicht über eine spätere Umsiedlung freuen. Plane im vorraus und sei dir sicher, dass du diesen Platz später nicht benötigst.
2. Wenn man einen geeigneten Chunk als **Plot / Grundstück** innerhalb der Stadt an andere Spieler verkaufen will, stellt man sich auf den Chunk und gibt `/plot fs 50` ein, sofern man diesen Chunk als Grundstück für 50 {{ servervars.currencyname }} verkaufen will, dieser Preis kann frei bestimmt werden. Diesen Prozess kann man mit allen Chunks wiederholen, die man gerne verkaufen möchte. **Achte auf mögliche Zuwege zu den Grundstücken**, die bestenfalls nicht auf dem Grund der Spielergrundstücke stehen, um Griefing an den Wegen zu vermeiden. Jenachdem, wie wichtig einem die Privatsphäre von den Einwohnern ist, kann man die **Plots / Grundstücke** entweder sehr nah beieinander platzieren oder auch weiter auseinander. **Spieler können das Grundstück kaufen**, indem sie `/plot claim` eingeben, dafür muss der Spieler auf dem Grundstück stehen. Mit einem Schild kann man die Einwohner darüber informieren.
---
  
#### 2.4 Plots / Grundstücke benennen und kategorisieren
1. Alle Chunks innerhalb der Stadt können verschieden benannt und kategorisiert werden, so kann man mit `/plot set name` dem Chunk einen Namen geben, z. B. kann man Wege als Weg benennen. **Chunks von Spielern müssen nicht benannt werden**, wenn diese nicht benannt wurden, **benennen diese sich automatisch nach dem Spieler**, der das Grundstück kauft.
2. Wenn man den Chunk kategorisieren möchte, lässt sich dies mit `/plot set kategorie`, `kategorie` ist dabei mit dem Kategorienamen zu ersetzen. Jede Grundstückskategorie kann auch mit besonderen Steuersätzen besteuert werden. Aktuell gibt es:
  1. `/plot set shop`, welches das Grundstück als Laden (Shop) klassifiziert.
  2. `/plot set embassy` setzt das Grundstück zu einer Botschaft, diese erlaubt jedem Spieler (auch Stadtfremde), dieses Grundstück zu kaufen.
  3. `/plot set arena` macht dem Spieler klar, dass es hier um PvP geht und man nicht ohne weiteres betreten sollte.
  4. `/plot set jail` ist der Gefängnisbereich für Spieler, die sich in der Stadt nicht korrekt verhalten haben.
  5. `/plot set farm` erlaubt es deinen Einwohnern, in bestimmten Bereichen Farmblöcke abzubauen.
3. Es ist auch jederzeit möglich, die Kategorie wieder zurückzusetzen, mithilfe von `/plot set reset`. Ache immer darauf, auf dem Chunk zu stehen, der bearbeitet werden soll.
---
  
#### 2.5 Finanzierung der Stadt
1. Sofern man es bis hier geschafft hat, ist es auch notwendig, darüber nachzudenken, wie sich die Stadt finanziert.
    1. Es gibt die Möglichkeit, entweder Stadtsteuern zu verlangen, bei denen jeder Einwohner täglich einen bestimmten, von dir festgelegten Betrag an {{ servervars.currencyname }} bezahlen muss, sollte ein Einwohner diesen nicht bezahlen können, wird dieser aus der Stadt geworfen. Diese Möglichkeit ist mit `/town set taxes 5` nutzbar, in dem Beispiel würde jeder Spieler 5 {{ servervars.currencyname }} pro Tag an Stadtsteuer bezahlen. Optional kann man auch eine prozentuale Menge des Spielerkontos abbuchen, dafür gibt man `/town toggle taxpercent` ein, damit werden täglich 5% vom Konto des Spielers an die Stadt überwiesen.
    2. Alternative Möglichkeiten sind z. B., die Stadt an sich kostenlos anzubieten, dafür aber eine Grundstückssteuer zu erheben, die pro Grundstück fällig wird, hier ist auch eine Aufteilung in normale Grundstücke, Botschaften und Shops möglich.
        1. `/town set plottax 2` setzt die allgemeine Grundstücksteuer auf 2.
        2. `/town set shoptax 5` legt die Steuer für Läden (Shops) auf 5.
        3. `/town set embassytax 5` stellt die Steuer für Botschaften auf 5.
---

!!! done "Erledigt"
    **Gratulation**. Du hast es geschafft, deine Stadt sicher einzurichten und auszubauen. Doch es gibt noch mehr! Schau dir die Liste an Befehlen an, es ist möglich für jedes Grundstück jeweils PvP, Monster, Feuer, Explosionen ein- und auszuschalten, sowie Außenposten zu erstellen.
    
    Auch der Beitritt in einer Nation oder sogar die Erschaffung eines eigenen Königreiches mit vielen Städten steht dir offen. Sollte es Fragen dazu geben, helfen wir gerne im Spiel über ein [[Ticket]] weiter.



---
  
## 3. In eine Nation beitreten
1. Um in eine Nation beizutreten, benötigt man den Kontakt zur Königin oder zum König der jeweiligen Nation. Nur diese können deine Stadt zu ihrer Nation hinzufügen. Städte innerhalb der Nation genießen besonders günstige Teleportationskosten für Stadtteleportation. Nationen können auch den Zugriff auf Farmen mit anderen Nationsmitgliedern teilen.
2. Die Königin oder der König muss die Stadt mit dem Befehl `/nation add Stadtname` einladen.
3. Der Bürgermeister der Stadt muss die Anfrage mit `/accept` annehmen, um der Nation beizutreten.
Achte regelmäßig auf die Steuern der Nation, manche Nationen verlangen überzogene Steuern, die deiner Stadt schaden könnnen.
---
  
## 4. Die Erstellung einer eigenen Nation
1. Erstelle eine Nation mit dem Befehl `/nation new Nationsname`, der Name der Nation kann später geändert werden.
2. Lade Städte in deine Nation ein, mit `/nation add Stadtname`.
3. Setze Steuern mit `/nation set taxes 10` für deine Nation fest, die von den Städten bezahlt werden müssen, in diesem Fall 10 {{ servervars.currencyname }} pro Tag. Können Städte deine Steuer nicht bezahlen, werden diese automatisch aus deiner Nation austreten.
4. Wenn deine Nation eine neutrale Position im Fall eines Krieges sein soll, muss die Nation als Neutral festgelegt werden, dies kostet innerhalb der Kriegszeit 100 {{ servervars.currencyname }} am Tag und ist mit `/nation toggle neutral` möglich.

## 5. Alle Befehle und deren Zweck
Hier sind alle Befehle für Städte und Nationen aufgelistet.[^1]

!!! tip
    Verwende die im Browser eingebaute Suchfunktion um nach dem von dir benötigten Befehl zu suchen. 
    
    Mit ++ctrl+f++ (**STRG + F**) kann diese Suchfunktion in den meisten Internetbrowsern geöffnet werden.

| Befehl | Beispiel | Erklärung |
| :-- | :--- | :--- |
|`/plots` | | Zeigt alle Plots an, die dir gehören. |
|`/towny ?` | | Zeigt weitere Towny Befehle.|
|`/towny map` | | Zeigt eine minimalistische Karte mit Grundstücken.|
|`/towny prices` | | Zeigt die Kosten für die Stadt.|
|`/towny time` | | Zeigt die Zeit, bis die nächste Steuer fällig wird.|
|`/towny top residents <all/town/nation>` | `/towny top residents all` | Zeigt die besten Bewohner an.|
|`/towny top land <all/town/nation>` | `/towny top land all` | Zeigt die besten Landbesitzer an.|
|`/plot claim` | | Kauft das Land, auf dem man gerade steht, sofern es zum verkauf steht.|
|`/plot unclaim` | | Gibt das Land, auf dem man gerade steht wieder ab.|
|`/plot <forsale/fs> <Preis>` | `/plot fs 5` | Stellt das Land, auf dem man steht zum verkauf.|
|`/plot <notforsale/nfs>` | `/plot nfs` | Entfernt das Verkaufsangebot für dieses Land.|
|`/plot evict` | | Wirft den Spieler von seinem Grundstück.|
|`/plot perm` | | Zeigt die Berechtigungen für das Grundstück, auf dem man gerade steht.|
|`/plot perm hud` | | Öffnet eine praktische Sidebar, die die Berechtigungen für das Grundstück anzeigt und aktualisiert.|
|`/plot set reset` | | Setzt die Grundstückskategorie zu einem normalen Grundstück zurück.|
|`/plot set shop ` | | Setzt die Grundstückskategorie zu einem Shop.|
|`/plot set embassy` | | Setzt die Grundstückskategorie zu einer Botschaft.|
|`/plot set arena` | | Setzt die Grundstückskategorie zu einer Arena.|
|`/plot set wilds` | | Setzt die Grundstückskategorie zu einem Wildnis Bereich.|
|`/plot set inn` | | Setzt die Grundstückskategorie zu einem Erholungsgebiet.|
|`/plot set jail` | | Setzt die Grundstückskategorie zu einem Gefängnis.|
|`/plot set farm` | | Setzt die Grundstückskategorie zu einer Farm.|
|`/plot set bank` | | Setzt die Grundstückskategorie zu einer Bank.|
|`/plot set name <text>` | `/plot set name Hallo` | Setzt den Namen des Grundstücks zum angegebenen Namen.|
|`/plot set perm <on/off>` | `/plot set perm off` | Setzt alle Berechtigungen des Grundstücks auf an oder aus.|
|`/plot set perm <resident/ally/outsider> <on/off>` | `/plot set perm outsider off` | Setzt alle Berechtigungen des Grundstücks für Stadtbewohner, Verbündete oder Außenseiter auf an oder aus.|
|`/plot set perm <build/destroy/switch/itemuse> <on/off>` | `/plot set perm itemuse off` | Setzt alle Berechtigungen des Grundstücks für bestimmte Aktionen, wie bauen, abbauen, umstellen oder Items verwenden an oder aus.|
|`/plot set perm <resident/ally/outsider> <build/destroy/switch/itemuse> <on/off>` | `/plot set perm outsider itemuse off` | Setzt bestimmte Berechtigungen des Grundstücks für bestimmte Aktionen, wie bauen, abbauen, umstellen oder Items verwenden für bestimmte Gruppen wie Stadtbewohner, Verbündete oder Außenseiter an oder aus.|
|`/plot set perm reset` | | Stellt die Standardeinstellungen für Berechtigungen für dieses Grundstück wieder her.|
|`/plot toggle fire` | | Schaltet die Feuerverteilung an oder aus.|
|`/plot toggle pvp` | | Schaltet Spieler gegen Spieler an oder aus.|
|`/plot toggle explosion` | | Schaltet Explosionen an oder aus.|
|`/plot toggle mob` | | Schaltet Mobsppawning an oder aus.|
|`/plot clear` | | Entfernt einige Blöcke vom Grundstück.|
||||
|`/res ?` | | Zeigt verfügbare Befehle für den Bewohner Befehl an.|
|`/res` | | Zeigt Informationen über sich selbst.|
|`/res <Spielername>` | `/res Immanuel94` | Zeigt Informationen über den Spieler.|
|`/res friend add <Spielername>` | `/res friend add Immanuel94` | Fügt den Spieler (online) als Freund hinzu.|
|`/res friend add+ <Spielername>` | `/res friend add+ Immanuel94` | Fügt den Spieler (offline) als Freund hinzu.|
|`/res friend remove <Spielername>` | `/res friend remove Immanuel94` | Entfernt den Spieler (offline) von der Freundesliste.|
|`/res friend remove+ <Spielername>` | `/res friend remove+ Immanuel94` | Entfernt den Spieler (offline) von der Freundesliste.|
|`/res friend clearlist` | | Entfernt alle von der Freundesliste.|
|`/res list` | | Zeigt alle Spieler, die gerade innerhalb der Stadt online sind.|
|`/res jail paybail` | | Bezahlt die Kaution, wenn man gerade im Gefängnis ist.|
|`/res spawn` | | Teleportiert den Spieler zu seinem Bett, wenn innerhalb einer Stadt.|
|`/res toggle map` | | Sendet die `/towny map` jedes mal, wenn man einen neuen Chunk betretet.|
|`/res toggle townclaim` | | Claimt automatisch neue Chunks für die Stadt.|
|`/res toggle plotborder` | | Zeigt Rauchschwaden an, die das Grundstück markieren, wenn man einen neuen Chunk betretet.|
|`/res toggle constantplotborder ` | | Zeigt dauerhaft Rauchschwaden an, die das Grundstück markieren.|
|`/res toggle ignoreplots` | | Zeigt keine Grundstücksnamen in der Stadt an.|
|`/res toggle reset` | | Setzt alle Einstellungen zurück.|
|`/res set perm <on/off>` | `/plot set perm off` | Setzt alle Berechtigungen der Spielergrundstücke auf an oder aus.|
|`/res set perm <friend/ally/outsider> <on/off>` | `/plot set perm outsider off` | Setzt alle Berechtigungen der Spielergrundstücke für Freunde, Verbündete oder Außenseiter auf an oder aus.|
|`/res set perm <build/destroy/switch/itemuse> <on/off>` | `/plot set perm itemuse off` | Setzt alle Berechtigungen der Spielergrundstücke für bestimmte Aktionen, wie bauen, abbauen, umstellen oder Items verwenden an oder aus.|
|`/res set perm <friend/ally/outsider> <build/destroy/switch/itemuse> <on/off>` | `/plot set perm outsider itemuse off` | Setzt bestimmte Berechtigungen der Spielergrundstücke für bestimmte Aktionen, wie bauen, abbauen, umstellen oder Items verwenden für bestimmte Gruppen wie Freunde, Verbündete oder Außenseiter an oder aus.|
|`/res set perm reset` | | Stellt die Standardeinstellungen für Berechtigungen für Spielergrundstücke wieder her.|
|`/res tax` | | Zeigt die tägliche Steuer des Spielers an.|
||||
|`/town ?` | | Zeigt die verfügbaren `/town` Befehle an.|
|`/town` | | Zeigt Informationen über die aktuelle Stadt.|
|`/town <Stadtname>` | `/town Lobby` | Zeigt Informationen über die Stadt Lobby.|
|`/town here` | | Zeigt Informationen über die Stadt, in der man gerade steht.|
|`/town leave` | | Mit diesem Befehl kann ein Spieler eine Stadt verlassen.|
|`/town list <Seitennummer>` | `/town list 1` | Zeigt eine Liste aller Städte an.|
|`/town online` | | Zeigt eine Liste aller Spielker, die gerade in der Stadt online sind.|
|`/town plots <Stadtname>` | `/town plots Lobby` | Zeigt eine Liste aller Grundstücke, deren Typen und die Einnahmen der Stadt.|
|`/town new <Stadtname>` | `/town new Lobby` | Erstellt eine neue Stadt mit dem angegebenen Stadtnamen am aktuellen Standort des Spielers.|
|`/town add <Spielername>` | `/town add Immanuel94` | Fügt den angegebenen Spieler zur Stadt hinzu.|
|`/town kick <Spielername>` | `/town kick Immanuel94` | Kickt den angegebenen Spieler aus der Stadt.|
|`/town spawn` | | Teleportiert den Spieler zum Spawn der eigenen Stadt.|
|`/town spawn <Stadtname>` | `/town spawn Lobby` | Teleportiert den Spieler zum Spawn der angegebenen Stadt.|
|`/town claim` | | Claimt das Land für die eigene Stadt.|
|`/town claim outpost <name>`| `/town claim outpost Farm`| Claimt das Land für die eigene Stadt an einem Ort weiter weg von der Stadt.|
|`/town unclaim`|| Entfernt das Land von der Stadt und macht es wieder zur Wildnis.|
|`/town unclaim all`|| Entfernt das gesamte Land von der Stadt und macht es wieder zur Wildnis.|
|`/town withdraw <menge>`|| Hebt die angegebene Menge vom Stadtkonto ab.|
|`/town deposit <menge>`|| Legt die angegebene Menge auf dem Stadtkonto an.|
|`/bonuschunk <Stadt>`|| Kauft einen Bonuschunk für 1 EP.|
|`/town delete`|| Löscht die eigene Stadt.|
|`/town outlawlist <Stadtname>`|| Zeigt die verbannten Spieler aus der angegebenen Stadt.|
|`/town outlaw add <Spielername>`|| Verbannt den angegebenen Spieler aus der Stadt.|
|`/town outlaw remove <Spielername>`|| Entbannt den angegebenen Spieler in der Stadt.|
|`/town outpost <Außenposten Nummer>`|| Teleportiert den Spieler zur Außenposten Nummer.|
|`/town outpost list`|| Zeigt eine Liste aller Außenposten der Stadt an.|
|`/town ranklist`|| Zeigt eine Liste aller Bewohner und derer Ränge an.|
|`/town rank <add/remove> <Spielername> <Rangname>`|`/town rank add Immanuel94 assistant`| Gibt einem Spieler einen bestimmten Rang oder entfernt diesen wieder.|
|`/town reslist <Stadtname>`|| Zeigt alle Stadtmitglieder einer Stadt an.|
|`/town say <Nachricht>`|| Schreibt eine Nachricht an alle Stadtmitglieder, die gerade online sind.|
|`/town set board <Nachricht>`|| Schreibt eine Nachricht, die allen Stadtmitgliedern beim beitreten angezeigt wird.|
|`/town set mayor <Spielername>`|| Überträgt den Bürgermeister Rang an ein anderes Stadtmitglied.|
|`/town set homeblock`|| Versetzt den Hauptblock der Stadt auf den aktuellen Standort des Spielers.|
|`/town set spawn`|| Versetzt den Spawn der Stadt auf den aktuellen Standort des Spielers, muss bei homeblock liegen.|
|`/town set spawncost <Menge>`|| Stellt die Kosten für Nicht-Stadtmitglieder ein, die die Stadt mit dem `/town spawn` Befehl besuchen wollen.|
|`/town set name <Stadtname>`|| Ändert den Stadtnamen zum angegebenen Namen.|
|`/town set outpost`|| Ändert den Spawnpunkt des Außenpostens, an dem sich der Spieler gerade befindet.|
|`/town set jail`|| Ändert den Spawnpunkt des Gefängnisses, an dem sich der Spieler gerade befindet.|
|`/town set perm <on/off>` | `/plot set perm off` | Setzt alle Berechtigungen des Grundstücks auf an oder aus.|
|`/town set perm <resident/ally/outsider> <on/off>` | `/plot set perm outsider off` | Setzt alle Berechtigungen der Stadt für Stadtbewohner, Verbündete oder Außenseiter auf an oder aus.|
|`/town set perm <build/destroy/switch/itemuse> <on/off>` | `/plot set perm itemuse off` | Setzt alle Berechtigungen der Stadt für bestimmte Aktionen, wie bauen, abbauen, umstellen oder Items verwenden an oder aus.|
|`/town set perm <resident/ally/outsider> <build/destroy/switch/itemuse> <on/off>` | `/plot set perm outsider itemuse off` | Setzt bestimmte Berechtigungen der Stadt für bestimmte Aktionen, wie bauen, abbauen, umstellen oder Items verwenden für bestimmte Gruppen wie Stadtbewohner, Verbündete oder Außenseiter an oder aus.|
|`/town set perm reset` | | Stellt die Standardeinstellungen für Berechtigungen für die Stadt wieder her.|
|`/town set tag <Text>` | | Setzt ein Abkürzung für die Stadt, maximal 4 Zeichen.|
|`/town set tag reset` | | Löscht die Abkürzung der Strrradt wieder.|
|`/town set taxes <Menge>` | | Setzt die tägliche Steuer für die Stadtmitgliedschaft fest.|
|`/town set plottax <Menge>` | | Setzt die tägliche Steuer für Grundstücke fest.|
|`/town set shoptax <Menge>` | | Setzt die tägliche Steuer für Ladengrundstücke fest.|
|`/town set embassytax <Menge>` | | Setzt die tägliche Steuer für Botschaftsgrundstücke fest.|
|`/town set plotprice <Menge>` | | Setzt den Standardpreis für Grundstücke fest.|
|`/town set shopprice <Menge>` | | Setzt den Standardpreis für Ladengrundstücke fest.|
|`/town set embassyprice <Menge>` | | Setzt den Standardpreis für Botschaftsgrundstücke fest.|
|`/town toggle explosion` | | Schaltet Explosionen zwischen an und aus um.|
|`/town toggle fire` | | Schaltet Feuerverteilung zwischen an und aus um.|
|`/town toggle mobs` | | Schaltet Monster zwischen an und aus um.|
|`/town toggle public` | | Schaltet die Spawncoordinaten-Veröffentlichung zwischen an und aus um.|
|`/town toggle pvp` | | Schaltet Spieler gegen Spieler zwischen an und aus um.|
|`/town toggle explosion` | | Schaltet prozentuale Steuerberechnung zwischen an und aus um.|
|`/town toggle open` | | Schaltet betretbarkeit in die Stadt für jeden Spieler zwischen an und aus um.|
|`/town toggle jail <Nummer> <Spielername>` | `/town jail 1 Immanuel94` | Steckt den angegebenen Spieler in die angegebene Gefängnisnummer.|
||||
|`/nation ?` | | Zeigt verfügbare Befehle des `/nation` Befehls an.|
|`/nation list` | | Zeigt eine Liste aller Nationen an.|
|`/nation online` | | Zeigt eine Liste aller Spieler an, die gerade in der Nation online sind.|
|`/nation` | | Zeigt Informationen über die aktuelle Nation des Spielers an.|
|`/nation <Nationsname>` | | Zeigt Informationen über die angegebene Nation an.|
|`/nation leave` | | Verlässt die aktuelle Nation.|
|`/nation withdraw <Menge>` | | Hebt die angegebene Menge vom Nationskonto ab.|
|`/nation deposit <Menge>` | | Schreibt die angegebene MEnge dem Nationskonto gut.|
|`/nation new <Nationsname>` | | Erstelle eine neue Nation mit dem angegebenen Namen.|
|`/nation rank` <add/remove> <Spielername> <Rangname> | | Ermöglicht eigene Ränge in der Nation einzufügen.|
|`/nation add <Stadtname>` | |Lädt die angegebene Stadt zur Nation ein.|
|`/nation remove <Stadtname>` | |Entfernt die Stadt von der Nation.|
|`/nation delete` | |Löscht die eigene Nation.|
|`/nation ally add <Nationsname>` | |Fügt eine andere Nation zur Allianz hinzu.|
|`/nation ally remove <Nationsname>` | |Entfernt eine andere Nation aus der Allianz.|
|`/nation enemy add <Nationsname>` | |Fügt eine andere Nation als Feind hinzu.|
|`/nation enemy remove <Nationsname>` | |Entfernt eine andere Nation aus der Feindschaft.|
|`/nation say <Nachricht>` | |Sendet eine Nachricht an alle Nationsmitglieder.|
|`/nation set king <Spielername>` | |Gibt den Königsrang an den angegebenen Spieler ab.|
|`/nation set capital <Stadtname>` | |Setzt die Hauptstadt zum angegebenen Stadtnamen.|
|`/nation set board <Nachricht>` | |Setzt eine Nachricht, die alle Nationsmitglieder beim beitreten des Servers angezeigt bekommen.|
|`/nation set taxes <Menge>` | |Setzt die Steuer für die Nation zur angegebenen Menge.|
|`/nation set name <Nationsname>` | |Ändert den Namen der Nation zum angegebenen Namen.|
|`/nation set spawn` | |Setzt den Spawn der Nation zum Ort des Spielers.|
|`/nation set spawncost` | |Setzt die Kosten für `/nation spawn` für andere Spieler, die nicht in der Nation sind.|
|`/nation set tag <text>` | |Setzt den Tag der Nation, maximal 4 Zeichen.|
|`/nation set tag clear` | |Entfernt den gesetzten Tag der Nation.|
|`/nation set title <Spielername > <Titel>` | |Setzt den Titel des Spielers.|
|`/nation set surname <Spielername> <Nachname>` | |Setzt den Nachnamen des Spielers.|
|`/nation toggle neutral` | |Macht die Nation neutral und im Krieg unangreifbar, kostet im Krieg täglich eine höhe Gebühr.|

[^1]: Weitere Befehle für Towny auf https://github.com/TownyAdvanced/Towny/wiki/Towny-Commands
