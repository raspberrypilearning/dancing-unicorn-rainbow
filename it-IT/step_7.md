## Accendi il tuo arcobaleno

Per assicurarti che il tuo arcobaleno stia funzionando, lo proverai prima illuminando l'intero arcobaleno in una sola volta. Creerai quindi del codice per far lampeggiare tutti i colori del tuo arcobaleno uno dopo l'altro e poi con uno schema a tua scelta.

--- task --- Aggiungi più codice per controllare gli altri LED. Assicurati di includere i pin GPIO corretti. --- /task ---

Il tuo arcobaleno dovrebbe illuminarsi in questo modo:

![Arcobaleno acceso](images/rainbowlit.png)

--- hints ---
 --- hint --- Aggiungi altri blocchi `turn LED (0 v) [on v]`{:class="block3extensions"} in questo frammento di codice:

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```

--- /hint --- --- hint --- Continua ad aggiungere blocchi sotto al tuo codice fino a quando tutti i LED non saranno impostati su `on`{:class="block3extensions"}.

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
turn LED (18 v) [on v] ::extension
turn LED (22 v) [on v] ::extension
```

--- /hint --- --- hint ---

Se i tuoi LED non si accendono:

1) Controlla a quali pin GPIO sono collegati i tuoi LED, e assicurati di averli impostati su `on`{:class="block3extensions"} 
2) Verifica che i LED funzionino — puoi inserire il cavo jumper di un LED in **GPIO 3V3** per provarlo 
3) Assicurati che il circuito sulla breadboard sia completo

--- /hint ------ /hints ---

--- task --- Ora, aggiungi più codice per far lampeggiare l'arcobaleno con uno schema arcobaleno come questo:

<video width="560" height="315" controls> <source src="resources/Scratch-GPIO-Pathways-5.mp4" type="video/mp4"> Il tuo browser non supporta il tag video, prova FireFox o Chrome. </video> 

Per fare ciò, dovrai accendere un LED per un paio di secondi e poi spegnerlo contemporaneamente all'accensione del LED successivo. --- /task ---

--- hints ---
 --- hint ---

Assicurati che il tuo blocco `Situazioni`{:class="blockevents"} corrisponda a ciò che stai facendo per testare il codice. Nell'esempio qui, per far lampeggiare il nostro arcobaleno, dobbiamo cliccare sulla bandiera verde:

```blocks3
when flag clicked
```

--- /hint --- --- hint ---

Se sei bloccato, assicurati di utilizzare questi blocchi:

```blocks3
turn LED (0 v) [off v] ::extension
wait () secs
```

--- /hint --- --- hint ---

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

--- /hint ------ /hints ---

--- task --- Fai lampeggiare le luci ripetutamente attraverso l'arcobaleno in un ciclo.

Per ripetere lo schema dell'arcobaleno per sempre, usa:

```blocks3
forever
```

--- /task ---

--- challenge ---

+ Fai lampeggiare l'arcobaleno con uno schema a tua scelta.

--- collapse ---
---
title: Sfide arcobaleno
---

Prova le seguenti idee:

 1) Fai lampeggiare i LED molto velocemente e molto lentamente 
 2) Fai lampeggiare l'intero arcobaleno 
 3) Fai accendere coppie di LED in schemi alternati 
 4) Fai dire all'arcobaleno qualcosa in codice Morse 
 5) Fai fare all'arcobaleno cose differenti in risposta a situazioni differenti

--- /collapse --- --- /challenge ---