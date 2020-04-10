## Añade un botón

¡Ahora harás que tu arcoiris parpadee y tu unicornio baile a tiempo pulsando un botón!

### Conecta el botón

\--- task \--- Conecta tu botón a la placa de pruebas y un pin GPIO.

Haga clic a continuación para obtener instrucciones sobre cómo conectar un botón a la Raspberry Pi. Ten en cuenta que, en lugar de **GPIO 17** como las instrucciones dicen, hemos usado **GPIO 5** para el botón, **GPIO 17** ya está siendo usado por un LED.

[[[rpi-gpio-wiring-a-button]]]

Tu arcoiris debería tener un aspecto como este:

![Arcoiris con botón](images/rainbowbutton.png) \--- /task \---

### Programa el botón

\--- task \--- Usa el bloque que se muestra a continuación para que tu botón pueda hacer que el unicornio baile.

```blocks3
when button (5 v) is [pressed v] :: hat extension
```

\--- /task \---

### Controla el baile del unicornio

Por el momento, debes tener tres fragmentos de código de Scratch:

1. Código del unicornio que baila
2. Código del arcoiris parpadeante
3. Código de botón

Ahora conectarás estos trozos para que tu unicornio baile a tiempo con tu arcoiris y para que puedas controlar el arcoiris y el unicornio pulsando el botón que has añadido.

\--- task \--- Elimina todos los bloques `decir`{:class="block3looks"} en el código del botón y luego duplica este fragmento de código. \--- /task \---

\--- task \--- En tu código para el baile del unicornio, elimina el bloque `al hacer clic en la bandera`{:class="block3events"}. Toma el resto del código del unicornio y guardalo en el bloque `else`{:class="block3control"} de tu código del botón. Solo introdúcelo en **una copia** del código del botón. \--- /task \---

\--- task \--- En el código del arcoiris, elimina el bloque `al hacer clic en la bandera`{:class="block3events"} y coloca el resto del código del arcoiris en el bloque `else`{:class="block3control"} de la **otra copia** del código del botón. \--- /task \---

\--- task \--- En el espacio `si`{:class="block3control"} de ambas copias de tu código del botón, añade una acción. Podrías usar `cambiar el disfráz al primer disfráz`{:class="block3looks"}, para que a tu unicornio no se le mezclen sus movimientos de baile. \--- /task \---

\--- hints \--- \--- hint \--- Si pulsar el botón no hace que se encienda el arcoiris y el unicornio baile a tiempo, prueba a comprobar que:

1. Cada componente está conectado al pin GPIO correcto
2. Tienes las entradas y salidas correctas en tu código
3. Los tiempos coinciden en tus dos fragmentos de código
4. Has usado todos los bloques de código correctos \--- /hint \--- \--- /hints \---