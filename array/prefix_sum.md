# Prefix Sum
## Mukhosto Code
```cpp
int pf[n+1];
pf[0]=0;
for(int i=1; i<n; i++) pf[i]=pf[i-1]+a[i];
```
## TLE and Prefix Sum
Whenever you think there might be TLE in your solution and it is somehow related to prefix sum, then your the alarms of your brain should ring up. Because if the given array had all non-negative numbers, then the prefix sum should be sorted. Which means, you can use **binary search**.