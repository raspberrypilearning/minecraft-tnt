## Controlling Minecraft with Python

1. Open a new Python window and enter the following code:
    
    ```python
from mcpi.minecraft import Minecraft

mc = Minecraft.create()

mc.postToChat("Hello world")
```

2. Run the code with `F5` and you should see the message "Hello world" appear in the Minecraft window.

3. Add the following lines to your code:
    
    ```python
x, y, z = mc.player.getPos()
mc.setBlock(x+1, y, z, 1)
```

4. Run the code and you should see a block of stone appear near your player. If it's not in front of you, try looking around.

5. Change the `1` at the end of the `setBlock` line to a `2`:
    
    ```python
mc.setBlock(x+1, y, z, 2)
```

6. You should now see a block of grass appear. Try changing the number again and see what kind of block gets placed.

7. Try changing `setBlock` to `setBlocks` to build a 10x10x10 cube rather than a single block:
    
    ```python
mc.setBlocks(x+1, y+1, z+1, x+11, y+11, z+11, 1)
```

You should see a large solid cube of stone appear!