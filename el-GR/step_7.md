## Φώτισε το ουράνιο τόξο σου

Για να βεβαιωθείς ότι το ουράνιο τόξο σου λειτουργεί, θα δοκιμάσεις πρώτα να φωτίσεις ταυτόχρονα ολόκληρο το ουράνιο τόξο. Στη συνέχεια, θα δημιουργήσεις κώδικα για να κάνεις το ουράνιο τόξο να αναβοσβήνει σε όλα τα χρώματα το ένα μετά το άλλο, και έπειτα σε ένα μοτίβο της επιλογής σου.

\--- task \--- Πρόσθεσε περισσότερο κωδικα για να ελέγξεις τις άλλες λυχνίες LED. Βεβαιώσου ότι έχεις συμπεριλάβει τις σωστές ακίδες GPIO. \--- /task \---

Το ουράνιο τόξο σου θα πρέπει να ανάψει ως εξής:

![Αναμμένο Ουράνιο Τόξο](images/rainbowlit.png)

\--- hints \--- \--- hint \--- Πρόσθεσε περισσότερα μπλοκ `turn LED (0 v) [on v]`{:class="block3extensions"} σε αυτό το σημείο του κώδικα:

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```

\--- /hint \--- \--- hint \--- Συνέχισε να προσθέτεις μπλοκ στο κάτω μέρος του κώδικά σου μέχρι όλα τα LED να `ανάψουν`{:class="block3extensions"}.

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
turn LED (18 v) [on v] ::extension
turn LED (22 v) [on v] ::extension
```

\--- /hint \--- \--- hint \---

Εάν δεν ανάβουν τα LED:

1) Έλεγξε ποιες ακίδες GPIO συνδέονται με τα LED σου και βεβαιώσου ότι τα έχεις ρυθμίσει να είναι `on`{:class="block3extensions"} 2) Δοκίμασε κατά πόσον τα LED δουλεύουν - μπορείς να συνδέσεις ένα καλώδιο από ένα LED σε **GPIO 3V3** για να το δοκιμάσεις 3) Βεβαιώσου ότι το κύκλωμα στην πλακέτα δοκιμών είναι ολοκληρωμένο

\--- /hint \--- \--- /hints \---

\--- task \--- Τώρα, πρόσθεσε περισσότερο κώδικα για να κάνεις το ουράνιο τόξο να αναβοσβήνει σε ένα μοτίβο όπως αυτό:<video width="560" height="315" controls> <source src="resources/Scratch-GPIO-Pathways-5.mp4" type="video/mp4"> Το πρόγραμμα περιήγησής σου δεν υποστηρίζει ετικέτες βίντεο, επομένως δοκίμασε το Firefox ή το Chrome. </video> 

Για να γίνει αυτό, θα χρειαστεί να ενεργοποιήσεις μια λυχνία LED για μερικά δευτερόλεπτα και, στη συνέχεια, να την απενεργοποιήσεις ταυτόχρονα με την ενεργοποίηση της επόμενης λυχνίας LED. \--- /task \---

\--- hints \--- \--- hint \---

Βεβαιώσου ότι τα μπλοκ `Γεγονότα`{:class="blockevents"} σου ταιριάζουν με αυτό που κάνεις για να ελέγξεις τον κώδικα. Στο παράδειγμα εδώ, για να αναβοσβήνει το ουράνιο τόξο, πρέπει να κάνουμε κλικ στην πράσινη σημαία:

```blocks3
when flag clicked
```

\--- /hint \--- \--- hint \---

Εάν κολλήσεις, βεβαιώσου ότι χρησιμοποιείς αυτά τα μπλοκ:

```blocks3
turn LED (0 v) [off v] ::extension
wait () secs
```

\--- /hint \--- \--- hint \---

Δοκίμασε να χρησιμοποιήσεις αυτήν την προσέγγιση:

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

Θα χρειαστεί να προσθέσεις μπλοκ για όλα τα LED σου και βεβαιώσου ότι χρησιμοποιείς τους σωστούς αριθμούς ακίδων GPIO στον κώδικα σου.

\--- /hint \--- \--- /hints \---

\--- task \--- Κάνε τα φώτα να αναβοσβήνουν επανειλημμένα ως ουράνιο τόξο σε ένα βρόχο.

Για να επαναλαμβάνεις αυτό το μοτίβο του ουράνιου τόξου για πάντα, χρησιμοποίησε:

```blocks3
forever
```

\--- /task \---

\--- challenge \---

+ Κάνε το ουράνιο τόξο να αναβοσβήνει με ένα μοτίβο της επιλογής σου.

## \--- collapse \---

## title: Rainbow challenges

Try out the following ideas:

1) Make the LEDs blink very fast and very slow 2) Make the whole rainbow blink 3) Make pairs of LEDs light up in alternate patterns 4) Make the rainbow blink something in Morse code 5) Make the rainbow do different things in response to different events

\--- /collapse \--- \--- /challenge \---