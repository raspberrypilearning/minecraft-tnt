## Het besturen van Minecraft met Python

--- task ---

Voer de volgende code in:

```python
from mcpi.minecraft import Minecraft 

mc = Minecraft.create () 

mc.postToChat ("Hello world")
```

--- /task ---

--- task ---

Voer het programma uit door op **F5** te drukken en u zou het bericht "Hallo wereld" in het Minecraft-venster moeten zien verschijnen.

--- /task ---

--- task ---

Voeg de volgende regels toe aan uw programma:

```python
x, y, z = mc.player.getPos () 

mc.setBlock (x + 1, y, z, 1)
```

--- /task ---

--- task ---

Voer het programma uit (F5) en je zou een steenblok in de buurt van je speler moeten zien verschijnen. Als het niet voor je is, kijk dan even rond.

--- /task ---

--- task ---

Wijzig de `1` aan het einde van de `setBlock` regel naar een `2`:

```python
mc.setBlock (x + 1, y, z, 2)
```

--- /task ---

--- task ---

Je zou nu een blok gras moeten zien verschijnen. Probeer het nummer opnieuw te veranderen en kijk welk blok wordt geplaatst.

--- /task ---

--- task ---

Probeer te veranderen `setBlock` naar `setBlocks` om een ​​kubus van 10x10x10 te bouwen in plaats van een enkel blok:

```python
mc.setBlocks (x + 1, y + 1, z + 1, x + 11, y + 11, z + 11, 1)
```

Je zou een grote, stevige kubus van steen moeten zien verschijnen!

--- /task ---