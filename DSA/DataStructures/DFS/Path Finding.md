```
Algorithm pathDFS(G, v, z)  

	setLabel(v, VISITED)  
	S.push(v)  
	
	if v = z  
		return S.elements()  
		
	for all e in G.incidentEdges(v)  
	
		if getLabel(e) = UNEXPLORED  
			w <- opposite(v,e)  
			
			if getLabel(w) = UNEXPLORED  
			
				setLabel(e, DISCOVERY)  
				S.push(e)  
				pathDFS(G, w, z)  
				S.pop(e)  
				
			else  
				setLabel(e, BACK)  
	S.pop(v)
```