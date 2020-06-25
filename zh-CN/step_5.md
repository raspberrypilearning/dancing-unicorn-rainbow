## 控制彩虹电路

设置好整个彩虹后，你可以控制它的闪烁方式。 先试试用Scratch进行如下操作来控制一盏LED灯

\--- task \--- 按下<kbd>P</kbd>键，让LED点亮两秒钟后熄灭。 \--- /task \---

\--- hints \--- \--- hint \--- 查看`Control`部分 使用

```blocks3
  wait (2) secs
```

\--- /hint \--- \--- hint \---

```blocks3
when [p v] key pressed
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
```

\--- /hint \--- \--- /hints \---

\--- task \--- 当Scratch程序启动后，让你的LED灯亮2秒，然后熄灭2秒。 \--- /task \---

\--- hints \--- \--- hint \---

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

\--- /hint \--- \--- /hints \---

\--- task \--- 只要程序在运行LED就会持续闪烁。 \--- /task \---

使用

```blocks3
forever
```

\--- /hint \--- \--- hint \---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

\--- /hint \--- \--- /hints \---

+ 让 LED 闪烁的更快。

-- 提示 -- 在` wait x secs ` {：class =“ block3control”}中设定更短的秒数。 \--- /hint \--- \--- hint \---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (0.5) secs
turn LED (17 v) [off v] ::extension
wait (0.5) secs
```

\--- /hint \--- \--- /hints \---

干得漂亮 —— 现在你已经可以组装并且操控一道绚烂的彩虹了！