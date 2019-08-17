## Minecraft irányítása Pythonnal

\--- task \---

Írd be a következő kódot:

```python
from mcpi.minecraft import Minecraft 

mc = Minecraft.create () 

mc.postToChat ("Hello world")
```

\--- /task \---

\--- task \---

Futtasd a kódot az **F5** paranccsal és a Minecraft ablakban megjelenik a "Hello világ" üzenet.

\--- /task \---

\--- task \---

Add hozzá a következő sorokat a kódodhoz:

```python
x, y, z = mc.player.getPos () 

mc.setBlock (x + 1, y, z, 1)
```

\--- /task \---

\--- task \---

Futtasd a kódot, és megjelenik egy kőblokk a játékosod közelében. Ha nincs előtted, nézegess körbe.

\--- /task \---

\--- task \---

Váltsd az `1` -t a `setBlock` sor végén `2`-re:

```python
mc.setBlock (x + 1, y, z, 2)
```

\--- /task \---

\--- task \---

Most egy fűtömbnek kellene megjelennie. Próbáld újra megváltoztatni a számot, és figyeld meg, hogy milyen blokk jelenik meg.

\--- /task \---

\--- task \---

Próbáld megváltoztatni a `setBlock`-t `setBlocks`-ra, így egy blokk helyett egy 10x10x10 kockád lesz:

```python
mc.setBlocks (x + 1, y + 1, z + 1, x + 11, y + 11, z + 11, 1)
```

Most egy nagy kőtömbnek kellene megjelennie!

\--- /task \---