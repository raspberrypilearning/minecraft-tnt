## Controllo di Minecraft con Python

1. Apri una nuova finestra Python e inserisci il seguente codice:
    
    ```python
da mcpi.minecraft import Minecraft mc = Minecraft.create () mc.postToChat ("Hello world")
```

2. Esegui il codice con `F5` e dovresti vedere il messaggio "Hello world" nella finestra di Minecraft.

3. Aggiungi le seguenti righe al tuo codice:
    
    ```python
x, y, z = mc.player.getPos () mc.setBlock (x + 1, y, z, 1)
```

4. Esegui il codice e dovresti vedere un blocco di pietra apparire vicino al tuo giocatore. Se non è di fronte a te, prova a guardarti intorno.

5. Modificare il `1` alla fine della `setBlock` linea a un `2`:
    
    ```python
mc.setBlock (x + 1, y, z, 2)
```

6. Ora dovresti vedere un blocco di erba apparire. Prova a cambiare di nuovo il numero e vedi che tipo di blocco viene inserito.

7. Prova a cambiare `setBlock` a `setBlocks` per costruire un cubo 10x10x10 anziché un singolo blocco:
    
    ```python
mc.setBlocks (x + 1, y + 1, z + 1, x + 11, y + 11, z + 11, 1)
```

Dovresti vedere apparire un grande cubo di pietra solido!