```
Algorithm partition(S, p)  
	Input sequence S, position p of pivot  
	Output subsequences L, E, G of the elements of S less than, equal to, or greater than the pivot, resp. 
	 
	L, E, G <- empty sequences  
	x <- S.remove(p)  
	
	while (!S.isEmpty())
	
		y <- S.remove(S.first())  
		
		if y < x  
			L.insertLast(y)  
			
		else if y = x  
			E.insertLast(y)  
			
		else { y > x }  
			G.insertLast(y)  
			
	return L, E, G
```