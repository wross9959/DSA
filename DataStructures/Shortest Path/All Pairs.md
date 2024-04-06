
```
Algorithm AllPair(G) {assumes vertices 1,...,n}  
	for all vertex pairs (i,j)  
		if i = j  
			D0[i,i] <- 0  
		else if (i,j) is an edge in G  
			D0[i,j] <- weight of edge (i,j)  
		else  
			D0[i,j] <- + inf  
			
	for k <- 1 to n do  
		for i <- 1 to n do  
			for j <- 1 to n do  
				Dk[i,j] <- min{Dk-1[i,j], Dk-1[i,k] + Dk1[k,j]}  
	return Dn
```