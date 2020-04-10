## Ajoute un bouton

Tu vas maintenant faire clignoter ton arc-en-ciel et ta licorne dans le temps en appuyant sur un bouton !

### Connecter le bouton

Connecte ton bouton à la platine d'expérimentation et à une broche GPIO.

Clique ci-dessous pour savoir comment connecter un bouton au Raspberry Pi. Note qu'au lieu de **GPIO 17** comme le disent les instructions, nous avons utilisé **GPIO 5** pour le bouton - **GPIO 17** est déjà occupé par une LED.

[[[rpi-gpio-wiring-a-button]]]

Ton arc-en-ciel devrait maintenant ressembler à ceci :

![Arc-en-ciel avec bouton](images/rainbowbutton.png) \--- /task \---

### Coder le bouton

Utilise le bloc illustré ci-dessous pour que ton bouton puisse faire danser la licorne.

```blocks3
when button (5 v) is [pressed v] :: hat extension
```

\--- /task \---

### Contrôle la danse de la licorne

Pour le moment, tu devrais avoir trois bouts de code Scratch :

1. Code de licorne dansante
2. Code arc-en-ciel clignotant
3. Code du bouton

Tu vas maintenant connecter ces bouts pour que ta licorne danse au rythme de ton arc-en-ciel, et que tu puisses contrôler l'arc-en-ciel et la licorne en appuyant sur le bouton que tu as ajouté.

Supprime tous les blocs `dire`{:class="block3looks"} dans le code du bouton, puis duplique ce bout de code. \--- /task \---

Dans ton code pour la danse de la licorne, supprime le bloc `quand le drapeau est cliqué`{:class="block3events"}. Prends le reste du code de la licorne et insère-le dans le bloc `sinon`{:class="block3control"} de ton code de bouton. Insère-le uniquement dans **une copie** du code du bouton. \--- /task \---

Dans le code arc-en-ciel, supprime le bloc `quand le drapeau est cliqué`{:class="block3events"} et insère le reste du code arc-en-ciel dans le bloc `sinon`{:class="block3control"} de **l'autre copie** du code du bouton. \--- /task \---

Dans l'emplacement `si`{:class="block3control"} des deux copies de ton code de bouton, ajoute une action. Tu peux utiliser `basculer le costume sur le premier costume`{:class="block3looks"}, afin que ta licorne ne mélange pas ses mouvements de danse. \--- /task \---

Si le fait d'appuyer sur le bouton ne fait pas s'allumer l'arc-en-ciel et la licorne danser en rythme, essaie de vérifier que :

1. Chaque composant est connecté à la bonne broche GPIO
2. Tu as les entrées et sorties directement dans ton code
3. Les timings correspondent à tes deux bouts de code
4. Tu as utilisé tous les bons blocs de code