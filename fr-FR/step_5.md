## Contrôle ton circuit arc-en-ciel

Lorsque ton arc-en-ciel entier est installé, tu peux contrôler son allumage. Pour t'exercer un peu à contrôler une LED, utilise Scratch pour effectuer les opérations suivantes:

--- task ---
Lorsque tu appuies sur <kbd>P</kbd>, allume la LED pendant deux secondes, puis elle s'éteint. --- /task ---

--- hints ---
--- hint ---
Regarde dans la section des blocs `contrôle`{:class="block3control"}. Utilise

```blocks3
  attendre (2) secondes
```

--- /hint --- 
--- hint ---

```blocks3
when [p v] key pressed
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
```

--- /hint ---
--- /hints ---

--- task ---
Lorsque ton programme Scratch démarre, allume ta LED pendant 2 secondes, puis l'éteint pendant 2 secondes. 
--- /task ---

--- hints ---
--- hint ---

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

--- /hint ---
--- /hints ---

--- task ---
Allume et éteint ta LED tant que ton programme s'exécute. 
--- /task ---

--- hints ---
--- hint ---
Utilise

```blocks3
répéter indéfiniment
```

--- /hint --- 
--- hint ---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

--- /hint ---
--- /hints ---

+ Fais clignoter ta LED plus rapidement.

--- hints ---
--- hint ---

Utilise `attendre x secondes`{:class="block3control"} pendant moins de secondes.
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

--- /hint ---
--- /hints ---

Bien joué - tu es maintenant prêt à créer et contrôler un arc-en-ciel génial!