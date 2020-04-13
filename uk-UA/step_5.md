## Керуй своїм електричним колом для веселки

Коли твоя веселка буде повністю зібрана, ти зможеш керувати тим, як вона світиться. Щоб трохи попрактикуватися керувати одним світлодіодом за допомогою Скретч, зроби наступне:

\--- task \--- Коли натиснуто клавішу <kbd>P</kbd> (латинську), нехай світлодіод загориться на 2 секунди, а потім згасне. \--- /task \---

\--- hints \--- \--- hint \--- Заглянь в секцію блоків `Керування`{:class="block3control"}. \--- /hint \--- \--- hint \--- Використай

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

\--- task \--- Коли твоя програма на Скретч запускається, зроби так, щоб світлодіод загорівся на 2 секунди, а потім згас на 2 секунди. \--- /task \---

\--- hints \--- \--- hint \---

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

\--- /hint \--- \--- /hints \---

\--- task \--- Зроби так, щоб під час роботи твоєї програми світлодіод постійно загорався і згасав. \--- /task \---

\--- hints \--- \--- hint \--- Використай

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

+ Зроби так, щоб твій світлодіод блимав швидше.

\--- hints \--- \--- hint \--- Використай `чекати x секунд`{:class="block3control"} для меншої кількості секунд. \--- /hint \--- \--- hint \---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (0.5) secs
turn LED (17 v) [off v] ::extension
wait (0.5) secs
```

\--- /hint \--- \--- /hints \---

Чудово, тепер ти можеш створити та керувати прекрасною веселкою!