```
Algorithm linearProbingInsertItem(h, itm):  
	Input: h is an array of size N itm is an Item with a key and an element.  
	Output: None.  
	
	k = itm.key()  
	probe = f(k)  
	
	while (h[probe] is occupied) do {  
		probe = (probe + 1) mod N  
	}  
	h[probe] = itm  
	
• Operations: put(k,v), get(k), remove(k)  
• Lookups walk along table until the key or an empty slot is found  
• Uses less memory than chaining - don’t have to store all those links  
• Slower than chaining - may have to walk along table for a long way  
• A real pain to delete from - mark the deleted slot
```