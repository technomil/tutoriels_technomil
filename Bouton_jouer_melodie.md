# Faire jouer une mélodie en pressant le bouton A
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
input.onButtonPressed(Button.A, function () {
    music.play(music.stringPlayable("C5 B A G F E D C ", 120), music.PlaybackMode.UntilDone)
})

```

 input.onButtonPressed(Button.A, function () {
    music.play(music.stringPlayable("- - - - - - - - ", 120), music.PlaybackMode.UntilDone)
})