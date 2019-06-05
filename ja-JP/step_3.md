## PythonでMinecraftを制御する

\--- task \---

次のコードを入力します。

```python
from mcpi.minecraft import Minecraft

mc = Minecraft.create()

mc.postToChat("Hello world")
```

\--- /task \---

\--- task \---

**F5**でコードを実行します。 Minecraftウィンドウに"Hello world"というメッセージが表示されます。

\--- /task \---

\--- task \---

コードに次の行を追加します。

```python
x, y, z = mc.player.getPos()

mc.setBlock(x+1, y, z, 1)
```

\--- /task \---

\--- task \---

コードを実行すると、プレーヤーの近くに石のブロックが表示されます。 石のブロックが見えない場合は、あたりを見回してみてください。

\--- /task \---

\--- task \---

`setBlock`行の最後の`1`を`2`に変更してください。

```python
mc.setBlock(x+1, y, z, 2)
```

\--- /task \---

\--- task \---

草のブロックが現れるはずです。 もう一度番号を変更して、どんな種類のブロックが置かれるか確認します。

\--- /task \---

\--- task \---

`setBlock`を`setBlocks`に変更して、1つのブロックではなく10x10x10の立方体を作成してみましょう。

```python
mc.setBlocks(x+1, y+1, z+1, x+11, y+11, z+11, 1)
```

大きな石の立方体が現れるはずです！

\--- /task \---