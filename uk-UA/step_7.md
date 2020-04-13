## Засвіти свою веселку

Щоб переконатися, що твоя веселка працює, спочатку ти засвітиш її повністю. Потім ти створиш код, щоб її кольори блимали по черзі, а далі — так, як забажаєш.

\--- task \--- Додай код, щоб керувати іншими світлодіодами. Переконайся, що використовуєш правильні GPIO-піни. \--- /task \---

Твоя веселка має загорітися ось так:

![Rainbow Lit](images/rainbowlit.png)

\--- hints \--- \--- hint \--- Додай ще блоків `turn LED (0 v) [on v]`{:class="block3extensions"} до цього фрагменту коду:

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```

\--- /hint \--- \--- hint \--- Продовжуй додавати блоки в кінці свого коду, поки всі твої світлодіоди на стануть увімкненими (`on`{:class="block3extensions"}).

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
turn LED (18 v) [on v] ::extension
turn LED (22 v) [on v] ::extension
```

\--- /hint \--- \--- hint \---

Якщо твої світлодіоди не загораються:

1) Check which GPIO pins your LEDs are connected to, and make sure you have set them to `on`{:class="block3extensions"} 2) Test whether the LEDs are working — you can plug an LED's jumper wire into **GPIO 3V3** to test it 3) Make sure the circuit on the breadboard is complete

\--- /hint \--- \--- /hints \---

\--- task \--- Now, add more code to make the rainbow blink in a rainbow pattern like this:<video width="560" height="315" controls> <source src="resources/Scratch-GPIO-Pathways-5.mp4" type="video/mp4"> Your browser does not support the video tag, so try FireFox or Chrome. </video> 

To do this, you will need to make one LED turn on for a couple of seconds and then turn off at the same time as the next LED turns on. \--- /task \---

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