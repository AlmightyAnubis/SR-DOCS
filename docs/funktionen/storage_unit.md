# Lagersysteme

!!! info inline end ""
    ![Lagersystem Rezept](citybuild_lagersystem_rezept.png)
    Das Rezept für neue Lagersysteme

Möchte man viele Gegenstände im Citybuild lagern, bietet sich ein Lageersystem an. 

	
## Lagersysteme aufstellen
Du kannst ein Lagersystem überall aufstellen, wo du möchtest. Beachte, dass die Lagersysteme von sich aus nicht gesichert sind und damit auch gestohlen werden können. Lagersysteme können nicht über Trichtern platziert werden, da die Lagersysteme nicht mit Trichtern geleert werden können.

## Lagersysteme auffüllen
Es gibt mehrere Möglichkeiten, ein Lagersystem aufzufüllen:

=== "Über das Menü"
    !!! note ""
        Öffne das Lagersystem wie eine Kiste und lege den Gegenstand zum lagern hinein. Hast du bereits Items hineingelegt, kannst du auf die Kiste im Menü des Lagersystems klicken, um gleichzeitig alle passenden Gegeenstände automatisch in dein Lagersystem einzulagern.
    ![Über das Menü](citybuild_lagersystem_einlagern_mit_menu.png)
=== "Mit einem Trichter"
    !!! note ""
        Ist dir der Vorgang über das Menü zu aufwändig, kannst du ebenfalls einen Trichter an das Lagersystem anschließen und damit einen Gegenstand autoamtisch in deinem Lagersystem einlagern.
    ![Mit einem Trichter](citybuild_lagersystem_einlagern_mit_trichter.png)
=== "Mithilfe eines Rohrs"
    !!! note ""
        Hast du den [Techniker Skill](citybuild_techniker.md) und strebst eine besonders schnelle und effiziente Verbindung an, kann man das Lagersystem ebenfalls mit einer [Röhre](citybuild_techniker.md#9-rohren) auffüllen.
    ![Mit einem Rohr](citybuild_lagersystem_einlagern_mit_rohr.png)

## Lagersysteme leeren
Es gibt mehrere Möglichkeiten, ein Lagersystem aufzufüllen:

=== "Über das Menü"
    !!! note ""
        Möchtest du eine kleine Menge aus dem Lagersystem entnehmen, klicke einfach auf das Item im Menü des Lagersystems.
    ![Über das Menü](citybuild_lagersystem_leeren_mit_menu.png)
	
=== "Mit der Export Funktion"
    !!! note ""
        Wenn du schnell die Gegenstände aus dem Lager automatisch an einen anderen Ort transportieren willst, kannst du mithilfe der Export Funktion die Gegenstände in eine Kiste legen.
		Um diese Funktion zu nutzen, wird ein Infoschild für das Lagersystem benötigt, wie dieses aufgestellt wird, steht unter [Infoschild](#Infoschild).
		
		Je nach gewünster Exportmethode gibt es verschiedene Einstellungen. Um eine Einstellung für den Export zu definieren, schreibe diese einfach in die vierte Zeile des Infoschilds:

		- Leeren auf bis zu 1 Item: `EMPTY`
		- Komplett entleeren: `FULLYEMPTY`
		- Komplett entleeren und dann abbauen: `FULLYEMPTYBREAK`
		
    ![Mit einem Rohr](citybuild_lagersystem_leeren_mit_export.png)
	
## Infoschild
!!! info inline end ""
    ![Lagersystem Rezept](citybuild_lagersystem_infoschild.png)
    Ein eingerichtetes Infoschild

Über ein Infoschild können weitere Informationen angezeigt werden, wie beispielweise der im Lagersystem enthaltene Gegenstand und die Lagermenge.
Neben diesen Informationen kann auch eine Anweisung für das Lagersystem in die vierte Zeile des Infoschilds geschrieben werden.

Um ein Infoschild aufzustellen, platziere ein Schild mit `[Storage]` auf der ersten Zeile über einem Lagersystem, es wird sich automatisch einrichten.
Möchtest du eine Anweistung hinzufügen, kannst du diese einfach beim erstellen des Schildes in der vierten Zeile mit hinzufügen.
