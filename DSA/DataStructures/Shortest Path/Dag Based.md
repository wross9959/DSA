```
Algorithm DagDistances(G, s)  
	for all v in G.vertices()  
		if v = s  
			setDistance(v, 0)  
		else  
			setDistance(v, inf)  
			
	Perform a topological sort of the vertices  
	for u <- 1 to n do {in topological order}  
		for each e in G.outEdges(u)  
			{ relax edge e }  
			z <- G.opposite(u,e)  
			r <- getDistance(u)  + weight(e)  
			if r < getDistance(z)  
				setDistance(z,r)
```