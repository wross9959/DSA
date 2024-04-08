```
Algorithm BaruvkaMST(G)  
	T <- V {just the vertices of G}  
	while T has fewer than n-1 edges do  
		for each connected component C in T do  
			Let edge e be the smallest-weight edge from C to another component in T.  
			if e is not already in T then  
				Add edge e to T  
	return T
```