## Minecraft mit Python steuern

1. Öffne ein neues Python-Fenster und gib folgenden Code ein:
    
    ```python
    from mcpi.minecraft import Minecraft

    mc = Minecraft.create()

    mc.postToChat("Hallo Welt")
    ```

2. Führe den Code mit `F5` aus und du solltest die Nachricht "Hallo Welt" im Minecraft Fenster sehen.

3. Füge deinem Code die folgenden Zeilen hinzu:
    
    ```python
    x, y, z = mc.player.getPos()
    mc.setBlock(x+1, y, z, 1)
    ```

4. Führe den Code aus und du solltest einen Steinblock in der Nähe deines Spielers sehen. Wenn er nicht vor dir ist, versuche dich umzusehen.

5. Ände die `1` am Ende der `setBlock` Zeile zu einer `2`:
    
    ```python
    mc.setBlock(x+1, y, z, 2)
    ```

6. Du solltest jetzt einen Grasblock erscheinen sehen. Versuche, die Nummer erneut zu ändern und schau, welche Art von Block platziert wird.

7. Versuche `setBlock` zu `setBlocks` zu ändern, um einen 10x10x10 Würfel anstelle eines einzelnen Blocks zu bauen:
    
    ```python
    mc.setBlocks(x+1, y+1, z+1, x+11, y+11, z+11, 1)
    ```

    Du solltest einen großen, soliden Steinwürfel sehen!
