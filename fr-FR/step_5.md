## TNT

L'ID de bloc pour le TNT est `46`. Il existe deux types de TNT : le TNT non explosif et le TNT explosif. Vous voulez du TNT explosif.

1. Construire un cube solide de TNT. Pour obtenir du TNT explosif, vous devez ajouter un `1` à la fin de votre ligne `setBlocks`:
    
    ```python
    mc.setBlocks(x+1, y+1, z+1, x+11, y+11, z+11, 46, 1)
    ```

2. Montez à la hauteur du cube de TNT et frappez-le avec votre épée en utilisant le clic-droit. Cela activera le TNT. Reculez et profitez du spectacle!
