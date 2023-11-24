From the `Input`{:class="microbitinput"} menu, drag the `on button pressed`{:class="microbitinput"} block into the workspace.

There are **three** options to choose from the drop-down menu:

1. `wanneer knop A wordt ingedrukt`{:class="microbitinput"} wordt geactiveerd wanneer knop A wordt ingedrukt
2. `wanneer knop B wordt ingedrukt`{:class="microbitinput"} wordt geactiveerd wanneer knop B wordt ingedrukt
3. `on button A + B pressed`{:class="microbitinput"} will trigger when buttons A and B are pressed at the same time

```microbit
input.onButtonPressed(Button.A, function () {
	
})
input.onButtonPressed(Button.AB, function () {
	
})
input.onButtonPressed(Button.B, function () {
	
})
```

You can add the action you want to happen within the `on button pressed`{:class="microbitinput"} block.

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

Voer je code uit en wanneer je op de knoppen drukt, zou je de verschillende uitgevoerde acties moeten zien of horen.
