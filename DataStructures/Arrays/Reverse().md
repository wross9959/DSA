```

Alg: reverseArr(A[], start, end)
	In:
	Out:
	If (start >= end) return;
	
	Swap A[start] with A[end]
	
	reverseArray(A, start+1, end-1)

O(n/2) -> O(n)
```