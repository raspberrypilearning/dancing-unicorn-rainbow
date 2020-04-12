## Έλεγξε το κύκλωμα του ουράνιου τόξου σου

Όταν το ουράνιο τόξου σου έχει ρυθμιστεί, μπορείς να ελέγξεις πώς θα είναι αναμμένο. Για να εξοικειωθείς με τον ελέγχο ενός LED, χρησιμοποίησε το Scratch για να κάνεις τα εξής:

--- task --- Όταν πατάς το πλήκτρο <kbd>P</kbd>, ενεργοποιείται η λυχνία LED για δύο δευτερόλεπτα και στη συνέχεια απενεργοποιείται. --- /task ---

--- hints ---
 --- hint --- Κοίταξε στο τμήμα μπλοκ `Έλεγχος`{:class="block3control"}.
--- /hint ---
 --- hint --- Χρησιμοποίησε

```blocks3
  wait (2) secs
```

--- /hint --- --- hint ---

```blocks3
when [p v] key pressed
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
```

--- /hint ------ /hints ---

--- task --- Όταν ξεκινήσει το πρόγραμμα Scratch, το LED σου ανάβει για 2 δευτερόλεπτα και μετά σβήνει για 2 δευτερόλεπτα. --- /task ---

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

--- task --- Ενεργοποίησε και απενεργοποίησε τη λυχνία LED όσο εκτελείται το πρόγραμμα. --- /task ---

--- hints ---
 --- hint --- Χρησιμοποίησε

```blocks3
για πάντα
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

+ Κάνε το LED σου να αναβοσβήνει πιο γρήγορα.

--- hints ---
 --- hint --- Χρησιμοποίησε `περίμενε x δευτερόλεπτα`{:class="block3control"} για λιγότερα δευτερόλεπτα.
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

Συγχαρητηρια - είσαι έτοιμος τώρα να δημιουργήσεις και να ελέγξεις ένα φοβερό ουράνιο τόξο!