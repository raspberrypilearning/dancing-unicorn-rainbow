## Controla tu circuito arcoiris

Cuando tu arcoiris esté listo, puedes controlar cómo se ilumina. Para practicar un poco el control de un LED, usa Scratch para hacer lo siguiente:

\--- task \--- Cuando presionas la tecla <kbd>P</kbd>, haz que el LED se encienda durante dos segundos y luego apágalo. \--- /task \---

\--- hints \--- \--- hint \--- Mira en la sección bloques de `Control`{:class="block3control"}. \--- /hint \--- \--- hint \--- Usar

```blocks3
  esperar (2) segundos
```

\--- /hint \--- \--- hint \---

```blocks3
al presionar tecla [p v]
turn LED (17 v) [on v] :: extension
esperar (2) segundos
turn LED (17 v) [off v] :: extension
```

\--- /hint \--- \--- /hints \---

\--- task \--- Cuando tu programa de Scratch comience, haz que tu LED se encienda durante 2 segundos y luego se apague durante 2 segundos. \--- /task \---

\--- hints \--- \--- hint \---

```blocks3
al presionar bandera verde
turn LED (17 v) [on v] :: extension
esperar (2) segundos
turn LED (17 v) [off v] :: extension
esperar (2) segundos
```

\--- /hint \--- \--- /hints \---

\--- task \--- Haz que tu LED se encienda y apague mientras tu programa se está ejecutando. \--- /task \---

\--- hints \--- \--- hint \--- Usar

```blocks3
por siempre
```

\--- /hint \--- \--- hint \---

```blocks3
al presionar bandera verde
por siempre 
 turn LED (17 v) [on v] :: extension
 esperar (2) segundos
 turn LED (17 v) [off v] :: extension
 esperar (2) segundos
end
```

\--- /hint \--- \--- /hints \---

+ Haz que tu LED parpadee más rápido.

\--- hints \--- \--- hint \--- Usa `esperar x segundos`{:class="block3control"} con menos segundos. \--- /hint \--- \--- hint \---

```blocks3
al presionar bandera verde
por siempre 
 turn LED (17 v) [on v] :: extension
 esperar (0.5) segundos
 turn LED (17 v) [off v] :: extension
 esperar (0.5) segundos
end
```

\--- /hint \--- \--- /hints \---

Bien hecho, ¡ahora estás listo para crear y controlar un arcoiris increíble!