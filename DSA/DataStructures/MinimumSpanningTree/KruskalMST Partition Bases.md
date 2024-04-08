
```
Algorithm Kruskal(G):  
	Input: A weighted graph G.  
	Output: An MST T for G.  
	Let P be a partition of the vertices of G, where each vertex forms a separate set.  
	Let Q be a priority queue storing the edges of G, sorted by their weights  
	Let T be an initially-empty tree  
	
	while Q is not empty do  
		(u,v) <- Q.removeMinElement()  
		if P.find(u) != P.find(v) then  
			Add (u,v) to T  
			P.union(u,v)  
	return T
```

Running time:  
O((n+m)log n)