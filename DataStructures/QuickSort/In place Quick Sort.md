```
Algorithm inPlaceQuickSort(S, l, r)  
	Input sequence S, ranks l and r  
	Output sequence S with the elements of rank between l and r rearranged in increasing order  
	if l >= r  
		return  
		
	i <- a random integer between l and r  
	x <- S.elemAtRank(i)  
	
	(h, k) <- inPlacePartition(x) 
	 
	inPlaceQuickSort(S, l, h - 1)  
	inPlaceQuickSort(S, k + 1, r)
```