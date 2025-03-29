# Faire jouer une mélodie en pressant un bouton
Programme le micro:bit pour qu'une mélodie joue lorsqu'un bouton est pressé.


## @showdialog
## Avant de commencer

## Étape 1
Glisse le bloc ``||input:lorsque le un bouton est pressé||``
 ```blocks
input.onButtonPressed(Button.A, function ()

```
## Étape 2
Glisse le bloc ``||Music:jouer mélodie au tempo 120bpm jusqu'à la fin||``

```blocks

let Temps = 0
input.onButtonPressed(Button.A, function () {
    Temps = 4
    for (let index = 0; index < 3; index++) {
        music.playTone(262, music.beat(BeatFraction.Quarter))
    }
})

```

 input.onButtonPressed(Button.A, function () {
    music.play(music.stringPlayable("- - - - - - - - ", 120), music.PlaybackMode.UntilDone)
})