# Concept of Binary Search with range notation
> Please read [range notation of subarray](../array/subarray.md) if you haven't yet.

You will be given an array, $A$ of size $n$. The range of index of the array is `[0,n)`. For binary search you have to do the following:

**Step-1:** Define left, `l` and right, `r`, such that `[l,r)` represents the array on which you will do binary search. Initially `l=0` and `r=n`

**Step-2:** Find the mid point, `mid`.

**Step-3:** Divide the array into three
1. `[l,mid)`
1. `mid`
1. `[mid+1,r)`

**Step-4:** 
1. If `mid` is the result, you found it. 
1. Otherwise, either `[l,mid)` is good or `[mid+1,r)` is good. So, do binary search on the good.
   - if the good subarray is empty, exit.

# Overflow bug
* We often calculate mid using this formula: 
$mid=(L+R)/2$. But $L+R$ may overflow. So, we should always calculate mid using this formula:
  $$mid=L+(R−L)/2$$
  > Note: Here $/$ means floor division