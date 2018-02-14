## Minecraft mit Python kontrollieren

1. Öffnen Sie ein neues Python-Fenster und geben Sie folgenden Code ein:
    
    ```python
von mcpi.minecraft import Minecraft mc = Minecraft.create () mc.postToChat ("Hallo Welt")
```

2. Führen Sie den Code mit `F5` aus und du solltest die Nachricht "Hello world" im Minecraft Fenster sehen.

3. Fügen Sie Ihrem Code die folgenden Zeilen hinzu:
    
    ```python
x, y, z = mc.player.getPos () mc.setBlock (x + 1, y, z, 1)
```

4. Führe den Code aus und du solltest einen Steinblock in der Nähe deines Spielers sehen. Wenn es nicht vor dir ist, versuche dich umzusehen.

5. Ändern Sie die `1` am Ende der `setBlock` Linie zu a `2`:
    
    ```python
mc.setBlock (x + 1, y, z, 2)
```

6. Sie sollten jetzt einen Grasblock erscheinen sehen. Versuchen Sie, die Nummer erneut zu ändern und zu sehen, welche Art von Block platziert wird.

7. Versuchen Sie es zu ändern `setBlock` zu `setBlocks` um einen 10x10x10 Würfel anstelle eines einzelnen Blocks zu bauen:
    
    ```python
mc.setBlocks (x + 1, y + 1, z + 1, x + 11, y + 11, z + 11, 1)
```

Sie sollten einen großen soliden Steinwürfel sehen!