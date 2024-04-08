
```
Algorithm mergeSort(S, C)  
	Input sequence S with n elements, comparator C  
	Output sequence S sorted according to C  
	
	if(S.size() > 1)  
		(S1, S2) <- partition(S, n/2)  
		mergeSort(S1, C)  
		mergeSort(S2, C)  
		S <- merge(S1, S2)
```
O(nlogn)

Used for:
- fast  
- sequential data access  
- for huge data sets (> 1M)

Merge-sort on an input sequence S with n elements consists of three steps:  
- **Divide**: partition S into two sequences S1 and S2 of about n/2 elements each  
- **Recur**: recursively sort S1 and S2  
- **Conquer**: merge S1 and S2 into a unique sorted sequence