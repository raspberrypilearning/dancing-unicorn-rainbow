## Light your rainbow

Per assicurarti che il tuo arcobaleno stia funzionando, lo proverai prima illuminando l'intero arcobaleno in una sola volta. Creerai quindi del codice per far lampeggiare tutti i colori del tuo arcobaleno uno dopo l'altro e poi con uno schema a tua scelta.

\--- task \--- Aggiungi più codice per controllare gli altri LED. Assicurati di includere i pin GPIO corretti. \--- /task \---

Il tuo arcobaleno dovrebbe illuminarsi in questo modo:

![Rainbow Lit](images/rainbowlit.png)

\--- hints \--- \--- hint \--- Aggiungi altri blocchi `turn LED (0 v) [on v]`{:class="block3extensions"} in questo frammento di codice:

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```

\--- /hint \--- \--- hint \--- Continua ad aggiungere blocchi sotto al tuo codice fino a quando tutti i LED non saranno impostati su `on`{:class="block3extensions"}.

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
turn LED (18 v) [on v] ::extension
turn LED (22 v) [on v] ::extension
```

\--- /hint \--- \--- hint \---

If your LEDs are not lighting:

1) Check which GPIO pins your LEDs are connected to, and make sure you have set them to `on`{:class="block3extensions"} 2) Test whether the LEDs are working — you can plug an LED's jumper wire into **GPIO 3V3** to test it 3) Make sure the circuit on the breadboard is complete

\--- /hint \--- \--- /hints \---

\--- task \--- Ora, aggiungi più codice per far lampeggiare l'arcobaleno con uno schema come questo:<video width="560" height="315" controls> <source src="resources/Scratch-GPIO-Pathways-5.mp4" type="video/mp4"> Il tuo browser non supporta il tag video, prova FireFox o Chrome. </video> 

Per fare ciò, dovrai accendere un LED per un paio di secondi e poi spegnerlo contemporaneamente all'accensione del LED successivo. \--- /task \---

\--- hints \--- \--- hint \---

Make sure your `Events`{:class="blockevents"} block matches what you are doing to test the code. In the example here, to make our rainbow blink, we have to click the green flag:

```blocks3
when flag clicked
```

\--- /hint \--- \--- hint \---

Se sei bloccato, assicurati di utilizzare questi blocchi:

```blocks3
turn LED (0 v) [off v] ::extension
wait () secs
```

\--- /hint \--- \--- hint \---

Prova a utilizzare questo approccio:

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

Dovrai aggiungere blocchi per tutti i tuoi LED e assicurarti di utilizzare i giusti numeri di pin GPIO nel tuo codice.

\--- /hint \--- \--- /hints \---

\--- task \--- Make the lights blink repeatedly through the rainbow in a loop.

Per ripetere lo schema dell'arcobaleno per sempre, usa:

```blocks3
forever
```

\--- /task \---

\--- challenge \---

+ Fai lampeggiare l'arcobaleno con uno schema a tua scelta.

\--- collapse \---

* * *

## title: Sfide arcobaleno

Prova le seguenti idee:

1) Make the LEDs blink very fast and very slow 2) Make the whole rainbow blink 3) Make pairs of LEDs light up in alternate patterns 4) Make the rainbow blink something in Morse code 5) Make the rainbow do different things in response to different events

\--- /collapse \--- \--- /challenge \---