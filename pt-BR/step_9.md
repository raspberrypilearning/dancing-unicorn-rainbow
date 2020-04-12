## Adicione um botão

Agora você fará seu arco-íris brilhar e seu unicórnio dançar no tempo pressionando um botão!

### Conecte o botão

--- task --- Conecte seu botão à protoboard e a um pino GPIO.

Clique abaixo para obter instruções sobre como conectar um botão ao Raspberry Pi. Observe que, em vez de **GPIO 17** como dizem as instruções, usamos **GPIO 5** para o botão — **GPIO 17** já é usado por um LED.

[[[rpi-gpio-wiring-a-button]]]

Seu arco-íris agora deve parecer como algo assim:

![Arco-íris com botão](images/rainbowbutton.png) --- /task ---

### Programe o botão

--- task --- Use o bloco mostrado abaixo para que seu botão possa fazer o unicórnio dançar.

```blocks3
when button (5 v) is [pressed v] :: hat extension
```

--- /task ---

### Controle a dança do unicórnio

No momento, você deve ter três partes do código do Scratch:

1. Código do unicórnio dançarino
2. Código do arco-íris piscando
3. Código do botão

Agora você conectará essas partes para que seu unicórnio dance ao tempo com o o seu arco-íris e para poder controlar o arco-íris e o unicórnio pressionando o botão que você adicionou.

--- task --- Apague todos os blocos `diga`{:class="block3looks"} no código do botão, e então duplique este pedaço de código. --- /task ---

--- task --- No seu código para a dança do unicórnio, apague o bloco `quando bandeira verde for clicado`{:class="block3events"}. Pegue o restante do código do unicórnio e coloque-o no bloco `senão`{:class="block3control"} do seu código do botão. Coloque apenas **uma cópia** do código do botão. --- /task ---

--- task --- No código do arco-íris, apague o bloco `quando bandeira verde for clicado`{:class="block3events"} e coloque o restante do código do arco-íris no bloco `senão`{:class="block3control"} da **outra cópia** do código do botão. --- /task ---

--- task --- No espaço `se`{:class="block3control"} de ambas as cópias do código do botão, adicione uma ação. Você pode usar `mude de fantasia para a primeira fantasia`{:class="block3looks"}, para que seu unicórnio não tenha seus movimentos de dança misturados. --- /task ---

--- hints ---
 --- hint --- Se pressionar o botão não fizer a luz do arco-íris acender e o unicórnio dançar no tempo, tente verificar que:

1. Cada componente está conectado ao pino GPIO correto
2. Você tem as entradas e saídas corretas no seu código
3. Os tempos correspondem nos seus dois pedaços de código
4. Você usou todos os blocos de código corretos
--- /hint ---
--- /hints ---