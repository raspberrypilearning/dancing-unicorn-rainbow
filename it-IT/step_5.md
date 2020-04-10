## Controlla il circuito dell'arcobaleno

Quando l'intero arcobaleno è impostato, puoi controllare come viene acceso. Per impratichirti nel controllo di un LED, usa Scratch per effettuare le seguenti operazioni:

\--- task \--- Quando premi il tasto <kbd>P</kbd>, accendi il LED per due secondi e poi spegnilo. \--- /task \---

\--- hints \--- \--- hint \--- Cerca tra i blocchi della sezione `Controllo`{:class="block3control"}. \--- /hint \--- \--- hint \--- Usa

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

\--- task \--- Quando il programma Scratch inizia, accendi il LED per 2 secondi e poi spegnilo per 2 secondi. \--- /task \---

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

\--- hints \--- \--- hint \--- Usa

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

Complimenti — ora sei pronto per creare e controllare un fantastico arcobaleno!