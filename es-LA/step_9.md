## Add a button

¡Ahora harás que tu arcoíris parpadee y tu unicornio baile al mismo tiempo pulsando un botón!

### Connect the button

\--- task \--- Connect your button to the breadboard and a GPIO pin.

Click below for instructions on how to connect a button to the Raspberry Pi. Note that, instead of **GPIO 17** like the instructions say, we've used **GPIO 5** for the button — **GPIO 17** is already taken by an LED.

[[[rpi-gpio-wiring-a-button]]]

Tu arcoíris ahora debería verse así:

![Rainbow with Button](images/rainbowbutton.png) \--- /task \---

### Code the button

\--- task \--- Use the block shown below so that your button can make the unicorn dance.

```blocks3
when button (5 v) is [pressed v] :: hat extension
```

\--- /task \---

### Control the unicorn dance

At the moment, you should have three chunks of Scratch code:

1. Dancing unicorn code
2. Blinking rainbow code
3. Button code

You will now connect these chunks so that your unicorn dances in time to your rainbow, and so that you can control the rainbow and unicorn by pressing the button you've added.

\--- task \--- Elimina todos los bloques `decir`{:class="block3looks"} en el código del botón y luego duplica este fragmento de código. \--- /task \---

\--- task \--- En tu código para el baile de unicornio, elimina el bloque `al hacer clic en la bandera`{:class="block3events"}. Toma el resto del código del unicornio y ponlo en el bloque `sino`{:class="block3control"} de tu código del botón. Sólo ponlo en **una copia** del código del botón. \--- /task \---

\--- task \--- En el código del arcoíris, elimina el bloque `al hacer clic en la bandera`{:class="block3events"} y pon el resto del código del arcoíris en el bloque `sino`{:class="block3control"} de la **otro copia** del código del botón. \--- /task \---

\--- task \--- In the `if`{:class="block3control"} slot of both copies of your button code, add an action. You could use `switch costume to first costume`{:class="block3looks"}, so your unicorn doesn't get its dance moves mixed up. \--- /task \---

\--- hints \--- \--- hint \--- Si al pulsar el botón no se enciende el arcoíris y el unicornio baila al tiempo, comprueba que:

1. Every component is connected to the right GPIO pin
2. You've got the inputs and outputs right in your code
3. The timings match for your two chunks of code
4. You've used all the right code blocks \--- /hint \--- \--- /hints \---