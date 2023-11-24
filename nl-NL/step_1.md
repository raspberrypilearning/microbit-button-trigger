Sleep vanuit het `Invoer`{:class="microbitinput"} menu een `wanneer knop wordt ingedrukt`{:class="microbitinput"} blok in het bewerkingspaneel.

Er zijn **drie** opties waaruit je kunt kiezen in het vervolgkeuzemenu:

1. `wanneer knop A wordt ingedrukt`{:class="microbitinput"} wordt geactiveerd wanneer knop A wordt ingedrukt
2. `wanneer knop B wordt ingedrukt`{:class="microbitinput"} wordt geactiveerd wanneer knop B wordt ingedrukt
3. `wanneer knop A+B wordt ingedrukt`{:class="microbitinput"} wordt geactiveerd wanneer knop A en B tegelijkertijd worden ingedrukt.

```microbit
input.onButtonPressed(Button.A, function () {
	
})
input.onButtonPressed(Button.AB, function () {
	
})
input.onButtonPressed(Button.B, function () {
	
})
```

Binnen het `wanneer knop wordt ingedrukt`{:class="microbitinput"} blok kun je de actie toevoegen die je wilt doen.

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
