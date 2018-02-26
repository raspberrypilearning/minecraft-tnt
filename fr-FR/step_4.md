## Contrôler Minecraft avec Python

1. Ouvrez une nouvelle fenêtre Python et entrez le code suivant:
    
    ```python
from mcpi.minecraft import Minecraft

mc = Minecraft.create()

mc.postToChat("Bonjour à tous")
```

2. Exécutez le code avec `F5` et vous devriez voir que le message "Bonjour à tous" apparaît dans la fenêtre Minecraft.

3. Ajoutez les lignes suivantes à votre code:
    
    ```python
x, y, z = mc.player.getPos()
mc.setBlock(x+1, y, z, 1)
```

4. Exécutez le code et vous devriez voir un bloc de pierre apparaître près de votre lecteur. Si ce n'est pas en face de vous, essayez de regarder autour de vous.

5. Changez le `1` à la fin de la ligne `setBlock` à un `2`:
    
    ```python
mc.setBlock(x+1, y, z, 2)
```

6. Vous devriez maintenant voir qu'un bloc d'herbe apparaît. Essayez de changer à nouveau le numéro et voyez quel type de bloc est placé.

7. Essayez de changer `setBlock` à `setBlocks` pour construire un cube 10x10x10 plutôt qu'un seul bloc:
    
    ```python
mc.setBlocks(x+1, y+1, z+1, x+11, y+11, z+11, 1)
```

Vous devriez voir apparaître un grand cube de pierre solide!