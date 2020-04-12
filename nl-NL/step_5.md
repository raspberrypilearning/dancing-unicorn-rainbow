## Bestuur je regenboogcircuit

Wanneer je hele regenboog is opgezet, kun je bepalen hoe deze wordt verlicht. Voor een korte oefening in het besturen van één LED, gebruik Scratch om het volgende te doen:

--- task --- Als je op de <kbd>P</kbd>-toets drukt, zet de LED twee seconden aan en schakel hem daarna uit. --- /task ---

--- hints ---
 --- hint --- Kijk in de `Besturen`{:class="block3control"} blokkensectie.
--- /hint ---
 --- hint --- Gebruik

```blocks3
  wacht (2) sec
```

--- /hint --- --- hint ---

```blocks3
when [p v] key pressed
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
```

--- /hint ------ /hints ---

--- task --- Als je Scratch programma start, laat je LED 2 seconden oplichten en zet je deze na 2 seconden weer uit. --- /task ---

--- hints ---
 --- hint ---

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

--- /hint ------ /hints ---

--- task --- Laat je LED aan en uit gaan zolang je programma loopt. --- /task ---

--- hints ---
 --- hint --- Gebruik

```blocks3
herhaal
```

--- /hint --- --- hint ---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

--- /hint ------ /hints ---

+ Laat je LED sneller knipperen.

--- hints ---
 --- hint --- Gebruik `wacht x sec.`{:class="block3control"} voor minder seconden.
--- /hint ---
 --- hint ---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (0.5) secs
turn LED (17 v) [off v] ::extension
wait (0.5) secs
```

--- /hint ------ /hints ---

Goed gedaan - je bent nu klaar om een geweldige regenboog te maken en te besturen!