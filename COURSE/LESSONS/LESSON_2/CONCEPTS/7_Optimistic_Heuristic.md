# Sliding Blocks Puzzle

```
[ 1][ 2][ 3][ 4]

[ 5][ 6][ 7][ 8]

[ 9][10][11][12]

[13][14][15][XX]
```

The following blocks can be slide around, and the goal is to get to a certain position for each block (*configuration*).

We can think about two heuristics to see if they are rather optimistic or not:

* h1:
* h2:

## Creating heuristics

If we give an heuristic function to the AI (the intelligence comes from the outside)... then it's not that intelligent, right?

**How can the AI come up with its own heuristic function?**

Given a description, the AI should come up with an heuristic function.

"Generating a relaxed problem":

* We take the original problem (h) where is hard to move squares around.
* We make it easier by relaxing one of the constraints (h2).
* We keep relaxing the problem (h1) as if we were adding new operators.
* It means that by adding new operators, it makes the problem easier.
* Thus, it never **overestimates**.
* Thus, it is **admissible**.

> h: A block can move to square A to square B if:
- A and B are adjacents
- B is blank

> h2: A block can move to square A to square B if:
- A and B are adjacents
- ~~B is blank~~


> h1: A block can move to square A to square B if:
- ~~A and B are adjacents~~
- ~~B is blank~~


`h = max(h1, h2)`
