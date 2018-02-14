# Exercises

Initial State

```js
{
  city: 'Arad',
  path: 0,
  cost: 0,
  frontier: [],
  explored: []
}
```

## Tree Search


### Breadth-First Search

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
