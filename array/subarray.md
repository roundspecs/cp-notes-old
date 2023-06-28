# Subarray
**Definition:** Contguous part of an array.

## Notation
It is helpful to denote the range of index of subarray as `[start, end)`\
**Example:** Index range of subarray `[d,e,f]` of the array `[a,b,c,d,e,f,g]` is `[3,6)`\
It is important to note that you should only use one form of notation and always use that. If you think `[a,b]` is better, then always use that. Becuase you will use the same concept in many sectors like: prefix sum, binary search. If you use both notations, then you might get confused about which should be used where.
### Why its useful
|                                 | `[start,end)`                                                         | `[start,end]`                                |
| ------------------------------- | --------------------------------------------------------------------- | -------------------------------------------- |
| Length of the array             | `end - start`                                                         | `end - start + 1`                            |
| Array of size `n`               | `[0,n)`<br>Matches with 0-based index                                 | `[1,n]`<br>Does not match with 0-based index |
| Print all elements in the range | `for(int i=start; i<end; i++)`<br>Yes, you have already been using it | `for(int i=start; i<=end; i++)`              |
| Easy migration to python        | ✅                                                                     | ❎                                            |

## Number of subarrays
- Number of non-empty subarrays of an array of size $n$ is $\frac{n(n+1)}{2}$
- Number of subarrays of an array of size $n$ is $\frac{n(n+1)}{2}+1$
