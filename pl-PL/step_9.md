## Dodaj przycisk

Teraz sprawisz, że tęcza zabłyśnie, a jednorożec będzie tańczył podczas gdy przycisk będzie wciśnięty!

### Podłącz przycisk

--- task --- Podłącz swój przycisk do płytki stykowej i pinu GPIO.

Kliknij poniżej, aby uzyskać instrukcje na temat podłączania przycisku do Raspberry Pi. Zauważ, że zamiast **GPIO 17** jak mówi instrukcja, użyliśmy **GPIO 5** dla przycisku - **GPIO 17** jest już zajęte przez diodę LED.

[[[rpi-gpio-wiring-a-button]]]

Twoja tęcza powinna teraz wyglądać podobnie do tej:

![Tęcza z przyciskiem](images/rainbowbutton.png) --- /task ---

### Zaprogramuj przycisk

--- task --- Użyj poniższego bloku, aby twój przycisk sprawił, żeby jednorożec zatańczył.

```blocks3
when button (5 v) is [pressed v] :: hat extension
```

--- /task ---

### Kontroluj taniec jednorożca

W tej chwili powinieneś mieć trzy kawałki kodu Scratch:

1. Kod tańczącego jednorożca
2. Kod migającej tęczy
3. Kod przycisku

Teraz połączysz te fragmenty, aby jednorożec tańczył wraz z tęczą i abyś mógł kontrolować tęczę i jednorożca, naciskając dodany przycisk.

--- task --- Usuń wszystkie bloki `powiedz` w tym kodzie dla przycisku, a później skopiuj ten fragment kodu. --- /task ---

--- task --- W kodzie dla tańca jednorożcowego usuń blok `kiedy kliknięto zieloną flagę`{:class="block3events"}. Weź resztę kodu jednorożca i umieść go w bloku `w przeciwnym razie`{:class="block3control"} w kodzie przycisku. Umieść go tylko w **jednej kopii** kodu przycisku. --- /task ---

--- task --- W kodzie tęczy usuń blok `kiedy kliknięto zieloną flagę`{:class="block3events"} i umieść resztę kodu tęczy w bloku `w przeciwnym razie`{:class="block3control"} **innej kopii** kodu przycisku. --- /task ---

--- task --- W obu kopii kodu przycisku wewnątrz bloków `jeżeli`{:class="block3control"}, dodaj akcję. Możesz użyć bloku `przełącz kostium na pierwszy kostium`{:class="block3looks"}, żeby twój jednorożec nie mieszał ruchów tanecznych. --- /task ---

--- hints ---
 --- hint --- Jeśli naciśnięcie przycisku nie rozświetliło tęczy, a jednorożec tańczy poprawnie, spróbuj sprawdzić, czy:

1. Każdy komponent jest podłączony do odpowiedniego pinu GPIO
2. Masz wejścia i wyjścia poprawnie w swoim kodzie
3. Czasy pasują do twoich dwóch fragmentów kodu
4. Użyłeś wszystkich odpowiednich bloków kodu --- /hint --- --- /hints ---