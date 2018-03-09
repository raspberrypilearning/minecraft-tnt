## TNT

The block ID for TNT is `46`. There are two types of TNT: unexplosive TNt and explosive TNT. You want explosive TNT.

1. Build a solid cube of TNT. To get explosive TNT, you need to add a `1` to the end of your `setBlocks` line:

    ```python
    mc.setBlocks(x+1, y+1, z+1, x+11, y+11, z+11, 46, 1)
    ```

1. Go up to the cube of TNT and hit it with your sword using right-click. This will activate the TNT. Stand back and watch the show!
