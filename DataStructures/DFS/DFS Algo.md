
```
Algorithm DFS(G)  
	Input graph G  
	Output labeling of the edges of G as discovery edges and back edges
	
	for all u in G.vertices()  
		setLabel(u, UNEXPLORED) 
		 
	for all e in G.edges()  
		setLabel(e, UNEXPLORED) 
		 
	for all v in G.vertices()  
		if getLabel(v) = UNEXPLORED  
			DFS(G, v)

Algorithm DFS(G, v)  
	Input graph G and a start vertex v of G  
	Output labeling of the edges of G in the connected component of v as discovery edges and back edges
	
	setLabel(v, VISITED)  
	
	for all e in G.incidentEdges(v)  
		if getLabel(e) = UNEXPLORED  
			w <- opposite(v,e)  
			if getLabel(w) = UNEXPLORED  
				setLabel(e, DISCOVERY)  
				DFS(G, w)  
			else  
				setLabel(e, BACK)

```