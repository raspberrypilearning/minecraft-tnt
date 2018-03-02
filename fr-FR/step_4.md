## Contrôlez Minecraft avec Python

1. Ouvrez une nouvelle fenêtre Python et entrez le code suivant :
    
    ```python
    from mcpi.minecraft import Minecraft

    mc = Minecraft.create()

    mc.postToChat("Bonjour à tous")
    ```

2. Exécutez le code avec `F5` et vous devriez voir apparaître le message "Bonjour à tous" dans la fenêtre Minecraft.

3. Ajoutez les lignes suivantes à votre code:
    
    ```python
    x, y, z = mc.player.getPos()
    mc.setBlock(x+1, y, z, 1)
    ```

4. Exécutez le code et vous devriez voir un bloc de pierre apparaître près de votre joueur. Si ce n'est pas en face de vous, essayez de regarder autour de vous.

5. Remplacez le `1` à la fin de la ligne `setBlock` par à un `2` :
    
    ```python
    mc.setBlock(x+1, y, z, 2)
    ```

6. Vous devriez maintenant voir apparaître un bloc d'herbe. Essayez de changer à nouveau le numéro et voyez quel type de bloc est placé.

7. Essayez de remplacer `setBlock` par `setBlocks` pour construire un cube de 10x10x10 plutôt qu'un seul bloc :
    
    ```python
    mc.setBlocks(x+1, y+1, z+1, x+11, y+11, z+11, 1)
    ```

    Essayez de remplacer <0>setBlock</0> par <0>setBlocks</0> pour construire un cube de 10x10x10 plutôt qu'un seul bloc :
