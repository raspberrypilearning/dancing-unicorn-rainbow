## Add a button

You will now make your rainbow flash and your unicorn dance in time by pressing a button!

### Connect the button

+ Connect your button to the breadboard and a GPIO pin.

Click below for instructions on how to connect a button to the Raspberry Pi. Note that, instead of **GPIO 17**, we've used **GPIO 5** for the button because **GPIO 17** is already taken by an LED.
[[[rpi-gpio-wiring-a-button]]]

Your rainbow should now look something like this:
![Rainbow with Button](images/rainbowbutton.png)

### Code the button

+ Configure your button in Scratch.

[[[rpi-scratch-button]]]

### Control the rainbow unicorn dance

You can control your rainbow and unicorn by pressing a button.

At the moment, you should have three chunks of code in Scratch:
1) Unicorn dancing code
2) GPIO blinking rainbow code
3) Button configuring code

You will now connect these chunks so that you can control your rainbow and your unicorn by pressing the button.

+ Delete all of the `say ___`{:class="blocklooks"} blocks in the code for the button you just created, and then duplicate the code.

+ In your code for the unicorn dance, delete the `when flag clicked`{:class="blockevents"} block, and slot the rest of the code into the `else`{:class="blockcontrol"} block of your button code. Only slot it into one copy of the button code.

+ In the rainbow code, delete the `when flag clicked`{:class="blockevents"} block and slot the rest of the GPIO blinking rainbow code into the `else`{:class="blockcontrol"} block of the other copy of the button code.

+ In the `if`{:class="blockcontrol"} slot of both copies of your button code, add an action. You could use `switch costume to first costume`{:class="blocklooks"}, so your unicorn doesn't get its dance moves mixed up.

--- hints ---
--- hint ---
If pressing the button doesn't make the rainbow light up and the unicorn dance in time, try checking that:
1) Everything is connecting to the right GPIO pin
2) You've got the inputs and outputs right
3) The timings match for your two copies of code
4) You've used all the right code blocks
--- /hint ---
--- /hints ---

--- challenge ---

+ Have some fun with your dancing unicorn rainbow

--- collapse ---

---
title: Dancing unicorn rainbow challenges
---

Ideas:
1) Make your rainbow blink and your unicorn dance faster
2) Teach your unicorn a new dance (play around with costumes and speeds)
3) Add more buttons to make the unicorn do different dances
4) Add more `events`{:class="blockevents"} to make the unicorn do different dances
5) Make a game with your rainbow and dancing unicorn

--- /collapse ---

--- /challenge ---
