# Greedy Best First Search

## A* Search

- Always expanding the path that has a minimum value of the function `f` which is the sum of the values `g` and `h` functions.
- Where:
  * `g` is the path cost. Minimizing g, helps us keep the path short.
  * `h` (heuristic) is the value of the state, which is the estimated distance to the goal. Minimizing h makes us keep focused on finding the goal.

> `[State] ------ g ------ [X] * * * * h * * * * * [Goal]`

The result will be the best strategy possible: it finds the shortest path while expanding the minimum number of paths possible.

However, A* algorithm won't always find the shortest path. It depends on the `h` function.

** `h` is 
* `h(state) < true cost of the path to the goal through that state`
* **We want the h to never underestimate the distance to the goal**
* h is optimistic
* h is admissible (to find the lowest cost path)
