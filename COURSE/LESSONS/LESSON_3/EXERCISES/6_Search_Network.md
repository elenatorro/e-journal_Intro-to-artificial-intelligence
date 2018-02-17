# Search Network

Given the following graph:

```
           [A]
         /     \
       [ ]     [ ]
      /   \   /   \
   [ ]     [ ]     [ ]
   /  \   /   \   /   \
 [ ]   [ ]     [ ]    [B]
   \  /   \   /   \   /
   [ ]     [ ]     [ ]
      \   /   \   /
       [ ]     [ ]
          \   /
           [ ]
```

Assumptions:
1. Our search never expands a node twice.
2. Start node is A and Goal Node is B

How many nodes will be expanded from A to B?


Left-To-Right
* Breadth First => 10

```
           [1]
         /     \
       [2]     [3]
      /   \   /   \
   [4]     [5]     [6]
   /  \   /   \   /   \
 [7]   [8]     [9]    [10]
   \  /   \   /   \   /
   [ ]     [ ]     [ ]
      \   /   \   /
       [ ]     [ ]
          \   /
           [ ]
```

* Depth First => 16

```
           [1]
         /     \
       [2]     [14]
      /   \   /   \
   [3]     [11]    [15]
   /  \   /   \   /   \
 [4]   [8]     [12]    [16]
   \  /   \   /   \   /
   [5]     [9]     [13]
      \   /   \   /
       [6]     [10]
          \   /
           [7]
```

Right-To-Left
* Breadth First => 7

```
           [1]
         /     \
       [3]     [2]
      /   \   /   \
   [6]     [5]     [4]
   /  \   /   \   /   \
 [ ]   [ ]     [ ]    [7]
   \  /   \   /   \   /
   [ ]     [ ]     [ ]
      \   /   \   /
       [ ]     [ ]
          \   /
           [ ]
```

* Depth First => 4

```
           [1]
         /     \
       [ ]     [2]
      /   \   /   \
   [ ]     [ ]     [3]
   /  \   /   \   /   \
 [ ]   [ ]     [ ]    [4]
   \  /   \   /   \   /
   [ ]     [ ]     [ ]
      \   /   \   /
       [ ]     [ ]
          \   /
           [ ]
```
