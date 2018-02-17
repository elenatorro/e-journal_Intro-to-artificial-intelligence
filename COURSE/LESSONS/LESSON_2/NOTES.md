# Notes

## Search Algorithms

Personal notes on how I'd implement search algorithms in JavaScript.

### Tree Search

```js
function Node() = {
  links: [],
  visited: false,
  start: '',
  end: '',
  value: ''
}
```

```js
const InitialState = {
  city: '',
  path: 0,
  cost: 0,
  frontier: [],
  explored: []
}
```

```js
const Problem = {
  state: {},
  actions: [],
  result: function () {},
  goal: function() {}
}
```

```js
function treeSearch(problem, nodes) {
  let frontier = [ nodes[startNode] ];

  while(frontier.length) {
    const state = problem.state;  
    const node = frontier.shift();

    if (problem.goal(node.end)) return node;

    for(let action in problem.actions) {
      frontier.push(path);
      problem.result(action(state));
    }
  }
}
```

#### Breadth-First Search

```
const Paths = {
  Aral: {
    Zerind: {
      cost: 75
    },
    Sibiu: {
      cost: 140
    },
    Timisoara: {
      cost: 111
    }
  }
}

const InitialState = {
  city: 'Arad',
  path: 0,
  cost: 0,
  frontier: [],
  explored: []
}

const City = {
  NAME: '',
  neighbours: []
};

const GOAL_CITY = 'Bucharest';

const Path = {
  START: '', // City Name
  END: '' // City Name
};

function RemoveChoice(state) {}

function GoalTest(state) {
  return state.city.name === GOAL_CITY;
}

function Result(state, action) {}
```
