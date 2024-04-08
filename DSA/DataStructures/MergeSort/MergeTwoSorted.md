```
Algorithm merge(A, B)  
	Input sequences A and B with n/2 elements each  
	Output sorted sequence of A U B  
	
	S <- empty sequence  
	
	while (!A.isEmpty() && !B.isEmpty())  
		if (A.first().element() < B.first().element())  
			S.insertLast(A.remove(A.first()))  
		else  
			S.insertLast(B.remove(B.first()))  
	while !A.isEmpty()  
		S.insertLast(A.remove(A.first()))  
		
	while !B.isEmpty()  
		S.insertLast(B.remove(B.first()))  
		
	return S
```