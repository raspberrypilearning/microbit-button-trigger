Dans le menu `Entrée`{:class="microbitinput"}, fais glisser le bloc `lorsque le bouton est pressé`{:class="microbitinput"} dans l'espace de travail.

Il y a **trois** options à choisir dans le menu déroulant :

1. `lorsque le bouton A est pressé`{:class="microbitinput"} se déclenchera lorsque le bouton A est enfoncé
2. `lorsque le bouton B est pressé`{:class="microbitinput"} se déclenchera lorsque le bouton B est enfoncé
3. `lorsque le bouton A + B est pressé`{:class="microbitinput"} se déclenchera lorsque le bouton A et B sont enfoncés en même temps

```microbit
input.onButtonPressed(Button.A, function () {
	
})
input.onButtonPressed(Button.AB, function () {
	
})
input.onButtonPressed(Button.B, function () {
	
})
```

Tu peux ajouter l'action que tu souhaites voir se produire dans le bloc `lorsque le bouton est pressé`{:class="microbitinput"}.

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

Exécute ton code et lorsque tu appuies sur les boutons, tu devrais voir ou entendre les différentes sorties.
