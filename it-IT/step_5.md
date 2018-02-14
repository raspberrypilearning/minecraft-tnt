## TNT

L'ID del blocco per TNT è `46`. Esistono due tipi di TNT: TNT non esplosivo ed TNT esplosivo. Vuoi un TNT esplosivo.

1. Costruisci un solido cubo di TNT. Per ottenere un TNT esplosivo, devi aggiungere un `1` alla fine del tuo `setBlocks` linea:
    
    ```python
mc.setBlocks (x + 1, y + 1, z + 1, x + 11, y + 11, z + 11, 46, 1)
```

2. Vai al cubo di TNT e colpiscilo con la tua spada usando il tasto destro. Questo attiverà il TNT. Stai indietro e guarda lo spettacolo!