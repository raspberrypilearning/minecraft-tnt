## TNT

L'ID de block du TNT est `46`. Il y a deux types de blocs de TNT: TNT inerte et TNT explosif. Vous voulez utiliser le TNT explosif.

1. Construisez un cube de TNT. Pour obtenir du TNT explosif, vous devez ajouter un `1` à la fin de votre ligne `setBlocks`:
    
    ```python
    mc.setBlocks(x+1, y+1, z+1, x+11, y+11, z+11, 46, 1)
    ```

2. Allez jusqu'au cube de TNT et frappez le avec votre épée en utilisant le bouton droit de la souris. Ceci activera le TNT. Reculez vous et admirez le spectacle!
