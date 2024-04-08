```
Algorithm DijkstraDistances(G, s)  
	Q <- new heap-based priority queue 
	 
	for all v in G.vertices()  
		if v = s  
			setDistance(v, 0)  
		else  
			setDistance(v, inf)  
			
		l <- Q.insert(getDistance(v), v)  
		setLocator(v,l)  
			
	while !Q.isEmpty()  
		u <- Q.removeMin()  
		for all e in G.incidentEdges(u)  
			{ relax edge e }  
			z <- G.opposite(u,e)  
			r <- getDistance(u) weight(e)  
			if r < getDistance(z)  
				setDistance(z,r)  
				Q.replaceKey(getLocator(z),r)
```