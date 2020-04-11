## Steuere deine Regenbogen-Schaltung

Wenn dein ganzer Regenbogen eingerichtet ist, kannst du kontrollieren wie er leuchtet. Um ein bisschen zu üben wie man eine LED kontrolliert, nutze Scratch um folgendes zu tun:

--- task --- 

Wenn du die Taste <kbd>P</kbd> drückst, schalte die LED für zwei Sekunden ein und dann aus. 

--- /task ---

--- hints --- 
--- hint --- 

Schau in den `Steuerungs`{:class="block3control"}-Blöcke Abschnitt. 

--- /hint --- 
--- hint --- 

Verwende

```blocks3
  wait (2) secs
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

Wenn dein Scratch Programm startet, lass deine LED für 2 Sekunden aufleuchten und schalte sie dann für 2 Sekunden aus. 

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

Lass deine LED an und aus gehen solange dein Programm läuft. 

--- /task ---

--- hints --- 
--- hint --- 

Verwende

```blocks3
forever
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

+ Lass deine LED schneller blinken.

--- hints --- 
--- hint --- 

Verwende `warte x Sekunden`{:class="block3control"} mit weniger Sekunden. 

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

Gut gemacht – du bist jetzt bereit einen tollen Regenbogen zu bauen und zu kontrollieren!