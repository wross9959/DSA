
```
Algorithm BellmanFord(G, s)  
	for all v in G.vertices()  
		if v = s  
			setDistance(v, 0)  
		else  
			setDistance(v, inf)
			  
	for i <- 1 to n-1 do  
		for each e in G.edges()  
			{ relax edge e }  
			u <- G.origin(e)  
			z <- G.opposite(u,e)  
			r <- getDistance(u) weight(e)  
			if r < getDistance(z)  
				setDistance(z,r)
```