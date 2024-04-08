
```
Algorithm KruskalMST(G)  
	for each vertex V in G do  
		define a Cloud(v) of <- {v}
		  
	let Q be a priority queue.  
	Insert all edges into Q using their weights as the key  
	T <- empty  
	
	while T has fewer than n-1 edges do  
	
		edge e = T.removeMin()  
		
		Let u, v be the endpoints of e  
		
		if Cloud(v) != Cloud(u) then  
			Add edge e to T  
			Merge Cloud(v) and Cloud(u)  
return T
```