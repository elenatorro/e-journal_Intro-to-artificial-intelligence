# Concepts

## Agent, Sensors, Activators

How does an agent make decissions to use its actuators depending on the sensors data?

* An **Agent** interacts with an **Environment**.
* The Agent perceives the state of the Environment through **Sensors**.
* Changes its state through **Actuators**
* Control Policy for the agent: the function that connects sensors to activators.

## Perception Action Cycle

The perception-action cycle is the circular flow of information that takes place between the organism and its **environment** in the course of a sensory-guided sequence of behavior towards a goal.

Environments can be:
* Fully Observable or Partially Observable
* Deterministic or Stochastic
* Discrete or Continuous
* Benign or Adversarial

## Fully vs Partially Observable Environments

* An environment is fully observable if the sensors always see the entire **Environment State**.
* Agents that deal with Partially Observable Environments need a **memory** component to understand the state.

## Deterministic vs Stochastic Environments

* Deterministic Environment: You need to determine de outcome of the agents' actions.
* *A **chess** game is deterministic, a **dices** game is stochastic*.
* *An environment is deterministic if the next state is perfectly predictable given knowledge of the previous state and the agent's action.*

## Discrete vs Continuous Environments

* A discrete environment has fixed locations or time intervals (it has limits). It deterministic if there is a limited number of actions you can do.
* A continuous environment could be measured quantitatively to any level of precision (it does not have limits).

## Benign vs Adversarial
*[ES] Favorable vs En condiciones adversas*

* Benign: could be random **or** stochastic, but has no objective on its own that would contradict your own objective.
* Adversarial: try to contract what you are trying to achieve.
* *A **chess** game is adversarial*.
