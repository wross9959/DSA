```
Algorithm quadraticProbingInsertItem(h, itm):  
	Input: h is an array of size N itm is an Item with a key and an element.  
	Output: None.  
	
	k = itm.key()  
	probe = f(k)  
	j = 1 
	 
	while (h[probe] is occupied) do {  
		probe = (f(k) + (j*j) mod N) mod N  
		j = j + 1  
	}  
	h[probe] = itm
```