## Verlicht je regenboog

Om er zeker van te zijn dat je regenboog werkt, test je deze eerst door de hele regenboog tegelijk te verlichten. Je maakt vervolgens code om de kleuren van de regenboog achter elkaar te laten knipperen. en dan in een patroon van jouw keuze.

\--- task \--- Voeg meer code toe om de andere LED's te besturen. Zorg ervoor dat je de juiste GPIO-pinnen toevoegt. \--- /task \---

Je regenboog zou als volgt moeten oplichten:

![Regenboog verlicht](images/rainbowlit.png)

\--- hints \--- \--- hint \--- Voeg meer `zet LED (0 v) [aan v]`{:class="block3extensions"} blokken toe in dit stuk code:

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```

\--- /hint \--- \--- hint \--- Blijf aan de onderkant blokken aan je code toevoegen tot al je LED's `aan`{:class="block3extensions"} staan.

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
turn LED (18 v) [on v] ::extension
turn LED (22 v) [on v] ::extension
```

\--- /hint \--- \--- hint \---

Als je LED's niet branden:

1) Controleer met welke GPIO-pinnen je LED's verbonden zijn, en zorg ervoor dat je ze hebt ingesteld op `aan`{:class="block3extensions"} 2) Test of de LED's werken - je kunt een LED verbindingsdraad aansluiten op **GPIO 3V3** om het te testen 3) Zorg ervoor dat het schakelcircuit op het experimenteerbord compleet is

\--- /hint \--- \--- /hints \---

\--- task \--- Voeg nu meer code toe om de regenboog in een regenboogpatroon te laten knipperen zoals hier:<video width="560" height="315" controls> <source src="resources/Scratch-GPIO-Pathways-5.mp4" type="video/mp4"> Je browser ondersteunt de video-tag niet, dus probeer Firefox of Chrome. </video> 

Om dit te doen moet je een LED een paar seconden aanzetten en vervolgens uitschakelen op hetzelfde moment als de volgende LED aangaat. \--- /task \---

\--- hints \--- \--- hint \---

Zorg ervoor dat je `Gebeurtenissen`{:class="block3events"} blok overeenkomt met wat je doet om de code te testen. In het voorbeeld hier, om onze regenboog te laten knipperen, moeten we op de groene vlag klikken:

```blocks3
when flag clicked
```

\--- /hint \--- \--- hint \---

Als je vastzit, zorg er dan voor dat je deze blokken gebruikt:

```blocks3
turn LED (0 v) [off v] ::extension
wait () secs
```

\--- /hint \--- \--- hint \---

Probeer deze aanpak te gebruiken:

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

Je moet voor al je LED's blokken toevoegen en ervoor zorgen dat je de juiste GPIO-pinnummers in je code gebruikt.

\--- /hint \--- \--- /hints \---

\--- task \--- Laat de lampjes de hele tijd volgens de regenboog oplichten.

Om eindeloos door het regenboogpatroon te lopen, gebruik je:

```blocks3
forever
```

\--- /task \---

\--- challenge \---

+ Laat de regenboog in een patroon naar keuze knipperen.

## \--- collapse \---

## title: Regenboog uitdagingen

Probeer de volgende ideeën uit:

1) Laat de LED's heel snel en erg langzaam knipperen 2) Laat de hele regenboog knipperen 3) Laat paren van LED's in alternatieve patronen knipperen 4) Laat de regenboog iets in morsecode knipperen 5) Laat de regenboog verschillende dingen doen in reactie op verschillende gebeurtenissen

\--- /collapse \--- \--- /challenge \---