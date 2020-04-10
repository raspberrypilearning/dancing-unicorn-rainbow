## Prueba tu circuito en Scratch

Ahora conectarás tu circuito y tu primer color del arcoiris a Scratch, para que puedas programar un programa Scratch para controlar el LED.

\--- task \--- Abre Scratch 3 en tu Raspberry Pi.

![abrir-scratch](images/open-scratch.png) \--- /task \---

\--- task \--- Luego añade la extensión de Raspberry Pi Simple Electronics

![añadir-extensión](images/add-extension.png)

![electrónica-simple](images/simple-electronics.png) \--- /task \---

\--- task \--- En el paso anterior, conectaste tu LED al pin **3V3**. Este es el pin al que te tienes que conectar si estás probando tu LED. Ahora necesitas conectar tu LED a un pin que puedes controlar con Scratch. Mueve el cable del pin **3V3** a un nuevo pin, por ejemplo **GPIO 17**. \--- /task \---

![Mover el pin](images/movepin.png)

\--- task \--- Ahora prueba que el LED puede ser controlado usando el siguiente script simple

```blocks3
al presionar bandera verde
turn LED (17 v) [on v] :: extension
esperar (1) segundos
turn LED (17 v) [off v] :: extension
```

\--- /task \---

\--- task \--- Haz clic en la bandera verde para ejecutar tu script. El LED debería encenderse durante 1 segundo. \--- /task \---