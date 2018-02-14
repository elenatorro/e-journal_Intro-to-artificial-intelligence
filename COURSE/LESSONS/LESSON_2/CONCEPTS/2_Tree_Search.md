# Tree Search

We're given the **Agent** the full map of Romania.

* We want to go from A (Arad) to B (Bucharest).
* In order to do that, we need to come up with a sequence of actions.

The structure of the problem is the following:

1. **Initial State**:
  We are in point A, Arad.
2. **Actions**:
  Given a city, we know its neighbours, but we can't go to other cities.
3. **Result**:
  Given:
    * A state *S* where the current city *c* is Arad.
    * An action *A* which is going along route *r* to city *c'*, Timisora.
    * The **result** *R* will be a new state where the Agent is in the city *c'*.

4. **Goal Test**:
  Function that returns true if we are in the destination city *dc*.
5. **Cost Action**:
  In this case, we want to know the cost of a Path from one city to another.
    * Function that returns the cost of this path, by given a sequence of state action transitions.
    * In this case, each action transition will return the cost of a path, and the Cost Action will be the sum of all of the costs.

In this problem, we want to separate the state into three parts:
* A Frontier Region: The ends of the paths.
* An Explored Region
* An Unexplored Region

**Tree Search** represents a whole family of algorithms. We are going to study the following algorithms to implement the search, which since a general approach to problem solving in AI is to reduce the problem to be solved to one of **searching a graph**. The main difference of these algorithms is how they choose of the next item on the frontier: which path do we look at first.

```
TreeSearch(problem p) returns path
  frontier = { path(p.initial) }
  loop:
    if frontier is empty : return FAIL
    path = removeChoice(frontier)
    s = path.end
    if GoalTest(s) : return path
    for a in p.Actions(s):
      Add [path + a -> Result(s, a)] to frontier
```
