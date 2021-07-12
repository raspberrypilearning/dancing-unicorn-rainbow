## 虹を光らせる

虹がちゃんと点くことを確認するために、最初に虹全体を一度に光らせてテストします。 次に、虹のすべての色を次々と点滅させ、その後、選択したパターンで点滅させるコードを作成します。

--- task --- 他のLEDを制御するコードを追加します。 正しいGPIOピンを使っていることを確認してください。 --- /task ---

虹はこのように光るはずです：

![虹の点灯](images/rainbowlit.png)

--- hints ---
--- hint ---
`LED (0 v) [をオン v]にする`{:class="block3extensions"}ブロックをこのプログラムにさらに追加します:

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```

--- /hint ------ hint ---
全部のLEDが`on`{:class="block3extensions"}に設定されるまでコードの最後にブロックを追加します 。

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
turn LED (18 v) [on v] ::extension
turn LED (22 v) [on v] ::extension
```

--- /hint --- --- hint ---

LEDが点灯しない場合：

1）LEDが接続されているGPIOピンを確認し、それが`オン` {:class="block3extensions"}に設定されていることを確認します。 2）LEDが機能しているかどうかをテストします— LEDのジャンパー線を**GPIO 3V3**に接続することでテストできます。 3）ブレッドボードの回路が完全であることを確認します

--- /hint ------ /hints ---

--- task --- ここで、次のようなパターンで虹を点滅させるコードを追加します。
<video width="560" height="315" controls> <source src="resources/Scratch-GPIO-Pathways-5.mp4" type="video/mp4"> お使いのブラウザはビデオタグをサポートしていません。FirefoxまたはChromeをお試しください. </video> 

このようにするには、1つのLEDを数秒間オンにしてから、次のLEDがオンになると同時にオフにする必要があります。 --- /task ---

--- hints ---
 --- hint ---

`イベント`{:class="blockevents"}ブロックは、コードをテストするために行っていることと一致していることを確認してください。 この例では、虹を点滅させるために、緑の旗をクリックする必要があります。

```blocks3
when flag clicked
```

--- /hint --- --- hint ---

行き詰まった場合は、次のブロックを使用していることを確認してください。

```blocks3
turn LED (0 v) [off v] ::extension
wait () secs
```

--- /hint --- --- hint ---

このアプローチを試してください：

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

すべてのLEDのブロックを追加し、コードで正しいGPIOピン番号を使用していることを確認する必要があります。

--- /hint ------ /hints ---

--- task --- 虹のLEDを繰り返して次々に点滅し続けるようにします。

レインボーパターンを永久にループするには、これを使います。

```blocks3
forever
```

--- /task ---

--- challenge ---

+ 好きなパターンで虹を点滅させます。

--- collapse ---
---
title: レインボーチャレンジ
---

次のアイデアに挑戦してみてください。

1) LEDの点滅をとても速くしたりとても遅くしたりする 2) 虹全体を点滅させる 3) ペアになったLEDを交互に点灯する 4) 虹の点滅をモールス信号にする 5) さまざまなイベントに反応して虹にいろんなことをさせる

--- /collapse --- --- /challenge ---