## 编辑一个独角兽随着彩虹跳舞

在这个步骤中，我们会应用Scratch编辑一个随着彩虹颜色变换的节奏舞蹈的独角兽。 我们需要用到一个按钮来操控彩虹和跳舞的独角兽。

### 独角兽子画面

选择以下之一以作为独角兽子画面：

1. 使用Scratch中独角兽子画面
2. 从其他地方上传独角兽图片并将其用作你的子画面
3. 在Scratch或其他程序中绘制自己的独角兽图像 (如右边可爱的绿色独角兽)。

示例：

|              (1) Scratch子画面：              |            (2) 上传图片：            |            (3) 绘制图像：             |
|:-----------------------------------------:|:-------------------------------:|:--------------------------------:|
| ![Scratch 独角兽](images/scratchunicorn.png) | ![网络独角兽](images/webunicorn.png) | ![绘制独角兽](images/drawunicorn.png) |

\--- task \--- 如果选1，请点这里 [[[generic-scratch3-sprite-from-library]]] \--- /task \---

\--- task \--- 如果选2，因为要上传从其他地方找到的独角兽图像，请先单击下面的内容以了解图像权限，然后使用第二个框中的说明上传文件： [[[images-permissions-to-use]]]

[[[generic-scratch3-sprite-from-library]]] \--- /task \---

\--- task \--- 如果选3，请单击下面的说明，以了解如何在Scratch中绘制自己的独角兽： [[[generic-scratch3-draw-sprite]]] \--- /task \---

### 独角兽造型

你的独角兽需要不同的**造型**才能够跳舞。 造型是一组子画面之一，也就是说我们可以通过更改独角兽的造型来改变我们看到的子画面外观。 因此，我们可以通过 改变造型使子画面看起来像是在动，并借此创建动画。

在这里，我们要创建一个独角兽跳舞的动画，因此每个造型都代表独角兽的一个舞蹈动作。

\--- task \--- 想好要让独角兽跳舞的造型数量，并编辑对应数量的造型。

点击以提醒如何在Scratch中添加造型： [[[generic-scratch3-add-costume]]]

点击以提醒如何复制Scratch中的造型： [[[generic-scratch3-duplicate-costumes]]] \--- /task \---

你想要为独角兽加几个造型都可以。 这个跳舞的绿色独角兽，我们使用了五组造型：

| ![Dancing Unicorn Gif](images/dancingunicorn.gif) | ![Five Costumes](images/fivecostumes.png) |

### 独角兽跳舞

要创建跳舞的动画，我们要对独角兽进行编程以切换造型。

\--- task \--- 在前两个造型之间切换让独角兽开始舞蹈。

要从第一个造型切换到第二个，请使用：

```blocks3
switch costume to [costume 2 v]
```

独角兽大多是优秀的舞者哦，因此请将独角兽变换舞步的节奏与彩虹灯闪烁的速度同步。 可以使用`wait`{:class="blockcontrol"}指令块来调整独角兽与彩虹的等待时间 并进行匹配。

```blocks3
wait (0.5) secs
switch costume to [costume 2 v]
```

\--- /task \---

\--- task \--- 想让独角兽跳舞，我们要在所有造型之间连续切换。 需要用哪种循环？ \--- /task \---

\--- hints \--- \--- hint \---

使用forever（永久）循环：

```blocks3
forever
```

\--- /hint \--- \--- hint \---

每次循环时，使用此指令块切换到下一个造型：

```blocks3
next costume
```

\--- /hint \--- \--- hint \---

你的指令应该是这样的：

```blocks3
forever
wait (0.5) secs
next costume
```

\--- /hint \--- \--- /hints \---