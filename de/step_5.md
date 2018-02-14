## TNT

Die Block-ID für TNT ist `46`. Es gibt zwei Arten von TNT: nicht explodierendes TNt und explosives TNT. Sie wollen explosive TNT.

1. Baue einen soliden Würfel von TNT. Um explosive TNT zu erhalten, müssen Sie ein `1` bis zum Ende deiner `setBlocks` Linie:
    
    ```python
mc.setBlocks (x + 1, y + 1, z + 1, x + 11, y + 11, z + 11, 46, 1)
```

2. Geh zum Würfel von TNT und schlag ihn mit deinem Schwert mit der rechten Maustaste. Dies aktiviert das TNT. Steh zurück und schau dir die Show an!