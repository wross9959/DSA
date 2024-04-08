
```
Algorithm DijkstraShortestPathsTree(G, s)  
...  
	for all v in G.vertices()  
	...  
		setParent(v, inf)  
	...  
		for all e in G.incidentEdges(u)  
			{ relax edge e }  
			z <- G.opposite(u,e)  
			r <- getDistance(u) weight(e)  
			if r < getDistance(z)  
				setDistance(z,r)  
				setParent(z,e)  
				Q.replaceKey(getLocator(z),r)
```