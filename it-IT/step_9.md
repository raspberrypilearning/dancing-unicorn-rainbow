## Aggiungi un pulsante

Ora farai lampeggiare il tuo arcobaleno e il tuo unicorno ballare a tempo premendo un pulsante!

### Collega il pulsante

\--- task \--- Collega il tuo pulsante alla breadboard e a un pin GPIO.

Clicca qui sotto per le istruzioni su come collegare un pulsante al Raspberry Pi. Nota che, invece di **GPIO 17** come dicono le istruzioni abbiamo usato **GPIO 5** per il pulsante — **GPIO 17** è già stato utilizzato per uno dei LED.

[[[rpi-gpio-wiring-a-button]]]

Il tuo arcobaleno ora dovrebbe assomigliare a questo:

![Arcobaleno con pulsante](images/rainbowbutton.png) \--- /task \---

### Programma il pulsante

\--- task \--- Usa il blocco mostrato sotto in modo che il tuo pulsante possa far ballare l'unicorno.

```blocks3
when button (5 v) is [pressed v] :: hat extension
```

\--- /task \---

### Controlla la danza dell'unicorno

Al momento, dovresti avere tre frammenti di codice Scratch:

1. Codice unicorno danzante
2. Codice arcobaleno lampeggiante
3. Codice pulsante

Ora collegherai questi frammenti in modo che il tuo unicorno balli a tempo col tuo arcobaleno e in modo da poter controllare l'arcobaleno e l'unicorno premendo il pulsante che hai aggiunto.

\--- task \--- Elimina tutti i blocchi `dire`{:class="block3looks"} nel codice del pulsante e poi duplica questo pezzo di codice. \--- /task \---

\--- task \--- Nel tuo codice per la danza dell'unicorno, elimina il blocco `quando fai clic sulla bandiera verde`{:class="block3events"}. Prendi il resto del codice di unicorno e mettilo nel blocco `altrimenti`{:class="block3control"} del codice del pulsante. Only slot it into **one copy** of the button code. \--- /task \---

\--- task \--- In the rainbow code, delete the `when flag clicked`{:class="block3events"} block and slot the rest of the rainbow code into the `else`{:class="block3control"} block of the **other copy** of the button code. \--- /task \---

\--- task \--- In the `if`{:class="block3control"} slot of both copies of your button code, add an action. You could use `switch costume to first costume`{:class="block3looks"}, so your unicorn doesn't get its dance moves mixed up. \--- /task \---

\--- hints \--- \--- hint \--- If pressing the button doesn't make the rainbow light up and the unicorn dance in time, try checking that:

1. Every component is connected to the right GPIO pin
2. You've got the inputs and outputs right in your code
3. The timings match for your two chunks of code
4. You've used all the right code blocks \--- /hint \--- \--- /hints \---