## Test Your Circuit in Scratch

You will now connect your circuit and base rainbow colour to Scratch so you can use Scratch programming to control the LED.

+ Open up Scratch 2 on your Raspberry Pi. Reminder: this will not work with the online version or with Sratch 1.4.

+ In the last step, you connected your LED to **GPIO 3V3**. This is the pin to connect to if you are testing your LED. You now need to connect your LED to a pin you can control with Scratch (for example, **GPIO 17**).

+ Follow these instructions to control your LED with Scratch:

[[[rpi-scratch-add-pi-gpio]]]

[[[rpi-scratch-control-led]]]

+ To practice controlling your LED, complete the following:

--- challenge ---


1) When you press the P key, make the LED turn on for 2 seconds then turn off

--- hints ---
--- hint ---
Look in the `Control`{:class="blockcontrol"} blocks
--- /hint ---
--- hint ---
Use
```blocks
  wait (2) secs
```
--- /hint ---
--- hint ---
```blocks  
	when [p v] key pressed
	set gpio (17) to [output high v] :: extension
	wait (2) secs
  set gpio (17) to [output low v] :: extension
```
--- /hint ---
--- /hints ---

2) On any event, make your LED go on for 2 seconds and then off for 2 seconds

--- hints ---
--- hint ---
```blocks  
	when flag clicked
	set gpio (17) to [output high v] :: extension
	wait (2) secs
  set gpio (17) to [output low v] :: extension
  wait (2) secs
```
--- /hint ---
--- /hints ---

3) On any event, make your LED blink on and off repeatedly

--- hints ---
--- hint ---
Use
```blocks
  forever
```
--- /hint ---
--- /hints ---

4) Make your LED blink faster

--- hints ---
--- hint ---
Use `wait x secs`{:class="blockcontrol"} for less seconds
--- /hint ---
--- /hints ---


--- /challenge ---
