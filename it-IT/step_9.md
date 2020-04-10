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

\--- task \--- Nel tuo codice per la danza dell'unicorno, elimina il blocco `quando fai clic sulla bandiera verde`{:class="block3events"}. Prendi il resto del codice di unicorno e mettilo nel blocco `altrimenti`{:class="block3control"} del codice del pulsante. Inseriscilo in **una copia** del codice pulsante. \--- /task \---

\--- task \--- Nel codice dell'arcobaleno, elimina il blocco `quando si clicca sulla bandiera verde`{:class="block3events"} e inserisci il resto del codice dell'arcobaleno nel blocco `altrimenti`{:class="block3control"} dell'**altra copia** del codice del pulsante. \--- /task \---

\--- task \--- Nello slot `se`{:class="block3control"} di entrambe le copie del tuo codice del pulsante, aggiungi un'azione. Puoi usare `passa al primo costume`{:class="block3looks"}, così i passi di danza del tuo unicorno non si mischieranno. \--- /task \---

\--- hints \--- \--- hint \--- Se premendo il pulsante non si accende l'arcobaleno e l'unicorno non balla a tempo, prova a verificare che:

1. Ogni componente sia collegato al pin GPIO giusto
2. Hai impostato gli input e gli output corretti nel tuo codice
3. I tempi utilizzati nei tuoi due pezzi di codice corrispondano
4. Hai usato tutti i blocchi di codice corretti \--- /hint \--- \--- /hints \---