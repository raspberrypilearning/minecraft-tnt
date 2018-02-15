## Contrôle de Minecraft avec Python

1. Ouvrez un nouveau fichier Python et entrez-y le code suivant:
    
    ```python
from mcpi.minecraft import Minecraft

mc = Minecraft.create()

mc.postToChat("Bonjour monde!")
```

2. Exécutez le code avec la touche `F5` et vous devriez voir le message "Bonjour monde!" apparaître dans la fenêtre Minecraft.

3. Ajoutez les lignes suivantes à votre code:
    
    ```python
x, y, z = mc.player.getPos()
mc.setBlock(x+1, y, z, 1)
```

4. Exécutez le code et vous devriez voir un bloc de pierre apparaître devant votre personnage. S'il n'est pas devant vous, essayez de regarder autour de vous.

5. Changez le `1` à la fin de la ligne `setBlock` pour un `2`:
    
    ```python
mc.setBlock(x+1, y, z, 2)
```

6. Vous devriez maintenant voir un bloc d'herbe apparaître. Essayez de changer à nouveau le numéro et voyez quel type de bloc est placé.

7. Essayez de changer `setBlock` à `setBlocks` pour construire un cube 10x10x10 plutôt qu'un seul bloc:
    
    ```python
mc.setBlocks (x + 1, y + 1, z + 1, x + 11, y + 11, z + 11, 1)
```

Vous devriez voir apparaître un grand cube de pierre solide!