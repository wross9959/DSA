

```
Algorithm PQ-Sort(S, C)  
	Input sequence S, comparator C for the elements of S  
	Output sequence S sorted in increasing order according to C P <- priority queue with comparator C  
		
	while !S.isEmpty ()  
		e <- S.remove (S. first())  
		P.insertItem(e, e)  
	while !P.isEmpty()  
		e <- P.removeMin()  
		S.insertLast(e)
```