## Zaświeć swoją tęczę

Aby upewnić się, że twoja tęcza działa, najpierw przetestujesz ją, zapalając całą tęczę naraz. Następnie utworzysz kod, który sprawi, że tęcza będzie migać po kolei we wszystkich kolorach, a następnie według wybranego wzoru przez ciebie.

\---task\--- Dodaj więcej kodu do sterowania innymi diodami LED. Upewnij się, że użyto odpowiednich pinów GPIO. \--- /task \---

Twoja tęcza powinna świecić się w następujący sposób:

![Zapalona tęcza](images/rainbowlit.png)

\--- hints \--- \--- hint \--- Dodaj więcej bloków `włącz diodę LED(0 v) [on v]`{:class="block3extensions"} w tej części programu:

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```

\--- /hint \--- \--- hint \--- Dodawaj bloki u dołu kodu, dopóki wszystkie twoje diody LED nie zostaną ustawione na `on`{:class="block3extensions"}.

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
turn LED (18 v) [on v] ::extension
turn LED (22 v) [on v] ::extension
```

\--- /hint \--- \--- hint \---

Jeśli diody LED nie świecą:

1) Sprawdź, do których pinów GPIO są podłączone diody LED i upewnij się, że ustawiłeś je na `on`{:class="block3extensions"} 2) Sprawdź, czy diody LED działają - możesz podłączyć przewód diody do **GPIO 3V3** aby go przetestować 3) Upewnij się, że obwód na płycie stykowej jest cały

\--- /hint \--- \--- /hints \---

\--- task \--- Teraz dodaj więcej kodu, aby tęcza migała w takim wzorze:<video width="560" height="315" controls> <source src="resources/Scratch-GPIO-Pathways-5.mp4" type="video/mp4"> Twoja przeglądarka nie obsługuje wideo, więc spróbuj FireFox lub Chrome. </video> 

Aby to zrobić, musisz włączyć jedną diodę LED na kilka sekund, a następnie wyłączyć ją w tym samym czasie, kiedy zaświecasz następną diodę LED. \--- /task \---

\--- hints \--- \--- hint \---

Upewnij się, że Twój blok`Zdarzenia`{:class="blockevents"} odpowiada temu, co robisz, aby przetestować kod. W tym przykładzie, aby nasza tęcza migała, musimy kliknąć zieloną flagę:

```blocks3
when flag clicked
```

\--- /hint \--- \--- hint \---

Jeśli utknęłaś, upewnij się, że używasz tych bloków:

```blocks3
turn LED (0 v) [off v] ::extension
wait () secs
```

\--- /hint \--- \--- hint \---

Spróbuj użyć tego podejścia:

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

Musisz dodać bloki dla wszystkich diod LED i upewnić się, że używasz odpowiednich numerów pinów GPIO w kodzie.

\--- /hint \--- \--- /hints \---

\--- task \--- Spraw aby światła w tęczy migały wielokrotnie w pętli.

Aby na zawsze zapętlić tęczowy wzór, użyj:

```blocks3
forever
```

\--- /task \---

\--- challenge \---

+ Spraw, aby tęcza mrugała według wybranego przez ciebie wzoru.

## \--- collapse \---

## title: Rainbow challenges

Try out the following ideas:

1) Make the LEDs blink very fast and very slow 2) Make the whole rainbow blink 3) Make pairs of LEDs light up in alternate patterns 4) Make the rainbow blink something in Morse code 5) Make the rainbow do different things in response to different events

\--- /collapse \--- \--- /challenge \---