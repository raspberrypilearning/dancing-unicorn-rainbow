## Ilumine o seu arco-íris

Para ter certeza que o seu arco-íris está funcionando, você primeiro testará iluminando todo o arco-íris de uma vez. Você então criará um código para fazer o arco-íris piscar todas as suas cores uma após a outra, e, em seguida, em um padrão de sua escolha.

\--- task \--- Adicione mais código para controlar os outros LEDs. Certifique-se de incluir os pinos GPIO corretos. \--- /task \---

Seu arco-íris deve acender assim:

![Arco-íris aceso](images/rainbowlit.png)

\--- hints \--- \--- hint \--- Adicione mais blocos `turn LED (0 v) [on v]`{:class="block3extensions"} neste pedaço de código:

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```

\--- /hint \--- \--- hint \--- Continue adicionando blocos na parte inferior do seu código até que todos os seus LEDs estejam definidos como `on`{:class="block3extensions"}.

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
turn LED (18 v) [on v] ::extension
turn LED (22 v) [on v] ::extension
```

\--- /hint \--- \--- hint \---

Se seus LEDs não estiverem acendendo:

1) Verifique em quais pinos GPIO seus LEDs estão conectados, e certifique-se de tê-los definido como `on`{:class="block3extensions"} 2) Teste se os LEDs estão funcionando — você pode conectar o fio jumper de um LED em **GPIO 3V3** para testá-lo 3) Certifique-se de que o circuito na protoboard está completo

\--- /hint \--- \--- /hints \---

\--- task \--- Agora, adicione mais código para fazer o arco-íris piscar em um padrão de arco-íris como este:<video width="560" height="315" controls> <source src="resources/Scratch-GPIO-Pathways-5.mp4" type="video/mp4"> Your browser does not support the video tag, so try FireFox or Chrome. </video> 

Para fazer isso, você precisará acender um LED por alguns segundos e depois apagar ao mesmo tempo que o próximo LED acender. \--- /task \---

\--- hints \--- \--- hint \---

Verifique se o seu bloco `Eventos`{:class="blockevents"} corresponde ao que você está fazendo para testar o código. Neste exemplo, para fazer nosso arco-íris piscar, temos de clicar na bandeira verde:

```blocks3
when flag clicked
```

\--- /hint \--- \--- hint \---

Se você estiver travado, verifique se está usando estes blocos:

```blocks3
turn LED (0 v) [off v] ::extension
wait () secs
```

\--- /hint \--- \--- hint \---

Tente usar esta abordagem:

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

Você precisará adicionar blocos para todos os seus LEDs e verifique se está usando os números de pinos GPIO corretos no seu código.

\--- /hint \--- \--- /hints \---

\--- task \--- Faça as luzes piscarem repetidamente através do arco-íris em um loop.

Para percorrer o padrão do arco-íris para sempre, use:

```blocks3
sempre
```

\--- /task \---

\--- challenge \---

+ Faça o arco-íris piscar em um padrão de sua escolha.

## \--- collapse \---

## title: Rainbow challenges

Try out the following ideas:

1) Make the LEDs blink very fast and very slow 2) Make the whole rainbow blink 3) Make pairs of LEDs light up in alternate patterns 4) Make the rainbow blink something in Morse code 5) Make the rainbow do different things in response to different events

\--- /collapse \--- \--- /challenge \---