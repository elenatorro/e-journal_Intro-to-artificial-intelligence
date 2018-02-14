# Problem Solving

What is a problem?

A problem can be broken down into a number of components.

1. Initial State *S*.
2. Actions *A*. Functions that get a state as an input and returns a set of possible actions. We have to consider that:
  - An agent can have the same actions for a given state.
  - An agent can have different actions for a given state.
3. Result *R*. Function which takes as input a state and a action, and delivers a new state.
4. Goal Test *GT*. Function that takes as input a state and returns a boolean value which means if the given state is rather a goal or not (*Condition of Success*)
5. Cost Action *CA*: Function which takes a **sequence** of **state action transitions** and returns a value, which is the cost of this action.

*Note: States are also all relevant aspects of the problem*
