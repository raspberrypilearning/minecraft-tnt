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

6. Vous devriez maintenant voir un bloc de gazon apparaître. Essayez de changer le nombre à nouveau et voyez quel type de bloc est créé.

7. Essayez de changer `setBlock` pour `setBlocks` pour créer un cube de 10x10x10 blocs plutôt qu'un bloc individuel:
    
    ```python
    mc.setBlocks(x+1, y+1, z+1, x+11, y+11, z+11, 1)
    ```

    Vous devriez maintenant voir un gros cube de pierre apparaître!
