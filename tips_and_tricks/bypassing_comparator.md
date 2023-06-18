# Bypassing Comparator Function for Sorting
The default sort function in C++ sorts the array in ascending order. If you follow the following steps it will sort it in descending order:\
**Step-1:** `for(int&it:a) it*=-1;`\
**Step-2:** `sort(a,a+n);`\
**Step-3:** `for(int&it:a) it*=-1;`
> Read [Problem 1](#problem-1) and [Problem 2](#problem-2) to understand the concept, and red [Problem 3](#problem-3) to understand why it is applicablle

## Problem 1
Sort an array of $n$ integers in ascending order

### Input
$n$\
$A_1\space A_2\space A_3\space A_4\space ...\space A_n$

### Solution
```c++
int n; cin>>n;
int a[n];
for(int&it:a) cin>>it;
sort(a,a+n);
for(int&it:a) cout<<it<<" ";
```

## Problem 2
Sort an array of $n$ integers in descending order

### Input
$n$\
$A_1\space A_2\space A_3\space A_4\space ...\space A_n$

### Solution
```c++
int n; cin>>n;
int a[n];
for(int&it:a) {
  int temp; cin>>temp;
  it=-temp;
}
sort(a,a+n);
for(int&it:a) cout<<-it<<" ";
```

## Problem 3
Sort an array of $n$ pair of integers in descending order of the first element and break tie with ascending order of second element

### Input
$n$\
$P_1\space Q_1$\
$P_2\space Q_2$\
$...$\
$P_n\space Q_n$

### Example
Input
```
5
2 4
2 3
1 0
1 1
```
Output
```
1 1
1 0
2 4
2 3
```

### Solution
```c++
int n; cin>>n;
pair<int,int> a[n];
for(auto&it:a) {
  int p; cin>>p;
  int q; cin>>q;
  it={-p,q};
}
sort(a,a+n);
for(auto&[p,q]:a) cout<<-p<<" "<<q<<"\n";
```