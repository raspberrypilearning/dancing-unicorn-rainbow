## Ilumina tu arcoíris

Para asegurarte de que tu arcoíris esté funcionando, primero lo probarás encendiendo todo el arcoíris a la vez. Luego crearás el código para hacer que el arcoíris parpadee en todos sus colores, uno tras otro, y luego en un patrón de tu elección.

\--- task \--- Añade más código para controlar los otros LEDs. Asegúrate de incluir los pines GPIO correctos. \--- /task \---

Tu arcoíris debería iluminarse así:

![Arcoíris iluminado](images/rainbowlit.png)

\--- hints \--- \--- hint \--- Añade más bloques `turn LED (0 v) [on v]`{:class="block3extensions"} en este fragmento de código:

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```

\--- /hint \--- \--- hint \--- Sigue agregando bloques en la parte inferior de tu código hasta que todos sus LEDs se establezcan en `on`{:class="block3extensions"}.

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

\--- task \--- Ahora, añade más código para hacer que el arcoíris parpadee en un patrón de arcoíris como este:<video width="560" height="315" controls> <source src="resources/Scratch-GPIO-Pathways-5.mp4" type="video/mp4"> Tu navegador no soporta la etiqueta de vídeo, prueba FireFox o Chrome. </video> 

Para hacer esto, tendrás que hacer que un LED se encienda durante un par de segundos y luego apagarlo al mismo tiempo que el siguiente LED se enciende. \--- /task \---

\--- hints \--- \--- hint \---

Asegúrate de que el bloque `Eventos`{:class="blockevents"} coincide con lo que estás haciendo para probar el código. En el ejemplo aquí, para hacer que nuestro arcoíris parpadee, tenemos que hacer clic en la bandera verde:

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

+ Haz que el arcoíris parpadee en el patrón que elijas.

## \--- collapse \---

## title: Desafíos arcoiris

Prueba las siguientes ideas:

1) Haz que los LED parpadeen muy rápido y muy lento 2) Haz que todo el arcoiris parpadee 3) Haz que los pares de LED se enciendan en patrones alternativos 4) Haz que el arcoiris parpadee algo en código Morse 5) Haz que el arcoiris haga diferentes cosas en respuesta a diferentes eventos

\--- /collapse \--- \--- /challenge \---