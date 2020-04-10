## Controlla il circuito dell'arcobaleno

When your whole rainbow is set up, you can control how it is lit. Per impratichirsi nel controllo di un LED, usa Scratch per effettuare le seguenti operazioni:

\--- task \--- When you press the <kbd>P</kbd> key, make the LED turn on for two seconds and then turn off. \--- /task \---

\--- hints \--- \--- hint \--- Look in the `Control`{:class="block3control"} blocks section. \--- /hint \--- \--- hint \--- Use

```blocks3
  attendi (2) secondi
```

\--- /hint \--- \--- hint \---

```blocks3
when [p v] key pressed
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
```

\--- /hint \--- \--- /hints \---

\--- task \--- When your Scratch program starts, make your LED light up for 2 seconds and then turn off for 2 seconds. \--- /task \---

\--- hints \--- \--- hint \---

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

\--- /hint \--- \--- /hints \---

\--- task \--- Fai accendere e spegnere il LED finché il programma viene eseguito. \--- /task \---

\--- hints \--- \--- hint \--- Use

```blocks3
per sempre
```

\--- /hint \--- \--- hint \---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

\--- /hint \--- \--- /hints \---

+ Fai lampeggiare il tuo LED più velocemente.

\--- hints \--- \--- hint \--- Usa `aspetta x secondi`{:class="block3control"} per meno secondi. \--- /hint \--- \--- hint \---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (0.5) secs
turn LED (17 v) [off v] ::extension
wait (0.5) secs
```

\--- /hint \--- \--- /hints \---

Well done — you are now ready to create and control an awesome rainbow!