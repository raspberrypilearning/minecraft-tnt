## Minecraft mit Python steuern

The block ID for TNT is `46`. There are two types of TNT: unexplosive TNT and explosive TNT. You want explosive TNT.

\--- task \---

Build a solid cube of TNT. Ände die `1` am Ende der `setBlock` Zeile zu einer `2`:

```python
mc.setBlocks(x+1, y+1, z+1, x+11, y+11, z+11, 1)
```

\--- /task \---

\--- task \---

Go up to the cube of TNT and hit it with your sword using right-click. This will activate the TNT. Stand back and watch the show!

\--- /task \---