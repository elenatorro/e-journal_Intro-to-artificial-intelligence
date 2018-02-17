# Search Comparison

## Breadth First Search
*ES: Búsqueda en anchura*

```
          [1]
         /   \
      [2]     [3]
     /   \   /   \
  [4]   [5] [6]  [7]
```

Optimal to find the shortest path?
[x] Yes
[ ] No

Yes because it is always expanding in the shortest paths first. Wherever the goal is hiding, it will find it by examining no longer paths. (In other words, always checks short paths first).

## Cheapest First / Uniform Search

```
          [1]
        5/   \2
      [4]     [2]
    3/   \2  4/   \2
  [7]   [6] [5]   [3]
```

Optimal to find the shortest path?
[x] Yes
[ ] No

## Depth First Search
*ES: Búsqueda en profundidad*

```
          [1]
         /   \
      [2]     [5]
     /   \   /   \
  [3]   [4] [6]   [7]
```
Optimal to find the shortest path?
[ ] Yes
[x] No

It goes as deep as it can first. It does not necessary find the shortest past, since it can find the goal in node 4, for instance, while there is a shortest path that ends up in node 7.
