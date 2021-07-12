--- no-print --- これは、このプロジェクトのスクラッチ3バージョンです。 [Scratch 2バージョンはここにあります。](https://projects.raspberrypi.org/ja-JP/projects/dancing-unicorn-rainbow-scratch2) --- / no-print ---

## はじめに

LEDで虹を作り、それに合わせてユニコーンを踊らせます。すべてRaspberry Piで動かします。

### 作るもの

Scratchを使用して、LEDの虹とユニコーンスプライトを連動させ、ユニコーンを虹のリズムに合わせてダンスさせます。 これは、踊っているユニコーンと虹がどのように見えるかを示すビデオです。
<video width="560" height="315" controls> <source src="resources/Screencast.mp4" type="video/mp4"> お使いのブラウザはビデオタグをサポートしていません。FireFoxまたはChromeをお試しください </video> 

ユニコーンを虹に合わせて踊るように訓練したら、レインボーを使用してユニコーンにトリックをさせたりゲームをプレイしたりする方法がわかるようになります。

--- collapse ---
---
title: 必要なもの
---

### ハードウェア

+ Raspberry Pi　1台
+ ブレッドボード　1台
+ 様々な色のLED　3個以上
+ 抵抗（100オーム以上）、**LED1個に1本**
+ 押しボタンスイッチ　1個
+ オス－メス ジャンパー線、**LED1個に1本**
+ オスーメス ジャンパー線　それ以外に2本
+ オスーオス ジャンパー線　1本

オプションの最終チャレンジ用に：

+ ブザー　1個
+ オスーメス ジャンパー線　それ以外にもう2本

### ソフトウェア

Raspbianの最新バージョンが必要です。これには、すでに次のソフトウェアが含まれています。

+ Scratch 3

```bash
sudo apt-get update
sudo apt-get install scratch3
```

**注意：**Scratch 3はRaspberry Pi 4で**だけ**動きます。 --- /collapse ---

--- collapse ---
---
title: 学ぶこと
---

このプロジェクトでは[Raspberry Pi デジタル・メイキング・カリキュラム](http://rpf.io/curriculum){:target="_blank"}（英語）の柱である、以下の要素を学びます。

+ [入力と出力を組み合わせてプロジェクトを作成、または問題を解決する](https://curriculum.raspberrypi.org/physical-computing/builder/){:target="_blank"}

+ [基本的なプログラミング構造を使って問題を解決する](https://www.raspberrypi.org/curriculum/programming/builder){:target="_blank} --- /collapse ---

--- collapse ---
---
title: 教育者向けの追加情報
---

このプロジェクトを印刷する必要がある場合は、 [印刷用バージョン](https://projects.raspberrypi.org/ja-JP/projects/dancing-unicorn-rainbow/print){:target="_blank"}を使用してください。

このプロジェクトの完全なソリューションは、[rpf.io/p/ja-JP/dancing-unicorn-rainbow-get](https://rpf.io/p/ja-JP/dancing-unicorn-rainbow-get)にあります --- /collapse ---