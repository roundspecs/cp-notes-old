# Check how many times an integer divides another
Lets check how many times 2 and 3 divides a given integer N
```c++
int n=N;
int p=0,q=0;
while(n && n%2==0) n/=2, p++;
while(n && n%3==0) n/=3, q++;
```
$N=n\times 2^{p}\times 3^{q}$, where $2∤n$ and $3∤n$\
Time complexity: $O(\log_{3}(n))+O(\log_{2}(n))$

## Example Problems:
1. [Gold Rush](https://codeforces.com/contest/1829/problem/D) - [Solution](https://codeforces.com/contest/1829/submission/207916591)
2. [Game 23](https://codeforces.com/problemset/problem/1141/A) - [Solution](https://codeforces.com/contest/1141/submission/207946176)