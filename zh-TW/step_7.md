## 點亮你的彩虹

為確保你的彩虹正常運作，首先你得通過一次點亮整個彩虹來對其進行測試。 然後，您將編寫程式來使彩虹發出所有顏色，一個接一個地，接著再以您選擇的模式閃爍所有顏色。

\---task\--- 編寫更多代碼來控制其他LED。 確認你包括正確的GPIO針腳。 \--- /task \---

你的彩虹應該像這樣點亮：

![彩虹燈](images/rainbowlit.png)

\--- hints \--- \--- hint \--- 添加更多`打開LED（0 v）[on v] ` {:class="block3extensions"}方塊在以下的代碼塊中：

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```

\--- /hint\--- \---hint\--- 繼續在代碼底部添加方塊，直到所有LED均設置為`開啟 ` {:class="block3extensions"}狀態。

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
turn LED (18 v) [on v] ::extension
turn LED (22 v) [on v] ::extension
```

\--- /hint \--- \--- hint \---

如果你的LED點不亮：

1）檢查你的LED連接到哪個GPIO引腳，並確保已將它們設置為`開啟 ` {:class="block3extensions"}。 2）測試LED是否運作，您可以將LED的跳線插入** GPIO 3V3 **測試。 3）確認麵包板上的電路完整。

\--- /hint \--- \--- /hints \---

\---task\--- 現在，添加更多代碼來使彩虹以彩虹圖案閃爍，如下所示：<video width="560" height="315" controls> <source src="resources/Scratch-GPIO-Pathways-5.mp4" type="video/mp4"> 您的瀏覽器不支持此視頻，請嘗試使用FireFox或Chrome。 </video> 

為此，您需要使一個LED點亮幾秒鐘，然後在下一個LED點亮時同時熄滅。 \--- /task \---

\--- hints \--- \--- hint \---

確認您的`事件` {:class="blockevents"} 區塊與您要測試程式碼的內容一樣。 在此處的範例中，要使彩虹閃爍，我們必須單擊綠色旗幟：

```blocks3
when flag clicked
```

\--- /hint \--- \--- hint \---

如果你卡住了，請確認你正在使用以下積木：

```blocks3
turn LED (0 v) [off v] ::extension
wait () secs
```

\--- /hint \--- \--- hint \---

嘗試使用這種方法：

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

您將需要為所有LED添加積木，並確保在代碼中使用正確的GPIO針腳號碼。

\--- /hint \--- \--- /hints \---

\---task\--- 使燈光反覆閃爍透過在迴圈的彩虹。

要永久循環彩虹模式，請使用：

```blocks3
forever
```

\--- /task \---

\--- challenge \---

+ 使彩虹按您選擇的方式閃爍。

## \--- collapse \---

## 標題：彩虹挑戰

嘗試以下的點子：

1）使LED閃爍非常快和非常慢 2）使整個彩虹閃爍 3）使成對的LED以交替的模式點亮 4）使彩虹閃爍摩斯密碼 5）使彩虹對不同事件做不同的事情

\--- /collapse \--- \--- /challenge \---