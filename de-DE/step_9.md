## Füge einen Taster hinzu

Du wirst jetzt deinen Regenbogen blitzen und dein Einhorn synchron zu einem Tastendruck tanzen lassen!

### Einen Taster anschließen

--- task --- Verbinde deinen Taster mit dem Steckbrett und einem GPIO-Pin.

Klicke unten für eine Anleitung wie du einen Taster mit dem Raspberry Pi verbindest. Beachte, dass wir statt **GPIO 17**, wie es die Anleitung sagt, **GPIO 5** für den Taster verwendet haben — **GPIO 17** ist bereits durch eine LED belegt.

[[[rpi-gpio-wiring-a-button]]]

Dein Regenbogen sollte nun so aussehen:

![Regenbogen mit Knopf](images/rainbowbutton.png) --- /task ---

### Einen Taster programmieren

--- task --- Verwende den unten gezeigten Block, damit dein Taster das Einhorn zum tanzen bringen kann.

```blocks3
when button (5 v) is [pressed v] :: hat extension
```

--- /task ---

### Steuere den Einhorntanz

Im Moment solltest du drei Teile Scratch-Code haben:

1. Einhorn-Tanz-Code
2. Regenbogen-Blink-Code
3. Taster-Code

Du wirst diese Stücke jetzt verbinden, damit dein Einhorn gleichzeitig mit deinem Regenbogen tanzt und damit du den Regenbogen und das Einhorn steuern kannst, indem du auf den Taster drückst, den du hinzugefügt hast.

--- task --- Lösche alle `sage`{:class="block3looks"}-Blöcke im Code für den Taster und dann dupliziere diesen Codeabschnitt. --- /task ---

--- task --- Lösche den `Wenn die grüne Flagge angeklickt`{:class="block3events"}-Block in deinem Code für den Einhorntanz. Nimm den Rest des Einhorncodes und setze ihn in den `sonst`{:class="block3control"}-Block deines Taster-Codes. Setze es nur in **eine Kopie** des Taster-Codes. --- /task ---

--- task --- Im Regenbogen-Code, lösche den `Wenn die grüne Flagge angeklickt`{:class="block3events"}-Block und setze den Rest den Regenbogen-Codes in den `sonst`{:class="block3control"}-Block der **anderen Kopie** des Taster-Codes. --- /task ---

--- task --- Füge eine Aktion, in den `falls`{:class="block3control"}-Teil beider Kopien deines Taster-Codes, hinzu. Du könntest `wechsle Kostüm zu Kostüm1`{:class="block3looks"} verwenden, damit dein Einhorn seine Tanzbewegungen nicht durcheinander bringt. --- /task ---

--- hints ---
 --- hint --- Falls das Drücken des Tasters nicht den Regenbogen leuchten und gleichzeitig das Einhorn tanzen lässt, versuche sicherzustellen, dass:

1. Jede Komponente mit dem richtigen GPIO-Pin verbunden ist
2. Die Ein- und Ausgänge in deinem Code stimmen
3. Das Timing deiner beiden Codeblöcke übereinstimmt
4. Du überall die richtigen Codeblöcke verwendest
--- /hint ---
--- /hints ---