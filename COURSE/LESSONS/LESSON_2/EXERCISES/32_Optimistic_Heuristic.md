# Optimistic Heuristic

Let's say we have a cleaning robot:

1. Cleaning
2. No Cleaning

Each state:
1. Power switch: on, off, sleep (3)
2. Dirt camera: on, off (2)
3. Brushes: 5 different highs (5)
4. Positions: 10 (10)

How many states in this state space exist?

* Try 1: **wrong**
Number of parameters:
1 + 3 + 2 + 5 + 10 = 21
2^21 = 2097152

* Try 2: **wrong**
2^4 + 2^3 + 2^6 + 2^11 = 16 + 8 + 64 + 2048 = 2136

* Try 3: **wrong**
2^4 * 2^3 * 2^6 * 2^11 = 16 * 8 * 64 * 2048 = 16777216

* Correct solution:
3 * 2 * 5 * 2^10 * 10 = 307200

**Note**: difference between variables and positions.
