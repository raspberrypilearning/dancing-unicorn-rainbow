## Allume ton arc-en-ciel

Pour t'assurer que ton arc-en-ciel fonctionne, tu dois d'abord le tester en allumant tout l'arc-en-ciel à la fois. Tu vas ensuite créer du code pour faire clignoter l'arc-en-ciel à travers toutes ses couleurs les unes après les autres, puis dans un motif de ton choix.

--- task ---
Ajoute plus de code pour contrôler les autres LEDs. Assure-toi d'inclure les bonnes broches GPIO. --- /task ---

Ton arc-en-ciel devrait s'allumer comme ceci:

![Lumières Arc-en-Ciel](images/rainbowlit.png)

--- hints ---
--- hint --

Ajoute plus de blocs `turn LED (0 v) [on v]`{:class="block3extensions"} dans ce bout de code:

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```
--- /hint ---
--- hint ---

Continue à ajouter des blocs au bas de ton code jusqu'à ce que toutes tes LEDs soient réglées sur `on`{:class="block3extensions"}.

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
turn LED (18 v) [on v] ::extension
turn LED (22 v) [on v] ::extension
```

--- /hint --- 
--- hint ---

Si tes LEDs ne s'allument pas:

1) Vérifie à quelles broches GPIO tes LEDs sont connectées et assure-toi de les avoir réglées sur `on`{:class="block3extensions"} 2) Teste si les LEDs fonctionnent - tu peux brancher le fil de cavalier d'une LED dans **GPIO 3V3** pour le tester 3) Assure-toi que le circuit de la platine d'expérimentation est complet

--- /hint ---
--- /hints ---

Maintenant, ajoute plus de code pour faire clignoter l'arc-en-ciel dans un motif arc-en-ciel comme ceci:

<video width="560" height="315" controls> <source src="resources/Scratch-GPIO-Pathways-5.mp4" type="video/mp4"> Ton navigateur ne supporte pas le tag vidéo, essaie FireFox ou Chrome. </video> 

Pour ce faire, tu devras allumer une LED pendant quelques secondes, puis l'éteindre en même temps que la prochaine LED s'allume. 
--- /task ---

--- hints ---
--- hint ---

Assure-toi que tes blocs `événements`{:class="blockevents"} correspondent à ce que tu fais pour tester le code. Dans l'exemple ici, pour faire clignoter notre arc-en-ciel, nous devons cliquer sur le drapeau vert:

```blocks3
when flag clicked
```

--- /hint --- 
--- hint ---

Si tu es bloqué, assure-toi que tu utilises ces blocs:

```blocks3
turn LED (0 v) [off v] ::extension
wait () secs
```

--- /hint --- 
--- hint ---

Essaie d'utiliser cette approche:

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

Tu devrais ajouter des blocs pour toutes tes LEDs et t'assurer que tu utilises les bons numéros de broches GPIO dans ton code.

--- /hint ---
--- /hints ---

--- task ---
Fais clignoter les lumières à plusieurs reprises à travers l'arc-en-ciel en boucle.

Pour faire une boucle à travers le motif arc-en-ciel indéfiniment, utilise:

```blocks3
forever
```

--- /task ---

--- challenge ---

+ Fais clignoter l'arc-en-ciel selon le motif de ton choix.

--- collapse ---
---
title: Défis arc-en-ciel
---

Essaie les idées suivantes:

1) Faire clignoter les LEDs très rapidement et très lentement 2) Faire clignoter tout l'arc-en-ciel 3) Faire s'allumer des paires de LEDs en alternance 4) Faire clignoter quelque chose de l'arc-en-ciel en code Morse 5) Faire en sorte que l'arc-en-ciel fasse différentes choses en réponse à différents événements

--- /collapse --- 
--- /challenge ---