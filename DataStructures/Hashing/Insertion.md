```
Algorithm InsertItem(h, itm):  
	Input: h is an array of size N itm is an Item with a key and an element.  
	Output: None. 
	 
	Let B be a linked list.  
	
	k = itm.key()  
	i = f(k)  
	
	if h[i] is empty then{  
		h[i] = new LinkedList B  
	}  
	else{  
		B = h[i]  
	}  
	B.insertLast(itm)  
}
```