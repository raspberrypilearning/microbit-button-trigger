Από το μενού `Είσοδος`{:class="microbitinput"} σύρε το μπλοκ `όταν πιεστεί το πλήκτρο button`{:class="microbitinput"} στον χώρο εργασίας.

Υπάρχουν **τρεις** επιλογές για να επιλέξεις από το αναπτυσσόμενο μενού:

1. Το `όταν πιεστεί το πλήκτρο button Α`{:class="microbitinput"} θα προκληθεί όταν πατηθεί το κουμπί Α
2. Το `όταν πιεστεί το πλήκτρο button Β`{:class="microbitinput"} θα προκληθεί όταν πατηθεί το κουμπί Β
3. Το `όταν πιεστεί το πλήκτρο button Α+Β`{:class="microbitinput"} θα προκληθεί όταν πατηθούν τα κουμπιά Α και Β ταυτόχρονα

```microbit
input.onButtonPressed(Button.A, function () {
	
})
input.onButtonPressed(Button.AB, function () {
	
})
input.onButtonPressed(Button.B, function () {
	
})
```

Μπορείς να προσθέσεις την ενέργεια που θέλεις να πραγματοποιηθεί εντός του μπλοκ `όταν πιεστεί το πλήκτρο button`{:class="microbitinput"}.

```microbit
input.onButtonPressed(Button.A, function () {
    basic.showString("Hello!")
})
input.onButtonPressed(Button.B, function () {
    music.play(music.tonePlayable(262, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
})
input.onButtonPressed(Button.AB, function () {
    basic.showIcon(IconNames.Heart)
})
```

Εκτέλεσε τον κώδικά σου και όταν πατήσεις τα κουμπιά, θα πρέπει να δεις ή να ακούσεις τις διαφορετικές εξόδους.
