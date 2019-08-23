## Control your rainbow circuit

When your whole rainbow is set up, you can control how it is lit. For a little practice of controlling one LED, use Scratch to do the following:

--- task ---
When you press the <kbd>P</kbd> key, make the LED turn on for two seconds and then turn off.
--- /task ---

--- hints ---
--- hint ---
Look in the `Control`{:class="block3control"} blocks section.
--- /hint ---
--- hint ---
Use
```blocks3
  wait (2) secs
```
--- /hint ---
--- hint ---
```blocks3
when [p v] key pressed
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
```
--- /hint ---
--- /hints ---

--- task ---
When your Scratch program starts, make your LED light up for 2 seconds and then turn off for 2 seconds.
--- /task ---

--- hints ---
--- hint ---
```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```
--- /hint ---
--- /hints ---

--- task ---
Make your LED turn on and off as long as your program runs.
--- /task ---

--- hints ---
--- hint ---
Use
```blocks3
forever
```
--- /hint ---
--- /hints ---

+ Make your LED blink faster.

--- hints ---
--- hint ---
Use `wait x secs`{:class="block3control"} for fewer seconds.
--- /hint ---
--- /hints ---

Well done — you are now ready to create and control an awesome rainbow!
