## Kontroluj twój obwód tęczy

Kiedy cała twoja tęcza jest gotowa, możesz kontrolować, jak ma się zapalać. Aby trochę poćwiczyć sterowanie jedną diodą LED, użyj Scratch, aby wykonać następujące czynności:

--- task --- Po naciśnięciu przycisku <kbd>P</kbd>, włącz diodę na dwie sekundy, a następnie wyłącz. --- /task ---

--- hints ---
 --- hint --- Spójrz na sekcje bloków `Kontrola`{:class="block3control"}.
--- /hint ---
 --- hint --- Użyj

```blocks3
  czekaj (2) sek
```

--- /hint --- --- hint ---

```blocks3
when [p v] key pressed
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
```

--- /hint ------ /hints ---

--- task --- Po uruchomieniu programu Scratch włącz diodę LED na 2 sekundy, a następnie wyłącz na 2 sekundy. --- /task ---

--- hints ---
 --- hint ---

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

--- /hint ------ /hints ---

---task--- Włączaj i wyłączaj twoją diodę LED tak długo jak twój program jest włączony. --- /task ---

--- hints ---
 --- hint --- Użyj

```blocks3
zawsze
```

--- /hint --- --- hint ---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

--- /hint ------ /hints ---

+ Spraw, aby Twoja dioda LED mrugała szybciej.

--- hints ---
 --- hint --- Użyj `czekaj x sekund`{:class="block3control"} na mniej sekund.
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

--- /hint ------ /hints ---

Dobra robota - jesteś teraz gotowy, aby stworzyć i kontrolować niesamowitą tęczę!