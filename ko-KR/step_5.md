## 무지개 회로 제어하기

무지개 회로가 모두 구성된 다음, 어떻게 불을 밝힐 것인지를 제어할 수 있습니다. 하나의 LED를 제어하는 작은 연습을 위해, 스크래치를 사용하여 다음을 수행하세요:

--- task --- <kbd>P</kbd> 키를 누르면 LED가 2 초 동안 켜졌다가 꺼지게 해보세요. --- /task ---

--- hints ---
 --- hint --- `제어`{:class="block3control"} 블록 섹션을 클릭하세요.
--- /hint ---
 --- hint ---

```blocks3
  (2) 초 기다리기
```

--- /hint --- --- hint ---

```blocks3
when [p v] key pressed
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
```

--- /hint ------ /hints ---

--- task --- Scratch 프로그램이 시작되면 LED를 2초 동안 켜고 2초 동안 끄게 만들어보세요. --- /task ---

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

--- task --- 프로그램이 실행되는 동안 LED를 켜고 끄게 하세요. --- /task ---

--- hints --- --- hint --- 사용

```blocks3
무한 반복하기
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

+ LED가 더 빨리 깜박이게 하세요.

--- hints ---
 --- hint --- 더 짧은 시간을 위해 `( ) 초 기다리기`{:class="block3control"}를 사용하세요.
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

잘했어요! 이제 멋진 무지개를 만들고 제어할 준비가 되었습니다!