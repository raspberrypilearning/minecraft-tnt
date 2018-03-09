## TNT

Die Block-ID für TNT ist `46`. Es gibt zwei Arten von TNT: nicht explodierendes TNt und explosives TNT. Du willst explosives TNT.

1. Baue einen massiven Würfel von TNT. Um explosives TNT zu erhalten, musst du eine `1` am Ende deiner `setBlocks` Zeile anfügen:
    
    ```python
    mc.setBlocks(x+1, y+1, z+1, x+11, y+11, z+11, 46, 1)
    ```

2. Geh zum Würfel von TNT und schlag ihn mit deinem Schwert mit der rechten Maustaste. Dies aktiviert das TNT. Tritt zurück und schau dir die Show an!
