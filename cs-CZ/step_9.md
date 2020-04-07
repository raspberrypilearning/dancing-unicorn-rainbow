## Add a button

You will now make your rainbow flash and your unicorn dance in time by pressing a button!

### Connect the button

\--- task \--- Connect your button to the breadboard and a GPIO pin.

Click below for instructions on how to connect a button to the Raspberry Pi. Note that, instead of **GPIO 17** like the instructions say, we've used **GPIO 5** for the button — **GPIO 17** is already taken by an LED.

[[[rpi-gpio-wiring-a-button]]]

Your rainbow should now look something like this:

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

\--- task \--- Delete all of the `say`{:class="block3looks"} blocks in the code for the button, and then duplicate this chunk of code. \--- /task \---

\--- task \--- In your code for the unicorn dance, delete the `when flag clicked`{:class="block3events"} block. Take the rest of the unicorn code, and slot it into the `else`{:class="block3control"} block of your button code. Only slot it into **one copy** of the button code. \--- /task \---

\--- task \--- In the rainbow code, delete the `when flag clicked`{:class="block3events"} block and slot the rest of the rainbow code into the `else`{:class="block3control"} block of the **other copy** of the button code. \--- /task \---

\--- task \--- In the `if`{:class="block3control"} slot of both copies of your button code, add an action. You could use `switch costume to first costume`{:class="block3looks"}, so your unicorn doesn't get its dance moves mixed up. \--- /task \---

\--- hints \--- \--- hint \--- If pressing the button doesn't make the rainbow light up and the unicorn dance in time, try checking that:

1. Every component is connected to the right GPIO pin
2. You've got the inputs and outputs right in your code
3. The timings match for your two chunks of code
4. You've used all the right code blocks \--- /hint \--- \--- /hints \---