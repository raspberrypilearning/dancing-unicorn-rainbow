## 控制你的彩虹電路

當你把彩虹架好了，你可以接著控制它該如何發亮。 來練習如何控制一個LED燈，你可以用Scratch操作以下步驟操作:

--- task --- 當你按 <kbd>P</kbd> 鍵時, 讓 LED燈亮兩秒鐘然後熄滅。 --- /task ---

--- hints ---
 --- hint --- 看看 `控制`{:class="block3control"} 的方塊部分。
--- /hint ---
 --- hint --- 使用

```blocks3
  等待（2）秒
```

--- /hint --- --- hint ---

```blocks3
when [p v] key pressed
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
```

--- /hint ------ /hints ---

---task--- 當Scratch程序啟動時，讓你的LED點亮2秒鐘，然後熄滅2秒鐘。 --- /task ---

--- hints ---
 --- hint ---

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

--- /hint ------ /hints ---

---task--- 只要程序運行，就點亮或熄滅LED。 --- /task ---

--- hints ---
 --- hint --- 使用

```blocks3
重複無限次
```

--- /hint --- --- hint ---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

--- /hint ------ /hints ---

+ 使你的LED閃爍得更快。

--- hints ---
 --- hint --- 使用`等待x 秒`{:class="block3control"} 來減少時間。
--- /hint ---
 --- hint ---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (0.5) secs
turn LED (17 v) [off v] ::extension
wait (0.5) secs
```

--- /hint ------ /hints ---

做得好! 你現在就可以創造和控制令人羨慕的彩虹了！