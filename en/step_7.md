## Light the Rainbow

Test your rainbow in Scratch by lighting the whole rainbow at once.

+ Add more code to control the other LEDs. Make sure you have the GPIO Pins selected.

Your rainbow should light up like this:
![Rainbow Lit](images/rainbowlit.png)

--- hints ---
--- hint ---
Add more `set gpio () to output high`{:class="blockmoreblocks"} blocks at the end of this code:
```blocks  
	when flag clicked
	set gpio (17) to [output high v] :: extension
```
--- /hint ---
--- hint ---
Keep adding blocks to the bottom of your code until all your GPIO pins are set to `output high`{:class="blockmoreblocks"}
```blocks  
	when flag clicked
	set gpio (17) to [output high v] :: extension
  set gpio (18) to [output high v] :: extension
  set gpio (22) to [output high v] :: extension
```
...
--- /hint ---
--- hint ---

If your LEDs are not lighting:

1) Make sure you look at which GPIO your LEDs are connected to and have set them in Scratch to `output high`{:class="blockmoreblocks"}
2) Check that the LED is working (you can plug the LED's jumper wire into **GPIO 3V3** to test)
3) Make sure the circuit on the breadboard is complete.

--- /hint ---
--- /hints ---

+ Now, make the rainbow blink in a rainbow pattern like this:

<video width="560" height="315" controls>
<source src="resources/Scratch-GPIO-Pathways-5.mp4" type="video/mp4">
Your browser does not support the video tag, try FireFox or Chrome
</video>

To do this, you will need to make one LED turn on for a couple of seconds, and then turn off at the same time as the next LED turns on. You will have to add more code to do this.

--- hints ---
--- hint ---

Make sure your `Events`{:class="blockevents"} block matches what you are doing to test the code.
For example, to make our rainbow blink, we click the green flag:
```blocks
  when flag clicked
```
--- /hint ---
--- hint ---

If you're stuck, make sure you are using these blocks
```blocks
	set gpio () to [output low v] :: extension
  wait () secs
```

--- /hint ---
--- hint ---

Try using this approach:
```blocks  
	when flag clicked
	set gpio (17) to [output high v] :: extension
  wait (0.5) secs
  set gpio (17) to [output low v] :: extension
  set gpio (18) to [output high v] :: extension
  wait (0.5) secs
  set gpio (18) to [output low v] :: extension
  set gpio (22) to [output high v] :: extension
```
...

--- /hint ---
--- /hints ---

+ Make the lights blink repeatedly through the rainbow in a loop

To loop through the rainbow pattern forever, use:
```blocks
forever
```

--- challenge ---

+ Make the rainbow blink in a pattern of your choice.

--- collapse ---

---
title: Rainbow Challenges
---

Ideas:
  1) Make the rainbow go very fast and very slow
  2) Make all LEDs in the rainbow blink together
  3) Make pairs of LEDs light in alternate patters
  4) Make the rainbow blink something in Morse Code
  5) Make the rainbow do different things on different events

--- /collapse ---
--- /challenge ---
