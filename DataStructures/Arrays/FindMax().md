```
Alg: findMax(A[], x, index)
	Input: 
	Output: 
	
	If (A.isEmpty() || index > length(A)) return false;
	
	If (A.length = 1) return A[index];
	
	Max = maxArr[A, x, index+1))
	
	If A[index] > max; return A[index]
		Return max;
		
	Return searchArr(Arr, x, index++)
	
```

```
Alg: arrMax(A[], n)

	Current max <- A[0]
	
	For I <- 1 to n-1 do
		If (A[i] > currentMax) then
			currentMax <- A[i]
			
	Return currentMax
```