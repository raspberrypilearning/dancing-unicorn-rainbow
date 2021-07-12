## 虹色発光回路を操作する

虹色全てが準備できたら、虹をどのように点灯するかを制御できます。 1個のLEDを制御する簡単な練習として、Scratchを使って以下のことをやってみましょう:

--- task --- <kbd>P</kbd>キーを押すと、LEDをオンにして2秒たったらオフにします。 --- /task ---

--- hints ---
--- hint ---
`制御`{:class="block3control"}ブロックのセクションを見てください。
--- /hint ---
--- hint ---
これを使います

```blocks3
  (2) 秒待つ
```

--- /hint --- --- hint ---

```blocks3
when [p v] key pressed
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
```

--- /hint ------ /hints ---

--- task --- Scratchプログラムを起動すると、LEDを2秒間点灯させ、2秒間消灯します。 --- /task ---

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

--- task --- プログラムが実行されている間、LEDのオンとオフを繰り返します。 --- /task ---

--- hints ---
--- hint ---
これを使います

```blocks3
ずっと
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

+ LEDの点滅を速くします。

--- hints ---
--- hint ---
秒を短くするには`x 秒待つ`{:class="block3control"}を使います。
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

よくできました—これで素晴らしい虹を作成して制御する準備ができました！