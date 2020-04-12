## 무지개 밝히기

무지개가 제대로 작동하는지 확인하려면 먼저 무지개 전체를 한 번에 켠 다음 테스트하세요. 그런 다음 무지개를 모든 색상에서 차례로 깜박이도록 코드를 만들고, 그 다음에는 원하는 패턴으로 깜박이게 합니다.

\--- task \--- 다른 LED를 제어하기 위해 더 많은 코드를 추가하세요. 올바른 GPIO 핀을 포함하도록 조심하세요. \--- /task \---

무지개는 다음과 같이 켜져야 합니다:

![불이 켜진 무지개](images/rainbowlit.png)

\--- hints \--- \--- hint \--- `LED (0 v) [켜기 v]`{:class="block3extensions"} 블록을 아래와 같이 추가하세요.

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```

\--- /hint \--- \--- hint \--- 아래와 같이 LED 블록을 추가해서 모든 LED를 `켜기`{:class="block3extensions"} 상태로 만드세요.

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

`이벤트`{:class="blockevents"} 블록이 코드를 테스트하기 위한 것과 동일한지 확인하세요: 이 예시에서는, 무지개를 깜박이려면 녹색 깃발을 클릭해야 합니다.

```blocks3
when flag clicked
```

\--- /hint \--- \--- hint \---

중간에 막힌다면, 다음 블록을 사용하고 있는지 확인하세요:

```blocks3
turn LED (0 v) [off v] ::extension
wait () secs
```

\--- /hint \--- \--- hint \---

이 방법을 사용해보세요:

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

모든 LED를 위한 블록을 추가하고 코드에서 올바른 GPIO 핀 번호를 사용하고 있는지 확인하세요.

\--- /hint \--- \--- /hints \---

\--- task \--- 불빛이 무지개를 따라 반복적으로 깜박이게끔 해보세요.

무지개 패턴을 영원히 반복하려면 다음을 사용하세요:

```blocks3
forever
```

\--- /task \---

\--- challenge \---

+ 무지개를 원하는 패턴으로 깜박이게 해보세요.

## \--- collapse \---

## title: 무지개 도전과제

아래의 아이디어를 시도해보세요:

1) LED가 매우 빠르거나 매우 느리게 깜박이게 하기 2) 전체 무지개가 깜박이게 하기 3) LED가 교대로 깜박이게 하기 4) 무지개가 모스 부호로 무엇인가를 깜박이게 하기 5) 무지개가 이벤트에 따라 다르게 작동하게 하기

\--- /collapse \--- \--- /challenge \---