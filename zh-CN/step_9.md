## 添加按钮

现在，你只需按一下按钮，就可以让霓虹灯闪烁，并让独角兽随着灯光的变换起舞！

### 连接按钮

--- task --- 将按钮连接到面板和GPIO引脚。

单击下面的说明，了解如何将按钮连接到Raspberry Pi。 注意，我们用**GPIO 5**来连接按钮，而不是像简介里边使用**GPIO 17**—— **GPIO 17**已经连接到某个LED灯了。

[[[rpi-gpio-wiring-a-button]]]

你的彩虹应该看起来像这样：

![彩虹按钮](images/rainbowbutton.png) --- /task ---

### 编译按钮

--- task --- 用下面显示的指令块，就可以用按钮使独角兽跳舞。

```blocks3
when button (5 v) is [pressed v] :: hat extension
```

--- /task ---

### 控制独角兽舞蹈

目前应该有三大块Scratch指令：

1. 跳舞独角兽代码
2. 闪烁彩虹代码
3. 按钮代码

现在，我们将这些指令块连接起来，这样独角兽就可以随着彩虹变换起舞了，并且我们也可以通过按我们添加的按钮来控制彩虹和独角兽了。

--- task --- 删除按钮指令中所有`说`{:class="block3looks"}指令块，然后复制这组代码。 --- /task ---

--- task --- 在跳舞独角兽指令中，删除`当 ⚑ 被点击`{:class="block3events"}指令块。 将剩余的独角兽指令放入按钮指令的`否则`{:class="block3control"}指令块中。 仅将它放入按钮指令的**one copy**。 --- /task ---

--- task --- 在彩虹指令中，删除`当 ⚑ 被点击`{:class="block3events"}指令块，并将其余的彩虹指令插入按钮指令中**other copy** 指令块中的`否则`{:class="block3control"}指令块。 --- /task ---

--- task --- 在按钮指令两个副本的`如果`{:class="block3control"}插槽中添加一个操作。 可以使用`switch costume to first costume`{:class="block3looks"}，这样独角兽的舞蹈动作就不会乱了。 --- /task ---

--- hints ---
 --- hint --- 如果按下按钮霓虹灯没有亮起并且独角兽没有随着跳动，请尝试检查一下：

1. 每个组件是否都连接到正确的GPIO引脚
2. 指令中的输入和输出内容是否都正确
3. 两个指令块的时间是否匹配
4. 指令块是否全部使用正确
--- /hint ---
--- /hints ---