## Python के साथ Minecraft का नियंत्रण करे

\--- task \---

निम्नलिखित कोड को दर्ज करें:

```python
from mcpi.minecraft import Minecraft

mc = Minecraft.create()

mc.postToChat("Hello world")
```

\--- /task \---

\--- task \---

**F5** दबाकर कोड चलाएं और "Hello world" संदेश Minecraft विंडो पर देखे।

\--- /task \---

\--- task \---

अपने कोड में निम्न पंक्तियां जोड़ें:

```python
x, y, z = mc.player.getPos()
mc.setBlock(x+1, y, z, 1)
```

\--- /task \---

\--- task \---

कोड चलने पर आपको अपने प्लेयर के पास पत्थर का एक ब्लॉक दिखाई देगा। यदि यह आपके सामने नहीं है, तो आसपास देखने का प्रयास करें।

\--- /task \---

\--- task \---

`setBlock` लाइन के आखिरी `1` को `2` में बदले:

```python
mc.setBlock(x+1, y, z, 2)
```

\--- /task \---

\--- task \---

अब आपको घास के एक ब्लॉक दिखाई देगा। संख्या को फिर से बदलने की कोशिश करें और देखें कि किस तरह का ब्लॉक रखा जाता है।

\--- /task \---

\--- task \---

`setBlock` को `setBlocks` में बदल कर एकल ब्लॉक के बजाय 10x10x10 का घन बनाए:

```python
mc.setBlocks(x+1, y+1, z+1, x+11, y+11, z+11, 1)
```

आपको पत्थर का एक बड़ा घनक्षेत्र दिखाई देगा!

\--- /task \---