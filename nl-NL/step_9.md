## Een knop toevoegen

Je gaat nu je regenboog laten oplichten en je eenhoorn laten dansen door op een knop te drukken!

### Sluit de knop aan

--- taak --- Sluit je knop aan op het experimenteerbord en een GPIO-pin.

Klik hieronder voor instructies over het verbinden van een knop met de Raspberry Pi. Let op, in plaats van **GPIO 17** zoals de instructies zeggen, hebben we **GPIO 5** gebruikt voor de knop — **GPIO 17** is al in gebruik door een LED.

[[[rpi-gpio-wiring-a-button]]]

Je regenboog zou er nu ongeveer zo uit moeten zien:

![Regenboog met knop](images/rainbowbutton.png) --- /task ---

### Programmeer de knop

--- task --- Gebruik het hieronder weergegeven blok zodat je knop de eenhoorn kan laten dansen.

```blocks3
when button (5 v) is [pressed v] :: hat extension
```

--- /task ---

### Bestuur de eenhoorn dans

Op dit moment zou je drie stukken Scratch code moeten hebben:

1. Dansende eenhoorn code
2. Knipperende regenboog code
3. Knop code

Je zult nu deze stukjes code verbinden zodat je eenhoorn gelijktijdig met je regenboog danst en dat je de regenboog en eenhoorn kunt bedienen door op de knop die je hebt toegevoegd te drukken.

--- task --- Verwijder alle `zeg`{:class="block3looks"} blokken in de code voor de knop, en kopieer dit stuk code. --- /task ---

--- task --- Verwijder in je code voor de eenhoorn dans het `wanneer op de groene vlag wordt geklikt`{:class="block3events"} blok. Neem de rest van de eenhoorncode en plaats deze in het `anders`{:class="block3control"} blok van je knopcode. Plaats het maar in **één exemplaar** van de knopcode. --- /task ---

--- task --- Verwijder in de regenboogcode het `wanneer op de groene vlag wordt geklikt`{:class="block3events"} blok en plaats de rest van de regenboogcode in het `anders`{:class="block3control"} blok van het **andere exemplaar** van de knopcode. --- /task ---

--- taak --- In het `als`{:class="block3control"}-deel van beide exemplaren van je knopcode voeg je een actie toe. Je kunt `verander uiterlijk naar het eerste uiterlijk`{:class="block3looks"} gebruiken, zodat de dansbewegingen van je eenhoorn niet in de war raken. --- /task ---

--- hints ---
 --- hint --- Als het indrukken van de knop de regenboog niet laat oplichten en de eenhoorn niet op tijd danst, probeer te controleren of:

1. Elke component is verbonden met de juiste GPIO-pin
2. Je hebt de in- en uitvoeren goed in je code
3. De timings komen overeen met je twee delen code
4. Je hebt alle juiste codeblokken gebruikt
--- /hint ---
--- /hints ---