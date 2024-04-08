```
Algorithm TreeSearch(k, v)  
	if T.isExternal (v)  
		return null  
		
	if k < key(v)  
		return TreeSearch(k, T.left(v))  
		
	else if k = key(v)  
		return v  
		
	else { k > key(v) }  
		return TreeSearch(k, T.right(v))
```