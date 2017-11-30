## Control Your Rainbow Dancing Unicorn with a Button

You will now make your unicorn dance when the rainbow is flashing, by pressing a button!

### Connect the Button

+ Connect your button to the breadboard and GPIO

Here are instructions on how to connect a button to the Raspberry Pi:
[[[rpi-gpio-wiring-a-button]]]

Instead of **GPIO 17** we've used **GPIO 5** for the button.

Your rainbow should now look something like this:
DIAGRAM

### Code the Button

+ Configure your button in Scratch

[[[rpi-scratch-button]]]

### Control Rainbow Unicorn Dance

+ Control your rainbow and unicorn by pressing the button

You should now have 3 different chunks of code in Scratch:
1) Unicorn dancing code
2) GPIO blinking rainbow code
3) Button configuring code

Delete all of the `say ___`{:class="blocklooks"} blocks in your button configuring code (from the last step), and then duplicate the code.

Slot your unicorn dancing code into `else`{:class="blockcontrol"} of the button configuring code.
Slot your GPIO blinking rainbow code into `else`{:class="blockcontrol"} of the other button configuring code.

In the `if`{:class="blockcontrol"} slots of your code, add an action. I suggest `switch costume to first costume`{:class="blocklooks"} so your unicorn doesn't get its dance moves mixed up.

--- hint ---
If pressing the button doesn't make your rainbow light, and unicorn dance, try:
1) Making sure everything is connecting to the right GPIO
2) Making sure you've got inputs and outputs right
3) Making sure timings match for your two chunks of code
4) Double checking your code
--- /hint ---


--- challenge ---

+ Have some fun with your dancing unicorn rainbow

Ideas:
1) Make your rainbow blink and unicorn dance faster.
2) Teach your unicorn a new dance (play around with costumes and speeds).
3) Add more buttons to make the unicorn do different dances.
4) Add more `events`{:class="blockevents"} to make the unicorn do different dances.
5) Make a game with your rainbow and dancing unicorn.

--- /challenge ---
