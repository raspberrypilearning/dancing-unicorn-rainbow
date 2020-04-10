## Adiciona um botão

Agora irás fazer o teu de arco-íris brilhar e o teu unicórnio dançar no tempo pressionando um botão!

### Liga o botão

\--- tarefa \--- Liga o teu botão à placa de ensaio e a um pino GPIO.

Clica em baixo para obter instruções sobre como ligar um botão ao Raspberry Pi. Observe que, em vez de **GPIO 17** como dizem as instruções, usamos o **GPIO 5** para o botão - o **GPIO 17** já está usado por um LED.

[[[rpi-gpio-wiring-a-button]]]

O teu arco-íris deverá agora ser algo como isto:

![Arco-íris com botão](images/rainbowbutton.png) \--- /task \---

### Programa o botão

\--- tarefa \--- Use o bloco mostrado em baixo para que o teu botão possa fazer o unicórnio dançar.

```blocks3
when button (5 v) is [pressed v] :: hat extension
```

\--- /task \---

### Controlar a dança do unicórnio

Até ao momento, deverás ter três partes de código do Scratch:

1. Código do unicórnio dançarino
2. Código do arco-íris piscando
3. Código do botão

Agora irás juntar estes bocados para que o teu unicórnio dançe ao tempo do teu arco-íris, e para que tu possas controlar o arco-íris e o unicórnio pressionando o botão que adicionaste.

\--- tarefa \--- Elimina todos os blocos `diz` {: class = "block3looks"} do código do botão e depois duplica este bocado de código. \--- /task \---

\--- tarefa \--- No teu código para a dança do unicórnio, elimina o bloco `quando alguém clicar na bandeira` {: class = "block3events"}. Pega no restante código do unicórnio e insire-o no bloco `senão`{:class="block3control"} do teu código do botão. Insere-o apenas ** numa cópia ** do código do botão. \--- /task \---

\--- tarefa \--- No código do arco-íris elimina o bloco `quando alguém clicar na bandeira verde`{:class="block3events"} e insere o resto do código do arco-íris dentro do bloco `senão`{:class="block3control"} da **outra cópia** do código do botão. \--- /task \---

\--- tarefa \--- No espaço `se`{:class="block3control"} de ambas as cópias do código do botão, adiciona uma ação. Poderias usar `mudar de traje para o primeiro traje`{:class="block3looks"}, para que o teu unicórnio não misture os seus movimentos de dança. \--- /task \---

\--- dicas \--- \--- dica \--- Se pressionar o botão não ander a luz do arco-íris e o unicórnio dançar no tempo, tenta verificar que:

1. Cada componente está ligado ao pino GPIO correto
2. Tens as entradas e saídas corretas no teu código
3. Os tempos correspondem nos teus dois bocados de código
4. Usaste todos os blocos de código certos \--- /dica \--- \--- /dicas \---