## Control Your Rainbow Circuit

When your rainbow is set up, you will need to know how to control how it is lit. In this step, you will learn the basics of programming an LED circuit. 

+ To practice controlling your LED, complete the following:

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
