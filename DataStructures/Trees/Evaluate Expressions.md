```
Algorithm evalExpr(v)  
	if isExternal (v)  
		return v.element ()  
	else  
		x <- evalExpr(leftChild(v)) 
		y <- evalExpr(rightChild(v))  
		
		z <- operator stored at v  
		
	return x z y
```