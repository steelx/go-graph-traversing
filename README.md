# go-graph-traversing
Graph DFS and BFS implementation in golang

### Breadth First Search
![breadth_first_traversal](https://user-images.githubusercontent.com/3184210/70855231-ee168580-1ec7-11ea-82fe-78927fd8bcdb.jpg)
```
Algorithm BFS(G, v)
    Q ← new empty FIFO queue
    Mark v as visited.
    Q.enqueue(v)
    while Q is not empty
        a ← Q.dequeue()
        // Perform some operation on a.
        for all unvisited neighbors x of a
            Mark x as visited.
            Q.enqueue(x)
```
[BFS visualization](https://www.cs.usfca.edu/~galles/visualization/BFS.html)


### Depth First Search
![dfs](https://user-images.githubusercontent.com/3184210/70855249-3d5cb600-1ec8-11ea-98c3-e692f30dd5f0.gif)
```
Algorithm DFS(G, v)
    if v is already visited
        return        
    Mark v as visited.
    // Perform some operation on v.
    for all neighbors x of v
        DFS(G, x)
```
[DFS visualization](https://www.cs.usfca.edu/~galles/visualization/DFS.html)
