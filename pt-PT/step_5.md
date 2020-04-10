## Controla o teu circuito arco-íris

Quando todo o teu arco-íris estiver configurado, tu podes controlar como ele é aceso. Para um pouco de prática para controlar um LED, usa o Scratch para fazer o seguinte:

\--- task \--- Quando pressionares a tecla <kbd>P</kbd>, liga o LED por dois segundos e depois desliga. \--- /task \---

\--- dicas \--- \--- dica \--- Procura na secção de blocos `controlo`{: class = "block3control"}. \--- / dica \--- \--- dica \--- Uso

```blocks3
  espera (2) segundos
```

\--- /hint \--- \--- hint \---

```blocks3
when [p v] key pressed
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
```

\--- /hint \--- \--- /hints \---

\--- task \--- Quando o programa do Scratch for iniciado, faz o teu LED acender por 2 segundos e depois apaga-o por 2 segundos. \--- /task \---

\--- hints \--- \--- hint \---

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

\--- /hint \--- \--- /hints \---

\--- task \--- Faça o LED acender e apagar enquanto o teu programa estiver em execução. \--- /task \---

\--- / dica \--- \--- dica \--- Uso

```blocks3
para sempre
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

+ Faz o teu LED piscar mais rápido.

\--- dicas \--- \--- dica \--- Usa `espera x secs` {: class = "block3control"} por menos segundos. \--- /hint \--- \--- hint \---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (0.5) secs
turn LED (17 v) [off v] ::extension
wait (0.5) secs
```

\--- /hint \--- \--- /hints \---

Muito bem - agora tu estás pronto para criar e controlar um arco-íris incrível!