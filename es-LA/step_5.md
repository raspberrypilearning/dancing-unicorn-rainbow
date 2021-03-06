## Controla tu circuito arcoíris

Cuando tu arcoíris esté listo, puedes controlar cómo se ilumina. Para practicar un poco el control de un LED, usa Scratch para hacer lo siguiente:

--- task --- Cuando presionas la tecla <kbd>P</kbd>, haz que el LED se encienda durante dos segundos y luego apágalo. --- /task ---

--- hints ---
 --- hint --- Mira en la sección bloques de `Control`{:class="block3control"}.
--- /hint ---
 --- hint --- Usa

```blocks3
  esperar (2) segundos
```

--- /hint --- --- hint ---

```blocks3
when [p v] key pressed
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
```

--- /hint ------ /hints ---

--- task --- Cuando tu programa de Scratch comience, haz que tu LED se encienda durante 2 segundos y luego se apague durante 2 segundos. --- /task ---

--- hints ---
 --- hint ---

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

--- /hint ------ /hints ---

--- task --- Haz que tu LED se encienda y apague mientras tu programa se está ejecutando. --- /task ---

--- hints ---
 --- hint --- Usa

```blocks3
por siempre
```

--- /hint --- --- hint ---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

--- /hint ------ /hints ---

+ Haz que tu LED parpadee más rápido.

--- hints ---
 --- hint --- Usa `esperar x segundos`{:class="block3control"} con menos segundos.
--- /hint ---
 --- hint ---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (0.5) secs
turn LED (17 v) [off v] ::extension
wait (0.5) secs
```

--- /hint ------ /hints ---

Bien hecho, ¡ahora estás listo para crear y controlar un arcoíris increíble!