# Useful builtin functions

## `find_if(being, end, func_condition)`
- Definition: Find the first number in the vector/array that satisfies the condition
- Example: Find the first positive number in an array:
  ```cpp
  int a[n]; for(int&x:a) cin>>x;
  int first_positive_num = find_if(a,a+n,[](int x){return x>0});
  ```