# Basic Format
In the following code sections,\
`len` is the size of the window\
`start` is the start of the window\
The window is represented by `[start,start+len)`
```c++
for(int start=0, len; start<n; start+=len) {
  len=0;
  while(start+len<n && condition) len++;
  // code...
}
```

# Sample Problem
Given an array $A$ of length $n$  find the maximum length of equal consecuitive numbers.

## Constaints
$1\leq n\leq 10^5$\
$1\leq A_i\leq 10^9$

## Input:
$n$\
$A_1\space A_2\space ...\space A_n$

## Example:
| Input                | Output |
| -------------------- | ------ |
| 8<br>1 2 2 1 2 2 2 1 | 3      |
| 8<br>2 2 2 1 1 1 1 2 | 4      |
| 7<br>1 2 3 4 1 2 3   | 1      |

## Solution
```c++
int n; cin>>n;
int a[n]; for(int &it: a) cin>>it;
int mx_cnt=0;
for(int i=0, j; i<n; i=j) {
  for(j=i; j<n && a[i]==a[j]; j++);
  mx_cnt=max(cnt,mx_cnt);
}
```

## Example Problems:
1. [Array Merging](https://codeforces.com/contest/1831/problem/B) - [Solution](https://codeforces.com/contest/1831/submission/208058751)