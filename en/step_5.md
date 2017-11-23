## Test Your Circuit in Scratch

You will now connect your circuit and base rainbow colour to Scratch so you can use Scratch programming to control the LED.

+ In the last step, you connected your LED to <b>GPIO 3V3</b>. This is the pin to connect to if you are testing your LED. You now need to connect your LED to a pin you can control with Scratch (GPIO 17, for example).

+ Follow the instructions below to control your LED with Scratch.

[[[rpi-scratch-control-led]]]

+ To practice controlling your LED, complete the following challenges

--- challenge ---

1) On an event, make your LED go on for 2 seconds and then off

--- hints ---
--- hint ---
Look in the `Control`{:class="blockcontrol"} blocks
--- /hint ---
--- hint ---
Use `wait 2 secs`{:class="blockcontrol"}
--- /hint ---
--- hint ---
`when greenflag clicked`{:class="blockevents"}
`set gpio 17 to output high`{:class="blockmoreblocks"}
`wait 2 secs`{:class="blockcontrol"}
`set gpio 17 to output low`{:class="blockmoreblocks"}
--- /hint ---
--- /hints ---

2) On an event, make your LED go on for 2 seconds and then off for 2 seconds

--- hints ---
--- hint ---
`when greenflag clicked`{:class="blockevents"}
`set gpio 17 to output high`{:class="blockmoreblocks"}
`wait 2 secs`{:class="blockcontrol"}
`set gpio 17 to output low`{:class="blockmoreblocks"}
`wait 2 secs`{:class="blockcontrol"}
--- /hint ---
--- /hints ---

3) On an event, make your LED blink on and off repeatedly

--- hints ---
--- hint ---
Use `forever`{:class="control"}
--- /hint ---
--- /hints ---

4) Make your LED blink faster

--- hints ---
--- hint ---
Use `wait x secs`{:class="blockcontrol"} for less seconds
--- /hint ---
--- /hints ---

--- /challenge ---
