## Controle o seu circuito arco-íris

Quando todo o seu arco-íris estiver configurado, você pode controlar como ele é aceso. Para um pouco de prática para controlar um LED, use o Scratch para fazer o seguinte:

\--- task \--- Quando você pressionar a tecla <kbd>P</kbd>, acenda o LED por dois segundos e depois apague. \--- /task \---

\--- hints \--- \--- hint \--- Olhe na seção de blocos `Controle`{:class="block3control"}. \--- /hint \--- \--- hint \--- Use

```blocks3
  espere (2) seg
```

\--- /hint \--- \--- hint \---

```blocks3
when [p v] key pressed
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
```

\--- /hint \--- \--- /hints \---

\--- task \--- Quando o seu programa Scratch for iniciado, acenda o seu LED por 2 segundos e depois apague-o por 2 segundos. \--- /task \---

\--- hints \--- \--- hint \---

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

\--- /hint \--- \--- /hints \---

\--- task \--- Faça o LED acender e apagar enquanto o seu código estiver em execução. \--- /task \---

\--- hints \--- \--- hint \--- Use

```blocks3
sempre
```

\--- /hint \--- \--- hint \---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

\--- /hint \--- \--- /hints \---

+ Faça o seu LED piscar mais rápido.

\--- hints \--- \--- hint \--- Use `espere x seg`{:class="block3control"} por menos segundos. \--- /hint \--- \--- hint \---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (0.5) secs
turn LED (17 v) [off v] ::extension
wait (0.5) secs
```

\--- /hint \--- \--- /hints \---

Muito bem — agora você está pronto para criar e controlar um arco-íris incrível!