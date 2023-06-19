# Subarray
**Definition:** Contguous part of an array.

## Notation
It is helpful to denote the range of index of subarray as `[start, end)`\
**Example:** Index range of subarray `[d,e,f]` of the array `[a,b,c,d,e,f,g]` is `[3,6)`
### Why its useful
- Length of the array: `len = end - start`
- Print all elements: `for(int i=start; i<end; i++)`
- Easy migration to python

## Number of subarrays
- Number of non-empty subarrays of an array of size $n$ is $\frac{n(n+1)}{2}$
- Number of subarrays of an array of size $n$ is $\frac{n(n+1)}{2}+1$
