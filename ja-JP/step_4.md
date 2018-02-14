## PythonでMinecraftを制御する

1. 新しいPythonウィンドウを開き、次のコードを入力します：
    
    ```python
mcpi.minecraftからのインポートMinecraft mc = Minecraft.create（）mc.postToChat（ "Hello world"）
```

2. コードを`F5`で実行します。 Minecraftウィンドウに "Hello world"というメッセージが表示されます。

3. コードに次の行を追加します。
    
    ```python
x、y、z = mc.player.getPos（）mc.setBlock（x + 1、y、z、1）
```

4. コードを実行すると、プレーヤーの近くに石のブロックが表示されます。 それがあなたの目の前にない場合は、見回してみてください。

5. `1`を変更してください。 | 123_6_2_321の終わりに| setBlock</code> `2`：
    
    ```python
mc.setBlock（x + 1、y、z、2）
```

6. あなたは今、草のブロックが現れるはずです。 番号をもう一度変更して、ブロックの種類を確認してください。

7. 変更しよう`setBlock` 〜`setBlocks` 1つのブロックではなく10x10x10の立方体を構築する：
    
    ```python
mc.setBlocks（x + 1、y + 1、z + 1、x + 11、y + 11、z + 11,1）
```

大きな石の立方体が現れます。