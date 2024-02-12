# DFS--AI

## PROGRAM:
```
graph = {
  '5' : ['3','7'],
  '3' : ['2', '4'],
  '7' : ['8'],
  '2' : [],
  '4' : ['8'],
  '8' : []
}
visited = set()
def dfs(visited, graph, node):  #function for dfs 
    if node not in visited:
        print (node)
        visited.add(node)
        for neighbour in graph[node]:
            dfs(visited, graph, neighbour)
# Driver Code
print("Following is the Depth-First Search")
dfs(visited, graph, '5')
```


## OUTPUT:
![Screenshot (468)](https://github.com/ashmistalin/DFS--AI/assets/103128410/8685cc27-7b2b-410a-9c65-e0c4a77006be)
