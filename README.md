## BFS Program

```python
graph = {
    'A': ['B', 'C'],
    'B': ['D'],
    'C': ['E'],
    'D': [],
    'E': []
}

visited = []
queue = ['A']

while queue:
    node = queue.pop(0)
    if node not in visited:
        print(node, end=" ")
        visited.append(node)
        queue.extend(graph[node])
```

START

BFS:
Add starting node to queue
Mark it as visited
While queue is not empty
    Remove node from queue
    Visit node
    Add unvisited neighbors to queue

DFS:
Visit current node
Mark it as visited
For each unvisited neighbor
    Recursively visit neighbor

STOP
