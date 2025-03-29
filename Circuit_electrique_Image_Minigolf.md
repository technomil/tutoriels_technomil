# Afficher une image grâce à un circuit électrique
Programme le micro:bit pour qu'un bonhomme sourire apparaisse lorsqu'un circuit électrique est fermé.


## @showdialog
## Avant de commencer

Supprime le bloc ``||basic:au démarrage||``.
#### Glisse-le vers la gauche, tu verras apparaître une poubelle

```blocks
basic.forever(function ()
})
```

## Étape 1
Place le bloc ``||basic:afficher LEDs||`` dans le bloc ``||basic:au démarrage||``
#### Dessine le chiffre 0
```blocks
basic.showLeds(`
    . # # # .
    . # . # .
    . # . # .
    . # . # .
    . # # # .
    `)
    ```
## Étape 2
Place le bloc ``|input:lorsque la broche est activé||``
#### Choisis la broche P1.
```blocks

input.onPinPressed(TouchPin.P1, function () {
	
})
```

## Étape 3
Place le bloc ``||basic:afficher LEDs||`` dans le bloc ``|input:lorsque la broche est activé||``
#### Dessine un bonhomme sourire
```blocks
input.onPinPressed(TouchPin.P1, function () {
    basic.showLeds(`
        . # . # .
        . # . # .
        # . . . #
        # . . . #
        . # # # .
        `)
})
```
