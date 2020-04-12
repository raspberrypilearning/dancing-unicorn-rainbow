## 무지개 밝히기

무지개가 제대로 작동하는지 확인하려면 먼저 무지개 전체를 한 번에 켠 다음 테스트하세요. 그런 다음 무지개를 모든 색상에서 차례로 깜박이도록 코드를 만들고, 그 다음에는 원하는 패턴으로 깜박이게 합니다.

\--- task \--- 다른 LED를 제어하기 위해 더 많은 코드를 추가하세요. 올바른 GPIO 핀을 포함하도록 조심하세요. \--- /task \---

무지개는 다음과 같이 켜져야 합니다:

![Rainbow Lit](images/rainbowlit.png)

\--- hints \--- \--- hint \--- Add more `turn LED (0 v) [on v]`{:class="block3extensions"} blocks in this chunk of code:

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```

\--- /hint \--- \--- hint \--- Keep adding blocks at the bottom of your code until all your LEDs are set to `on`{:class="block3extensions"}.

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
turn LED (18 v) [on v] ::extension
turn LED (22 v) [on v] ::extension
```

\--- /hint \--- \--- hint \---

LED가 켜지지 않는 경우:

1) LED가 어떤 GPIO 핀에 연결되어 있는지 확인하고 `켜짐`{:class="block3extensions"}으로 설정했는지 확인하세요 2) LED가 작동하는지 테스트하려면, LED의 점퍼 케이블을 **GPIO 3V3**에 꽂을 수 있습니다. 3) 브레드보드의 회로가 완전한지 확인하십시오.

\--- /hint \--- \--- /hints \---

\--- task \--- 이제 다음과 같이 무지개 패턴으로 무지개가 깜박이게끔 코드를 추가하세요:<video width="560" height="315" controls> <source src="resources/Scratch-GPIO-Pathways-5.mp4" type="video/mp4"> Your browser does not support the video tag, so try FireFox or Chrome. </video> 

이렇게 하기 위해서는 몇 초 동안 하나의 LED를 켜고, 다음 LED가 켜짐과 동시에 꺼줘야 합니다. \--- /task \---

\--- hints \--- \--- hint \---

Make sure your `Events`{:class="blockevents"} block matches what you are doing to test the code. In the example here, to make our rainbow blink, we have to click the green flag:

```blocks3
when flag clicked
```

\--- /hint \--- \--- hint \---

If you're stuck, make sure you are using these blocks:

```blocks3
turn LED (0 v) [off v] ::extension
wait () secs
```

\--- /hint \--- \--- hint \---

Try using this approach:

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

You will need to add blocks for all your LEDs and make sure that you're using the right GPIO pin numbers in your code.

\--- /hint \--- \--- /hints \---

\--- task \--- Make the lights blink repeatedly through the rainbow in a loop.

To loop through the rainbow pattern forever, use:

```blocks3
forever
```

\--- /task \---

\--- challenge \---

+ Make the rainbow blink in a pattern of your choice.

## \--- collapse \---

## title: Rainbow challenges

Try out the following ideas:

1) Make the LEDs blink very fast and very slow 2) Make the whole rainbow blink 3) Make pairs of LEDs light up in alternate patterns 4) Make the rainbow blink something in Morse code 5) Make the rainbow do different things in response to different events

\--- /collapse \--- \--- /challenge \---