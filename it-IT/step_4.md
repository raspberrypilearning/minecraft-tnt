## Controllare Minecraft con Python

1. Apri una nuova finestra Python e inserisci il seguente codice:
    
    ```python
    from mcpi.minecraft import Minecraft 

    mc = Minecraft.create() 

    mc.postToChat("Ciao")
    ```

2. Esegui il codice con `F5`. Il messaggio "Ciao" dovrebbe comparire nella finestra di Minecraft.

3. Aggiungi le seguenti righe al tuo codice:
    
    ```python
    x, y, z = mc.player.getPos()
    mc.setBlock(x + 1, y, z, 1)
    ```

4. Esegui il codice. Un blocco di pietra dovrebbe apparire vicino al tuo personaggio. Se il blocco non è di fronte a te, prova a guardarti intorno.

5. Sostituisci l'`1` alla fine della riga `setBlock` con un `2`:
    
    ```python
    mc.setBlock(x + 1, y, z, 2)
    ```

6. Ora dovresti vedere apparire un blocco di erba. Prova a cambiare di nuovo il numero e vedi che tipo di blocco viene inserito.

7. Prova a cambiare `setBlock` con `setBlocks` per costruire un cubo di 10x10x10, anziché un singolo blocco:
    
    ```python
    mc.setBlocks(x + 1, y + 1, z + 1, x + 11, y + 11, z + 11, 1)
    ```

    Dovresti vedere apparire un enorme cubo di pietra!
