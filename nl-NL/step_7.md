## Verlicht je regenboog

Om er zeker van te zijn dat je regenboog werkt, test je deze eerst door de hele regenboog tegelijk te verlichten. Je maakt vervolgens code om de kleuren van de regenboog achter elkaar te laten knipperen. en dan in een patroon van jouw keuze.

\--- task \--- Voeg meer code toe om de andere LED's te besturen. Zorg ervoor dat je de juiste GPIO-pinnen toevoegt. \--- /task \---

Je regenboog zou als volgt moeten oplichten:

![Regenboog verlicht](images/rainbowlit.png)

\--- hints \--- \--- hint \--- Voeg meer `zet LED (0 v) [aan v]`{:class="block3extensions"} blokken toe in dit stuk code:

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```

\--- /hint \--- \--- hint \--- Blijf aan de onderkant blokken aan je code toevoegen tot al je LED's `aan`{:class="block3extensions"} staan.

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
turn LED (18 v) [on v] ::extension
turn LED (22 v) [on v] ::extension
```

\--- /hint \--- \--- hint \---

Als je LED's niet branden:

1) Controleer met welke GPIO-pinnen je LED's verbonden zijn, en zorg ervoor dat je ze hebt ingesteld op `aan`{:class="block3extensions"} 2) Test of de LED's werken - je kunt een LED verbindingsdraad aansluiten op **GPIO 3V3** om het te testen 3) Zorg ervoor dat het schakelcircuit op het experimenteerbord compleet is

\--- /hint \--- \--- /hints \---

\--- task \--- Voeg nu meer code toe om de regenboog in een regenboogpatroon te laten knipperen zoals hier:<video width="560" height="315" controls> <source src="resources/Scratch-GPIO-Pathways-5.mp4" type="video/mp4"> Je browser ondersteunt de video-tag niet, dus probeer Firefox of Chrome. </video> 

To do this, you will need to make one LED turn on for a couple of seconds and then turn off at the same time as the next LED turns on. \--- /task \---

\--- hints \--- \--- hint \---

Make sure your `Events`{:class="blockevents"} block matches what you are doing to test the code. In the example here, to make our rainbow blink, we have to click the green flag:

```blocks3
when flag clicked
```

\--- /hint \--- \--- hint \---

If you're stuck, make sure you are using these blocks:

```blocks3
turn LED (0 v) [off v] ::extension
wait () secs
```

\--- /hint \--- \--- hint \---

Try using this approach:

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (0.5) secs
turn LED (17 v) [off v] ::extension
turn LED (18 v) [on v] ::extension
wait (0.5) secs
turn LED (18 v) [off v] ::extension
turn LED (22 v) [on v] ::extension
```

You will need to add blocks for all your LEDs and make sure that you're using the right GPIO pin numbers in your code.

\--- /hint \--- \--- /hints \---

\--- task \--- Make the lights blink repeatedly through the rainbow in a loop.

To loop through the rainbow pattern forever, use:

```blocks3
forever
```

\--- /task \---

\--- challenge \---

+ Make the rainbow blink in a pattern of your choice.

\--- collapse \---

* * *

## title: Rainbow challenges

Try out the following ideas:

1) Make the LEDs blink very fast and very slow 2) Make the whole rainbow blink 3) Make pairs of LEDs light up in alternate patterns 4) Make the rainbow blink something in Morse code 5) Make the rainbow do different things in response to different events

\--- /collapse \--- \--- /challenge \---