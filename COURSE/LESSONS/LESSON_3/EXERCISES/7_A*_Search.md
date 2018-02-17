# A* Search

```
   1  2  3  4  5  6
a [4][4][4][3][2][1]
b [3][3][3][3][2][1]
c [2][2][2][2][2][1]
d [1][1][1][1][1][0]
```

Start point: **a1**
Goal point: **d6**

1. Is it admissable?

* [x] Yes
* [ ] No

Yes, because we know the value of each node, and the value of the goal is strictly underestimated.

2. Which one is the first node A* would expand?

* [x] b1 (because it's lower)
* [ ] a2

2. Which one is the second node A* would expand?

* [ ] b1
* [x] c1
* [ ] a2
* [ ] a3
* [ ] b2

2. Which one is the third node A* would expand?

* [x] d1
* [ ] c2
* [ ] c2
* [ ] b3
* [ ] a4
