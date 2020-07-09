## Entra nel mondo di Minecraft

\--- task \---

Enter the following code:

```python
Sposta le finestre per far sì che Minecraft e Python siano affiancati.
```

\--- /task \---

\--- task \---

Sposta le finestre per far sì che Minecraft e Python siano affiancati.

\--- /task \---

\--- task \---

Add the following lines to your code:

```python
x, y, z = mc.player.getPos()
mc.setBlock(x+1, y, z, 1)
```

\--- /task \---

\--- task \---

Run the code and you should see a block of stone appear near your player. If it's not in front of you, try looking around.

\--- /task \---

\--- task \---

Change the `1` at the end of the `setBlock` line to a `2`:

```python
mc.setBlock(x+1, y, z, 2)
```

\--- /task \---

\--- task \---

You should now see a block of grass appear. Try changing the number again and see what kind of block gets placed.

\--- /task \---

\--- task \---

Try changing `setBlock` to `setBlocks` to build a 10x10x10 cube rather than a single block:

```python
mc.setBlocks(x+1, y+1, z+1, x+11, y+11, z+11, 1)
```

You should see a large solid cube of stone appear!

\--- /task \---