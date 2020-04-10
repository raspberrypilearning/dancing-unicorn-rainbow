## Añade un botón

¡Ahora harás que tu arcoíris parpadee y tu unicornio bailen al mismo tiempo pulsando un botón!

### Conecta el botón

\--- task \--- Conecta tu botón a la placa de pruebas y a un pin GPIO.

Haz clic a continuación para obtener instrucciones sobre cómo conectar un botón a tu Raspberry Pi. Ten en cuenta que, en lugar de **GPIO 17** como dicen las instrucciones, hemos usado **GPIO 5** para el botón — **GPIO 17** ya está tomado por un LED.

[[[rpi-gpio-wiring-a-button]]]

Tu arcoíris ahora debería verse así:

![Arcoíris con botón](images/rainbowbutton.png) \--- /task \---

### Codifica el botón

\--- task \--- Usa el bloque que se muestra a continuación para que tu botón pueda hacer bailar al unicornio.

```blocks3
when button (5 v) is [pressed v] :: hat extension
```

\--- /task \---

### Controla el baile del unicornio

En este momento, deberías tener tres fragmentos de código Scratch:

1. Código de unicornio bailando
2. Código de arcoríris parpadeante
3. Código del botón

Ahora conectarás estos pedazos para que tu unicornio baile al ritmo de tu arcoíris, y para que puedas controlar el arcoíris y el unicornio pulsando el botón que has añadido.

\--- task \--- Elimina todos los bloques `decir`{:class="block3looks"} en el código del botón y luego duplica este fragmento de código. \--- /task \---

\--- task \--- En tu código para el baile de unicornio, elimina el bloque `al hacer clic en la bandera`{:class="block3events"}. Toma el resto del código del unicornio y ponlo en el bloque `sino`{:class="block3control"} de tu código del botón. Sólo ponlo en **una copia** del código del botón. \--- /task \---

\--- task \--- En el código del arcoíris, elimina el bloque `al hacer clic en la bandera`{:class="block3events"} y pon el resto del código del arcoíris en el bloque `sino`{:class="block3control"} de la **otro copia** del código del botón. \--- /task \---

\--- task \--- En el `si`{:class="block3control"} pon ambas copias de tu código del botón, añade una acción. Puedes usar `cambiar de disfraz al primer disfraz` {:class = "block3looks"}, para que tu unicornio no mezcle sus movimientos de baile. \--- /task \---

\--- hints \--- \--- hint \--- Si al pulsar el botón no se enciende el arcoíris y baila el unicornio al tiempo, comprueba que:

1. Cada componente está conectado al pin GPIO derecho
2. Tienes las entradas y salidas correctas en tu código
3. Los tiempos coinciden en tus dos fragmentos de código
4. Has usado todos los bloques de código correctos \--- /hint \--- \--- /hints \---