## Prueba tu circuito en Scratch

Ahora conectarás tu circuito y el primer color del arcoíris a Scratch, de modo que puedas crear un programa Scratch para controlar el LED.

\--- task \--- Abre Scratch 3 en tu Raspberry Pi.

![abrir-scratch](images/open-scratch.png) \--- /task \---

\--- task \--- Luego añade la extensión de Raspberry Pi Simple Electronics (electrónica-simple)

![añadir-extensión](images/add-extension.png)

![electrónica-simple](images/simple-electronics.png) \--- /task \---

\--- task \--- In the previous step, you connected your LED to pin **3V3**. This is the pin to connect to if you are testing your LED. You now need to connect your LED to a pin you can control with Scratch. Move the wire from pin **3V3** to a new pin, for example **GPIO 17**. \--- /task \---

![Mover el pin](images/movepin.png)

\--- task \--- Now test that the LED can be controlled using the following simple script

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (1) secs
turn LED (17 v) [off v] ::extension
```

\--- /task \---

\--- task \--- Click the green flag to run your script. El LED debería encenderse durante 1 segundo. \--- /task \---