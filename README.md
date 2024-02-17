# Lab Experiment1: Breadth First Search
## Write a Python program to implement breath First Search. 
```
graph = {
  '2': ['3', '4'],
  '3': ['5'],
  '4': ['6', '7'],
  '6': [],
  '5': ['6'],
  '7': ['8'],
  '8': []
}

visited = []  # List for visited nodes.
queue = []    # Initialize a queue

def bfs(visited, graph, node):  # Function for BFS
    visited.append(node)
    queue.append(node)

    while queue:  # Creating loop to visit each node
        m = queue.pop(0)
        print(m, end=" ")

        for neighbour in graph[m]:
            if neighbour not in visited:
                visited.append(neighbour)
                queue.append(neighbour)

# Driver Code
print("BFS order is")
bfs(visited, graph, '2')
```
## OUTPUT
![image](https://github.com/HibaRajarajeswari/BREATH-FIRST-SEARCH/assets/129970809/0933e32f-7995-4a6d-9040-034737cb946b)
## RESULT

A Python program to implement breath First Search is executed successfully.

