# Peg Solitaire

Description:

Peg solitaire (or Solo Noble) is a board game for one player involving movement of pegs on a board with holes. Some sets use marbles in a board with indentations. The game is known simply as Solitaire in the United Kingdom where the card games are called Patience. It is also referred to as Brainvita (especially in India).

The first evidence of the game can be traced back to the court of Louis XIV, and the specific date of 1687, with an engraving made that year by Claude Auguste Berey of Anne de Rohan-Chabot, Princess of Soubise, with the puzzle by her side. The August 1687 edition of the French literary magazine Mercure galant contains a description of the board, rules and sample problems. This is the first known reference to the game in print.

The standard game fills the entire board with pegs except for the central hole. The objective is, making valid moves, to empty the entire board except for a solitary peg in the central hole.

[Wikipedia](https://en.wikipedia.org/wiki/Peg_solitaire)

* Board

```
         [ ][ ][ ]
         [ ][ ][ ]
         [ ][ ][ ]
[ ][ ][ ][ ][ ][ ][ ][ ][ ]
[ ][ ][ ][ ][ ][ ][ ][ ][ ]
[ ][ ][ ][ ][ ][ ][ ][ ][ ]
         [ ][ ][ ]
         [ ][ ][ ]
         [ ][ ][ ]
```

* Initial State: All the pieces are placed except the center piece:

```
         [0][0][0]
         [0][0][0]
         [0][0][0]
[0][0][0][0][0][0][0][0][0]
[0][0][0][0][ ][0][0][0][0]
[0][0][0][0][0][0][0][0][0]
         [0][0][0]
         [0][0][0]
         [0][0][0]
```

Answer the following questions?

1. Is it partially observable?

* [ ] Yes
* [x] No

It is fully observable because you can always see the entire environment state.

2. Is it stochastic?

* [ ] Yes
* [x] No

It is not stochastic because you always know the result state of an action.

3. Is it continuous?

* [ ] Yes
* [x] No

It is not continuous because it has limits.

3. Is it adversarial?

* [ ] Yes
* [x] No

It is not adversarial because you are playing with yourself (it is a solitaire game) and you do not want to contradict yourself!.
