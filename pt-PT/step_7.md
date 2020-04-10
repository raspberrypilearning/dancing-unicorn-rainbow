## Ilumina o teu arco-íris

Para garantir que o teu arco-íris está a funcionar, irás testá-lo primeiro iluminando todo o arco-íris de uma só vez. Irás criar código para fazer o arco-íris piscar através de todas as cores, uma após a outra, e depois num padrão à tua escolha.

\--- tarefa \--- Adiciona mais código para controlar os restantes LEDs. Certifica-te de incluir os pinos GPIO corretos. \--- /task \---

O teu arco-íris deverá acender assim:

![Arco-íris aceso](images/rainbowlit.png)

\--- dicas \--- \--- dica \--- Adicione mais blocos `turn LED (0 v) [on v]`{: class = "block3extensions"} neste pedaço de código:

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```

\--- / dica \--- \--- dica \--- Contina a adicionar blocos na parte inferior do teu código até que todos os teus LEDs estejam configurados para `on` {: class = "block3extensions"}.

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
turn LED (18 v) [on v] ::extension
turn LED (22 v) [on v] ::extension
```

\--- /hint \--- \--- hint \---

Se os teus LEDs não estiverem a acender:

1) Verifica quais os pinos GPIO os teus LEDs estão ligados e verifica se os definiste como `on` {: class = "block3extensions"} 2) Testa se os LEDs estão a funcionar - Podes ligar o fio de ligação de um LED ao **GPIO 3V3** para testá-lo 3) Verifica se o circuito na placa de ensaio está completo

\--- /hint \--- \--- /hints \---

\--- tarefa \--- Agora, adiciona mais código para fazer o arco-íris piscar num padrão de arco-íris como este:<video width="560" height="315" controls> <source src="resources/Scratch-GPIO-Pathways-5.mp4" type="video/mp4"> O teu navegador não suporta a tag de vídeo, tenta o FireFox ou o Chrome. </video> 

Para fazer isto, precisas de acender um LED por alguns segundos e depois desligar ao mesmo tempo que o próximo LED acender. \--- /task \---

\--- hints \--- \--- hint \---

Certifica-te que os teu bloco de `Eventos`{: class = "blockevents"} corresponde ao que estás fazendo para testar o código. Neste exemplo, para fazer nosso arco-íris piscar, é preciso clicar na bandeira verde:

```blocks3
when flag clicked
```

\--- /hint \--- \--- hint \---

Se você estiveres encalhado, certifica-te que estás a usar estes blocos:

```blocks3
turn LED (0 v) [off v] ::extension
wait () secs
```

\--- /hint \--- \--- hint \---

Tenta usar esta abordagem:

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

Precisas de adicionar blocos para todos os teus LEDs e certifica-te que estás a usar os números dos pinos GPIO corretos no teu código.

\--- /hint \--- \--- /hints \---

\--- tarefa \--- Faz as luzes piscarem repetidamente através do arco-íris num ciclo.

Para percorrer o padrão do arco-íris para sempre, usa:

```blocks3
forever
```

\--- /task \---

\--- challenge \---

+ Faz o arco-íris piscar num padrão à tua escolha.

\--- collapse \---

* * *

## title: Desafios do arco-íris

Tenta as seguintes ideias:

1) Faz os LEDs piscarem muito rápido e muito lentamente 2) Faz o arco-íris inteiro piscar 3) Faz pares de LEDs acenderem em padrões alternativos 4) Faz o arco-íris piscar algo em código Morse 5) Faz o arco-íris fazer coisas diferentes em resposta a diferentes eventos

\--- /collapse \--- \--- /challenge \---