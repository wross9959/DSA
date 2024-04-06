```
Algorithm doubleHashingInsertItem(h, itm):  
	Input: h is an array of size N itm is an Item with a key and an  
	element.  
	Output: None.  
	
	k = hash(itm.key())  
	probe = f1(k)  
	offset = f2(k)  
	
	while (h[probe] is occupied) do {  
		probe = (probe + offset) mod N  
	}  
	
	h[probe] = itm
```