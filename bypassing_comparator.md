# Bypassing Comparator Function for Sorting
Most often we can avoid making a comparator function and solve the problem more easily. The key is to manipulate the array in such a way that the default ascending sort does the work of descending sort too. The idea is demonstrated in the following examples.

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