```
Algorithm PrimJarnikMST(G)  
	Q <- new heap-based priority queue  
	s <- a vertex of G  
	
	for all v in G.vertices()  
		if v = s  
			setDistance(v, 0)  
		else  
			setDistance(v, inf)
			  
		setParent(v, empty)  
		l <- Q.insert(getDistance(v), v)  
		setLocator(v,l)  
		
	while !Q.isEmpty()  
		u <- Q.removeMin()  
		
		for all e in G.incidentEdges(u)  
			z <- G.opposite(u,e)  
			r <- weight(e)  
			
			if r < getDistance(z)  
				setDistance(z,r)  
				setParent(z,e)  
				
	Q.replaceKey(getLocator(z),r)
```