## Додай кнопку

А зараз ти зробиш, щоб веселка блимала, а єдиноріг танцював в ритм, за натисканням кнопки!

### Приєднай кнопку

\--- task \--- Приєднай кнопку до макетної плати та GPIO-піна.

Клацни нижче, щоб переглянути інструкції про те, як приєднати кнопку до Raspberry Pi. Зверни увагу, що замість **GPIO 17** як сказано в інструкції, ми будемо використовувати для кнопки **GPIO 5**, бо **GPIO 17** вже зайнятий світлодіодом.

[[[rpi-gpio-wiring-a-button]]]

Тепер твоя веселка має виглядати приблизно так:

![Rainbow with Button](images/rainbowbutton.png) \--- /task \---

### Код для кнопки

\--- task \--- Use the block shown below so that your button can make the unicorn dance.

```blocks3
when button (5 v) is [pressed v] :: hat extension
```

\--- /task \---

### Керуй танцем єдинорога

Наразі в тебе має бути три фрагменти коду на Скретч:

1. Код для танцюючого єдинорога
2. Код для блимаючої веселки
3. Код для кнопки

You will now connect these chunks so that your unicorn dances in time to your rainbow, and so that you can control the rainbow and unicorn by pressing the button you've added.

\--- task \--- Delete all of the `say`{:class="block3looks"} blocks in the code for the button, and then duplicate this chunk of code. \--- /task \---

\--- task \--- In your code for the unicorn dance, delete the `when flag clicked`{:class="block3events"} block. Take the rest of the unicorn code, and slot it into the `else`{:class="block3control"} block of your button code. Only slot it into **one copy** of the button code. \--- /task \---

\--- task \--- In the rainbow code, delete the `when flag clicked`{:class="block3events"} block and slot the rest of the rainbow code into the `else`{:class="block3control"} block of the **other copy** of the button code. \--- /task \---

\--- task \--- In the `if`{:class="block3control"} slot of both copies of your button code, add an action. You could use `switch costume to first costume`{:class="block3looks"}, so your unicorn doesn't get its dance moves mixed up. \--- /task \---

\--- hints \--- \--- hint \--- If pressing the button doesn't make the rainbow light up and the unicorn dance in time, try checking that:

1. Every component is connected to the right GPIO pin
2. You've got the inputs and outputs right in your code
3. The timings match for your two chunks of code
4. You've used all the right code blocks \--- /hint \--- \--- /hints \---