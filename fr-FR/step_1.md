From the `Input`{:class="microbitinput"} menu, drag the `on button pressed`{:class="microbitinput"} block into the workspace.

There are **three** options to choose from the drop-down menu:

1. `on button A pressed`{:class="microbitinput"} will trigger when button A is pressed
2. `on button B pressed`{:class="microbitinput"} will trigger when button B is pressed
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

Run your code, and when you press the buttons, you should see or hear the different outputs.
