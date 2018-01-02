## Control your rainbow circuit

When your rainbow is set up, you can control how it is lit. In this step, you will learn how to do this using the basics of programming an LED circuit. 

+ To practice controlling your LED, complete the following:

1) When you press the <kbd>P</kbd> key, make the LED turn on for two seconds and then turn off.

--- hints ---
--- hint ---
Look in the `Control`{:class="blockcontrol"} blocks section.
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

2) When your Scratch program starts, make your LED light up for 2 seconds and then turn off for 2 seconds.

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

3) Make your LED turn on and off as long as your program runs.

--- hints ---
--- hint ---
Use
```blocks
  forever
```
--- /hint ---
--- /hints ---

4) Make your LED blink faster.

--- hints ---
--- hint ---
Use `wait x secs`{:class="blockcontrol"} for fewer seconds.
--- /hint ---
--- /hints ---
