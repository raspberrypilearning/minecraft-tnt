## PythonでMinecraftをコントロールします

1. 新しいPythonウィンドウを開き、以下のコードを入力します：
    
    ```python
from mcpi.minecraft import Minecraft

mc = Minecraft.create()

mc.postToChat("Hello world")
```

2. `F5`でコードを実行します。 Minecraftウィンドウに "Hello world"というメッセージが表示されます。

3. コードに次の行を追加します。
    
    ```python
x, y, z = mc.player.getPos()

mc.setBlock(x+1, y, z, 1)
```

4. コードを実行すると、プレーヤーの近くに石のブロックが表示されます。 石のブロックが見えない場合は、あたりを見回してみてください。

5. `setBlock`関数の最後の`1`を`2`に変更してください。：
    
    ```python
mc.setBlock(x+1, y, z, 2)
```

6. 草のブロックが現れるはずです。 番号をもう一度変更して、ブロックの種類を確認してください。

7. `setBlock`関数を`setBlocks`関数に変更してみましょう。ブロック1つではなく、10x10x10の立方体を作成します：
    
    ```python
mc.setBlocks(x+1, y+1, z+1, x+11, y+11, z+11, 1)
```

大きな石の立方体が現れます。