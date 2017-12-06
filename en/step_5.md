## Test Your Circuit in Scratch

You will now connect your circuit and base rainbow colour to Scratch so you can use Scratch programming to control the LED.

+ Open up Scratch 2 on your Raspberry Pi. Reminder: this will not work with the online version or with Sratch 1.4.

+ In the last step, you connected your LED to **GPIO 3V3**. This is the pin to connect to if you are testing your LED. You now need to connect your LED to a pin you can control with Scratch (for example, **GPIO 17**).

+ Follow these instructions to control your LED with Scratch:

[[[rpi-scratch-add-pi-gpio]]]

[[[rpi-scratch-control-led]]]

+ To practice controlling your LED, complete these challenges:

--- challenge ---

--- collapse ---

---
title: Important Challenges
---

1) When you press the P key, make the LED turn on for 2 seconds then turn off

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
```blocks  
	when P key clicked
	set gpio (17) to [output high v]
	wait (2) secs
  set gpio (17) to [output low v]
```

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
```blocks  
	when flag clicked
	set gpio (17) to [output high v]
	wait (2) secs
  set gpio (17) to [output low v]
  wait (2) secs
```
--- /hint ---
--- /hints ---

3) On an event, make your LED blink on and off repeatedly

--- hints ---
--- hint ---
Use `forever`{:class="blockcontrol"}
--- /hint ---
--- /hints ---

4) Make your LED blink faster

--- hints ---
--- hint ---
Use `wait x secs`{:class="blockcontrol"} for less seconds
--- /hint ---
--- /hints ---

--- /collapse ---

--- /challenge ---
