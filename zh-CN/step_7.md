## 点亮彩虹

为了确保彩虹能正常运作，先通过一次点亮全部霓虹灯来对其进行测试。 然后通过编辑指令，让霓虹灯按颜色依次闪烁，然后再按你设定的模式闪烁。

\--- task \--- 继续编辑指令来控制其他的LED灯。 确保在编辑过程中输入了正确的GPIO引脚编号。 \--- /task \---

霓虹灯应该会像这样闪烁：

![点亮彩虹](images/rainbowlit.png)

\--- hints \--- \--- hint \--- 添加`turn LED (0 v) [on v]`{:class="block3extensions"} blocks 代码块在这一组指令里：

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```

\--- /hint \--- \--- hint \--- 继续在你的代码后边添加代码块直到全部LED灯都设置为`on`{:class="block3extensions"}。

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
turn LED (18 v) [on v] ::extension
turn LED (22 v) [on v] ::extension
```

\--- /hint \--- \--- hint \---

如果LED灯不亮：

1) 检查LED都连接到了哪个GPIO引脚，并确保已将它们设置为`on` {:class =“block3extensions”} 2) 测试LED灯是否是好的——可以将LED的跳线插入** GPIO 3V3 **测试 3) 检查面板上的电路是否完整闭合

\--- /hint \--- \--- /hints \---

\--- task \--- 现在，通过编辑指令让霓虹灯像这样的规律闪烁：<video width="560" height="315" controls> <source src="resources/Scratch-GPIO-Pathways-5.mp4" type="video/mp4"> 如果您的浏览器不支持WebM视频，请尝试使用FireFox或Chrome。 </video> 

想达到这样的效果，您需要使一个LED点亮几秒钟，然后在下一个LED点亮的同时熄灭。 \--- /task \---

\--- hints \--- \--- hint \---

我们要确认`Events` {:class="blockevents"}代码块与要测试的指令的内容匹配。 在此处的示例中，我们须单击绿旗使彩虹闪烁：

```blocks3
when flag clicked
```

\--- /hint \--- \--- hint \---

如果程序运行不顺畅，请彩虹你有使用以下指令块：

```blocks3
turn LED (0 v) [off v] ::extension
wait () secs
```

\--- /hint \--- \--- hint \---

试试用这种方法：

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (0.5) secs
turn LED (17 v) [off v] ::extension
turn LED (18 v) [on v] ::extension
wait (0.5) secs
turn LED (18 v) [off v] ::extension
turn LED (22 v) [on v] ::extension
```

继续为所有LED灯添加指令块， 并确保在编辑过程 输入了正确的GPIO引脚编号。

\--- /hint \--- \--- /hints \---

让所有灯依次循环反复闪烁。

想令彩虹不停循环闪烁，可以用：

```blocks3
forever
```

\--- /task \---

\--- challenge \---

+ 让彩虹按你设想的模式闪烁。

## \--- collapse \---

## title: 彩虹挑战

试试下面的想法：

1) 使LED灯闪烁的频率加快或者减慢 2) 使整个彩虹闪烁 3) 使LED灯以成对交替的模式闪烁 4) 使霓虹灯按摩尔斯电码的规则闪烁来传递信息 5) 使霓虹灯根据不同的事件做出不同的反应

\--- /collapse \--- \--- /challenge \---