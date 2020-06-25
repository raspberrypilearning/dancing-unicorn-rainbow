## Light your rainbow

Para asegurarte de que tu arcoíris esté funcionando, primero lo probarás encendiendo todo el arcoíris a la vez. Luego crearás el código para hacer que el arcoíris parpadee en todos sus colores, uno tras otro, y luego en un patrón de tu elección.

\--- task \--- Añade más código para controlar los otros LEDs. Asegúrate de incluir los pines GPIO correctos. \--- /task \---

Tu arcoíris debería iluminarse así:

![Rainbow Lit](images/rainbowlit.png)

\--- hints \--- \--- hint \--- Add more `turn LED (0 v) [on v]`{:class="block3extensions"} blocks in this chunk of code:

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```

\--- /hint \--- \--- hint \--- Keep adding blocks at the bottom of your code until all your LEDs are set to `on`{:class="block3extensions"}.

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
turn LED (18 v) [on v] ::extension
turn LED (22 v) [on v] ::extension
```

\--- /hint \--- \--- hint \---

Si tus LEDs no se iluminan:

1) Comprueba a qué pin GPIO están conectados tus LEDs y asegúrate de que las has establecido en `on`{:class="block3extensions"} 2) Prueba si los LEDs están funcionando — puedes conectar un cable de puente de un LED a **GPIO 3V3** para probarlo 3) Asegúrate de que el circuito en la placa de pruebas esté completo

\--- /hint \--- \--- /hints \---

\--- task \--- Now, add more code to make the rainbow blink in a rainbow pattern like this:<video width="560" height="315" controls> <source src="resources/Scratch-GPIO-Pathways-5.mp4" type="video/mp4"> Your browser does not support the video tag, so try FireFox or Chrome. </video> 

To do this, you will need to make one LED turn on for a couple of seconds and then turn off at the same time as the next LED turns on. \--- /task \---

\--- hints \--- \--- hint \---

Make sure your `Events`{:class="blockevents"} block matches what you are doing to test the code. En el ejemplo aquí, para hacer que nuestro arcoíris parpadee, tenemos que hacer clic en la bandera verde:

```blocks3
when flag clicked
```

\--- /hint \--- \--- hint \---

Si estás atascado, asegúrate de usar estos bloques:

```blocks3
turn LED (0 v) [off v] ::extension
wait () secs
```

\--- /hint \--- \--- hint \---

Intenta usar este método:

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

Necesitarás añadir bloques para todos tus LEDs y asegurarte de que estás usando los números de pin GPIO correctos en tu código.

\--- /hint \--- \--- /hints \---

\--- task \--- Haz que las luces parpadeen repetidamente a través del arcoíris en un bucle.

Para hacer un bucle a través del patrón arcoíris por siempre, usa:

```blocks3
forever
```

\--- /task \---

\--- challenge \---

+ Make the rainbow blink in a pattern of your choice.

## \--- collapse \---

## title: Desafíos arcoiris

Prueba las siguientes ideas:

1) Make the LEDs blink very fast and very slow 2) Make the whole rainbow blink 3) Make pairs of LEDs light up in alternate patterns 4) Make the rainbow blink something in Morse code 5) Make the rainbow do different things in response to different events

\--- /collapse \--- \--- /challenge \---