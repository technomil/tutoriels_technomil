# Fais jouer "Au clair de la lune" à ton micro:bit!
Programme le Micro:bit pour qu'une mélodie joue lorsqu'un bouton est pressé.


## @showdialog
## Avant de commencer

## Étape 1
Glisse le bloc`` || input: lorsque le bouton A est pressé || ``

```blocks
input.onButtonPressed(Button.A, function ()

```
## Étape 2
Glisse le bloc`` || Music: jouer tonalité Middle C pour 1 temps jusqu'à la fin||`` dans le bloc `` || input: lorsque le bouton A est pressé || ``.

```blocks
input.onButtonPressed(Button.A, function () {
    music.play(music.tonePlayable(262, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
```
## Étape 3
Clique sur "Low C" (Do) et choisis la touche du piano "Low G" (Sol). 

```blocks
input.onButtonPressed(Button.A, function () {
    music.play(music.tonePlayable(196, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
```

## Étape 4
Duplique 2 fois le bloc `` || Music: jouer tonalité Low G pour 1 temps jusqu'à la fin||`` sous le premier bloc musical afin que ton Micro:bit joue "Sol-Sol-Sol".
#### Observe l'indice au besoin

```blocks
input.onButtonPressed(Button.A, function () {
    music.play(music.tonePlayable(196, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
    music.play(music.tonePlayable(196, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
    music.play(music.tonePlayable(196, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
```

## Étape 5
Ajoute un autre bloc `` || Music: jouer tonalité Middle C pour 1 temps jusqu'à la fin||`` sous les 3 premiers.
#### Modifie Low C (Do) pour Low A (La).

```blocks
input.onButtonPressed(Button.A, function () {
    music.play(music.tonePlayable(196, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
    music.play(music.tonePlayable(196, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
    music.play(music.tonePlayable(196, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
    music.play(music.tonePlayable(220, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
```

## Étape 6
Ajoute un autre bloc `` || Music: jouer tonalité Middle C pour 1 temps jusqu'à la fin||`` sous les 3 premiers.
#### Modifie Low C (Do) pour Low B (Si) et 1 pour 2.

```blocks
input.onButtonPressed(Button.A, function () {
    music.play(music.tonePlayable(196, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
    music.play(music.tonePlayable(196, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
    music.play(music.tonePlayable(196, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
    music.play(music.tonePlayable(220, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
    music.play(music.tonePlayable(247, music.beat(BeatFraction.Double)), music.PlaybackMode.UntilDone)
    })
```

## Étape 7
Ajoute un dernier bloc `` || Music: jouer tonalité Middle C pour 1 temps jusqu'à la fin||`` sous les 3 premiers.
#### Modifie Low C (Do) pour Low G (Sol) et 1 pour 2.

```blocks
input.onButtonPressed(Button.A, function () {
    music.play(music.tonePlayable(196, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
    music.play(music.tonePlayable(196, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
    music.play(music.tonePlayable(196, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
    music.play(music.tonePlayable(220, music.beat(BeatFraction.Whole)), music.PlaybackMode.UntilDone)
    music.play(music.tonePlayable(247, music.beat(BeatFraction.Double)), music.PlaybackMode.UntilDone)
    music.play(music.tonePlayable(220, music.beat(BeatFraction.Double)), music.PlaybackMode.UntilDone)
})
```

### Voilà! Tu as réussi!
Amuse-toi à essayer de créer la suite de la chanson "Au clair de la lune". Les 5 prochaines notes sont: Sol-Si-La-La-Sol.

