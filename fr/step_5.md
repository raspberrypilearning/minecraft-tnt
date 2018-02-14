## TNT

L'ID de bloc pour TNT est `46`. Il existe deux types de TNT: le TNT non explosif et le TNT explosif. Vous voulez TNT explosif.

1. Construire un solide cube de TNT. Pour obtenir TNT explosif, vous devez ajouter un `1` à la fin de votre `setBlocks` ligne:
    
    ```python
mc.setBlocks (x + 1, y + 1, z + 1, x + 11, y + 11, z + 11, 46, 1)
```

2. Montez au cube de TNT et frappez-le avec votre épée en utilisant le clic-droit. Cela activera le TNT. Reculez et regardez le spectacle!