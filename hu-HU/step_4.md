## Az Minecraft és a Python irányítása

1. Nyisson meg egy új Python ablakot, és írja be a következő kódot:
    
    ```python
az mcpi.minecraft importálásából Minecraft mc = Minecraft.create () mc.postToChat ("Hello world")
```

2. Futtassa a kódot a `F5` paranccsal és a Minecraft ablakban megjelenik a "Hello world" üzenet.

3. Adja hozzá a következő sorokat a kódjához:
    
    ```python
x, y, z = mc.player.getPos () mc.setBlock (x + 1, y, z, 1)
```

4. Futtassa a kódot, és megjelenik egy kőblokk a játékos közelében. Ha nem előtted áll, próbáljon körülnézni.

5. Módosítsa a `1` -t a 123_6_2_321 | setBlock</code> végén a végén sor egy `2`:
    
    ```python
mc.setBlock (x + 1, y, z, 2)
```

6. Most látnia kell egy fűtömböt. Próbálja meg ismét a számot megváltoztatni, és nézze meg, hogy milyen blokkot kap.

7. Próbálja meg megváltoztatni `setBlock` `setBlokkok` 10x10x10 kockát kell létrehoznia, nem pedig egyetlen blokkot:
    
    ```python
mc.setBlocks (x + 1, y + 1, z + 1, x + 11, y + 11, z + 11, 1)
```

Látnia kell egy nagy szilárd kő kockát!