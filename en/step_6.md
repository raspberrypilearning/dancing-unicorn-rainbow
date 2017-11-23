## Build Your Rainbow

You are now ready to create an awesome rainbow! In this step, you will assemble your rainbow and program the LEDs to blink in a rainbow pattern.


+ Find all the LEDs you are going to use and make sure you also have the same amount of jumper wires and resistors


+ Rearrange the circuit you already have to make room for other colours of the rainbow.

(Diagram)

To make sure your rainbow is bright and not covered by too many jumper wires, each LED must share the same ground.

The breadboard looks like this inside:
![Breadboard Cross-Section](images/breadboardxsection.png)

To ground the whole rainbow with one wire, connect the ground to one of the rails and then make sure all the transistors connect to the same rail:

(diagram)

+ Now add all of your LEDs, LED jumper wires, and transistors to the breadboard in a colour arrangement of your choice.

Make sure to leave room for a button at the end.
It will help to use the same colour jumper wire as your LED if you are using many different colours.

Your rainbow should look similar to this one:

(diagram)

+ Test your rainbow in Scratch by lighting the whole rainbow at once

--- hints ---
--- hint ---

These are the blocks for the rainbow in the last diagram:
`when greenflag clicked`{:class="blockevents"}
`set gpio 17 to output high`{:class="blockmoreblocks"}
`set gpio 18 to output high`{:class="blockmoreblocks"}
`set gpio 22 to output high`{:class="blockmoreblocks"}
`set gpio 23 to output high`{:class="blockmoreblocks"}
`set gpio 9 to output high`{:class="blockmoreblocks"}
`set gpio 25 to output high`{:class="blockmoreblocks"}
`set gpio 11 to output high`{:class="blockmoreblocks"}

--- /hint ---
--- hint ---

If your LEDs are not lighting:

1) Make sure you look at which GPIO your LEDs are connected to and have set them in Scratch to `output high`{:class="blockmoreblocks"}
2) Check that the LED is working (you can plug the LED's jumper wire into GPIO 3V3 to test)
3) Make sure the circuit on the breadboard is complete.

--- /hint ---
--- /hints ---

+ Make the rainbow blink in a rainbow pattern

(screenshot, pic, video?)

--- challenge ---

+ Make the rainbow blink in a pattern of your choice.

Ideas:
  1) Make the rainbow go very fast and very slow
  2) Make all LEDs in the rainbow blink together
  3) Make pairs of LEDs light in alternate patters
  4) Make the rainbow blink something in Morse Code
  5) Make the rainbow do different things on different events

--- /challenge ---
