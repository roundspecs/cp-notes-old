# Tuple
- Elements of tuple can be of different data type
- Built-in sort
  > Note: For sorting, the order of the data in tuple matters

## Read/Write element
```cpp
tuple<int, string, double> x;

// Write
cin>>get<0>(x);
get<1>(x)="Hello";
cin>>get<2>(x);
get<0>(x)++;

// Read
cout<<get<0>(x)+get<2>(x);
cout<<get<1>(x);
```

## Read/Write array of tuples
```cpp
tuple<int, string, double> a[n];
for(auto[a,b,c]:a) cin>>a>>b>>c;
for(auto[a,b,c]:a) cout<<a<<b<<c;
```