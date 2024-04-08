```
Algorithm BFS(G)  
	Input graph G  
	Output labeling of the edges of G as discovery edges and back edges
	
	for all u in G.vertices()  
		setLabel(u, UNEXPLORED) 
		 
	for all e in G.edges()  
		setLabel(e, UNEXPLORED) 
		 
	for all v in G.vertices()  
		if getLabel(v) = UNEXPLORED  
			BFS(G, v)

Algorithm BFS(G, v)  
	Input graph G and a start vertex v of G  
	Output labeling of the edges of G in the connected component of v as discovery edges and back edges
	
	L0 <- new empty sequence  
	L0.insertLast(s)  
	
	setLabel(s, VISITED)  
	i <- 0  
	
	while !Li.isEmpty()  
		L(i+1) <- new empty sequence  
		for all v in Li.elements()  
			for all e in G.incidentEdges(v)  
				if getLabel(e) = UNEXPLORED  
					w <- opposite(v,e)  
					if getLabel(w) = UNEXPLORED  
						setLabel(e, DISCOVERY)  
						setLabel(w, VISITED)  
						L(i +1).insertLast(w)  
					else  
						setLabel(e, CROSS)
```